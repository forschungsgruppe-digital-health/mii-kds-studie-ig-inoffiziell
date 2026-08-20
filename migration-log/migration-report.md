# Migration report — MII KDS Modul Studie (Medizinisches Forschungsvorhaben) → MII KDS module template

**Try-run** executed 2026-08-19 with `mii-ig-migration` @ agent-skills **v0.15.1** onto
module-template **v0.11.0**, in a NEW repository
`forschungsgruppe-digital-health/mii-kds-studie-ig-inoffiziell` (a human decision recorded up
front: the MII source repository is strictly read-only for this exercise; an in-place migration
per spec §5.2 was deliberately not performed).

## L0 — Read this first (for everyone)

The MII publishes the "Studie" module as FHIR profiles (machine-readable rules) plus a German
guide on Simplifier. This migration moved both onto the MII KDS module template, which builds the
same guide with the standard HL7 toolchain (SUSHI + IG Publisher) on GitHub — bilingual (English
default, German mirror), with the TF-KDS-agreed page set. **Nothing was published**; the result is
a working-branch preview in an unofficial sandbox repository. All the module's technical
identifiers (canonical URLs, IDs, package id, version) are unchanged — consumers would notice no
difference. The open items below are decisions for humans, not defects in the build: the build is
green (SUSHI 0 errors; the 17 remaining QA errors exist in the source's own content).

- Source: `medizininformatik-initiative/kerndatensatzmodul-studie` @ `1394b43` (= tag
  `v2026.0.1`), shape A; narrative from the **in-repo** Simplifier guide tree (22 German pages).
- Rendered preview: `branches/migration/2026.0.1-template-v0.11.0/` on the sandbox repo's Pages.
- Verification: **45 IDENTISCH · 8 DIVERGIERT (all triaged, see ③/notes) · 14 NICHT PRÜFBAR**.

## ① Decision queue (Gate A — someone must choose)

| # | Decision | Evidence | Proposed owner |
|---|---|---|---|
| 1 | **License.** No machine source declares one (no LICENSE file; registry manifests `license=null`; `license-terms.fsh` is a literal TODO). The guide's own copyright section (Index page) declares **© 2019+ TMF e. V., CC BY 4.0** — carried into `sushi-config.yaml` as `CC-BY-4.0` with a provenance comment. Confirm, or correct upstream. | run.log `2.2 license-missing` + `2.2 license-amended` | MII / TMF |
| 2 | **Version 2026.0.1 vs 2026.0.2.** The registry's `dist-tags.latest` is 2026.0.2; the source tree, tag and sushi-config all say 2026.0.1 (no tag/commit for .2 found). Target carries the source tree's 2026.0.1. | run.log `2.1 identity-contradiction` + `decision` | MII module team |
| 3 | **Title.** The source declares no `title` anywhere; target uses the template pattern "MII Implementation Guide Medizinisches Forschungsvorhaben". | run.log `2.2 decision` | MII module team |
| 4 | **Description language.** Source ships a German package description; target's is an English summary (bilingual guide, EN default). | run.log `2.1 decision` | Gate A reviewer |
| 5 | **Template-machinery dependencies.** Added to the source's set (`hl7.fhir.extensions.r5`, meta 2026.0.0): `hl7.fhir.uv.crmi` 2.0.0 (CRMI profile claims) and direct pins `hl7.terminology.r4` 7.3.0 / `hl7.fhir.uv.extensions.r4` 5.3.0 (publisher auto-injection guard). | run.log `2.1 dependency-note` | Gate A reviewer |
| 6 | **Expansion manifest.** The template's default `Parameters-expansion-manifest.json` (id `mii-param-studie-manifest`) is wired; the source pins no expansion parameters. Keep, adapt, or drop. | run.log `5.3 manifest-decision` | MII module team |
| 7 | **APPROVAL_DATE / author contact / NCI topic** placeholders were filled with defensible stand-ins (tag date 2026-01-09; `info@medizininformatik-initiative.de`; NCI C15206 *Clinical Study*) — all marked for confirmation. | commit diff, sushi-config comments | MII module team |
| 8 | **`example.org` canonicals.** The 2 CS + 2 VS introduced with the 2026 examples use `http://example.org/...` canonicals (source-authored; carried unchanged, declared via `special-url`). Upstream may want real canonicals. | qa triage; sushi-config `special-url` comment | MII module team |

## ② Review queue (Gates B/C — someone must check)

1. **All English pages are machine translations** of the German source, each marked
   `TODO:REVIEW`; recurring boilerplate is fully translated, a few long German passages remain
   verbatim inside EN pages (marked). (Gate C)
2. **Terminologie discrepancy:** the source's Terminologie page claims "no own CodeSystems and
   ValueSets"; the package ships 2+2. Both target terminology pages state the discrepancy. (Gate B)
3. **Scenario narrative placement** (Beschreibung von Szenarien → `guidance.md`) is the spec §9
   default; reviewers may prefer `implementer-guidance.md`. (Gate B)
4. **Organization mapping tables** were summarized on `implementer-guidance.md`/`profiles.md`;
   the full contact/site mapping tables remain source-only (marked in the page map). (Gate B)
5. **Untranslated Änderungsprotokoll:** `changes.md` carries the German release notes verbatim in
   both languages (change history is German by origin). (Gate C)

## ③ QA triage (what the build says, and whose problem it is)

`qa.txt`: **17 errors / 661 warnings** (42 errors before the `special-url` fix). Provenance:

| Class | Count | Whose problem |
|---|---|---|
| R5-backport ValueSet bindings unresolvable in R4 (`characteristic-combination`, `research-study-party-role`, …) | 10 SD + 5 instance refs | **Source-inherent** — bindings verbatim in source FSH (e.g. `EvidenceVariable.fsh:94`, `ResearchStudy.fsh:191`); R5 ValueSets do not exist in the R4 package universe. Upstream candidate fix: bind copies or drop bindings. |
| Library example narrative: empty hyperlink | 2 + 2 rendered link errors | **Source-inherent** — example `text.div` authored with an empty `<a>`. |
| Canonical-vs-URL mismatches | 0 (was 12) | **Fixed in migration** via `special-url` (12 source-authored out-of-canonical URLs; canonicals untouched). |
| `retired {{title}}` literal on 6 `-definitions.html` pages | rendering note | **Publisher chrome** on R5-backport modifier boilerplate; absent from all narrative sources. |

A source-baseline build (unmigrated) could not be fetched (source publishes no `qa.txt` at a
stable URL — `gh-pages/qa.txt` 404, 2026-08-19); the source-inherence claims above rest on direct
file:line inspection instead.

## Applied polish fixes (revertible — a human confirms or reverts)

Review-round adaptations, applied as **one commit `f166d7c`** — revert with
`git revert f166d7c` if a reviewer disagrees. Each is a presentation decision,
never content or identity:

| Fix | Was | Now | Revert effect |
|---|---|---|---|
| CapabilityStatement page | link to the artifact page (extra click) | rendered INLINE via `lang-fragment` | back to link-only |
| Index: authors | separator-joined run-in line | simple list (template index style) | back to run-in line |
| Index: disclaimer | bullet list (carried from source) | prose sentences (template index style) | back to bullets |
| Logical-models page | inline LM tree include rendering only an ERROR | source-defect note + artifact-page link (root cause: `LogicalModel.fsh:100` bare-name `contentReference Studienarm` — **upstream fix needed**, one line: use the full path) | back to the broken include (self-heals once upstream fixes the reference) |

## Content map

`migration-log/page-map.tsv` — 22 source pages → 14 targets, 3 RETIRED with reason (2 deliberately
empty index pages, 1 near-duplicate), per-profile Suchparameter sections → `search-parameters.md`,
7 per-profile pages → `input/intro-notes/` (spec §9 N>2 rule), plus the template-shipped
IG-resource intro page (v0.11.0). M9 decisions: researcher-guidance/operations/metadata REMOVED;
extensions/search-parameters/value-sets/code-systems KEPT. M11: example box deleted, both
languages.

## Identity (verified unchanged)

| Field | Value | Source |
|---|---|---|
| canonical | `https://www.medizininformatik-initiative.de/fhir/modul-studie` | sushi-config (= template pattern, coincidentally identical) |
| id / name | `mii-ig-studie` / `MII_IG_Medizinisches_Forschungsvorhaben` | sushi-config |
| packageId | `de.medizininformatikinitiative.kerndatensatz.studie` | sushi-config + registry |
| version | `2026.0.1` | sushi-config + tag (① #2) |
| license | `CC-BY-4.0` | guide Index copyright section (tier R; ① #1) |
| publisher (IG chrome) | NUM-DIZ | template ≥ v1.0 rule (spec §9a overrides source-wins) |
| publisher (artifacts) | Medizininformatik Initiative | module's own `Publisher` RuleSet, untouched |
| dependencies | source set + recorded template machinery | ① #5 |

## Verification

`verify-migration.py` (v0.15.1): **45 IDENTISCH / 8 DIVERGIERT / 14 NICHT PRÜFBAR** (exit 3 —
"incomplete, not a pass", as designed). The 8 DIVERGIERT: 2× C5 (the v0.11.0 IG-resource intro
page — menu-less **by template design**, linked from Home; the verifier's template-page list is
pinned at v0.10.3), 1× F1 title + 1× P4 `?version=current` (both recorded Gate-A decisions,
run.log `decision` lines), 4× R2 (publisher chrome / verifier-message artifact — triage in
run.log `11 triage`). The 14 NICHT PRÜFBAR are mostly guide-harvest-dependent checks that do not
apply to the in-repo-narrative route plus the missing source QA baseline; each stays named here
rather than written as a pass.

## Protocol

Generated from `migration-log/run.log` (append-only, committed): source pin → identity ledger
(P/R tiers, 2 contradiction WARNs → decisions) → skeleton on template v0.11.0 (bootstrap,
placeholder substitution incl. 3 file renames) → FSH transfer (17 files, template scaffold
skipped, SUSHI **0 errors**, 60 resources) → §9/§9a page set (fql-scan `--strict` clean over 18
files) → bilingual setup (.po adapted; menus; lang-fragment includes) → CI build (publisher
2.3.2, Jekyll render green; preview published) → special-url fix (42→17 qa errors) →
verify-migration (two runs; L2/L3 closed by canonical log lines + decisions). Toolchain: SUSHI
3.20.1, IG Publisher 2.3.2 (sha-pinned in the target's workflows), skill v0.15.1.

## Mini-glossary

**IG** implementation guide — the rendered specification website. **SUSHI/FSH** compiler and
shorthand language for FHIR profiles. **IG Publisher** HL7's renderer. **Canonical URL** the
stable identifier consumers reference — never changed here. **Gate A–D** the four mandatory human
review gates of the migration skill. **§9a** the template's TF-KDS page-set rules.
