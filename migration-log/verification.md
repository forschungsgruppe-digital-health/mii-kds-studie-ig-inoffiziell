## Verification (generated — do not retype)

Produced by `verify-migration.py` from the target tree AND `migration-log/run.log`, the two oracles. **45 IDENTISCH · 8 DIVERGIERT · 14 NICHT PRÜFBAR.**

| Layer | Check | IDENTISCH | DIVERGIERT | NICHT PRÜFBAR |
|---|---|---|---|---|
| conservation | C1 | 1 | 0 | 0 |
| conservation | C2 | 2 | 0 | 0 |
| conservation | C3 | 0 | 0 | 1 |
| conservation | C4 | 0 | 0 | 1 |
| conservation | C5 | 2 | 2 | 0 |
| conservation | C6 | 0 | 0 | 1 |
| fidelity | F1 | 7 | 1 | 1 |
| fidelity | F2 | 2 | 0 | 3 |
| fidelity | F3 | 0 | 0 | 1 |
| fidelity | F4 | 1 | 0 | 0 |
| provenance | P1 | 1 | 0 | 0 |
| provenance | P2 | 1 | 0 | 0 |
| provenance | P3 | 1 | 0 | 0 |
| provenance | P4 | 0 | 1 | 0 |
| rendering | R1 | 2 | 0 | 1 |
| rendering | R2 | 0 | 4 | 0 |
| rendering | R3 | 1 | 0 | 0 |
| rendering | R4 | 1 | 0 | 0 |
| rendering | R5 | 1 | 0 | 0 |
| log | L0 | 1 | 0 | 0 |
| log | L1 | 1 | 0 | 0 |
| log | L2 | 16 | 0 | 3 |
| log | L3 | 3 | 0 | 0 |
| log | L4 | 1 | 0 | 2 |

### DIVERGIERT — each one a stop or a recorded decision

| id | Check | Subject | Evidence | Next action | Auto-fixable |
|---|---|---|---|---|---|
| `C5-e8746e` | C5 | input/pagecontent/ImplementationGuide-mii-ig-studie.md | narrative page in NO menu entry -- rendered, but reachable only by typing its URL | add it to input/includes/menu.xml (and the per-language copies), or retire the page | no |
| `C5-c55eba` | C5 | input/pagecontent/ImplementationGuide-mii-ig-studie.md | target page is neither a template page nor the target of any page-map row -- it appeared during migration | name its provenance in the page map, or remove it; a page nobody can trace to a source is content a reviewer cannot check | no |
| `F1-b5b102` | F1 | title | target MII Implementation Guide Medizinisches Forschungsvorhaben  vs  source Medizininformatik Initiative - Modul Medizinisches Forschung… | the SOURCE wins (spec 2.2); restore it or record the divergence as a Gate-A decision -- never normalise silently | no |
| `P4-379bde` | P4 | source guide version | the recorded guide URL carries ?version=current (run.log, action package-identity) -- the live, editable project, not a published version | re-harvest from a PUBLISHED version; `current` is not reproducible. Where the guide has no published version at all, that is the finding -- record it as such rather than leaving the pin unstated | no |
| `R2-4c016c` | R2 | /private/tmp/claude-503/-Users-marcel-Development-cross-hub-patientportal/e2e22580-543a-4bf5-88cc-83677866f38a/scratchpad/studie-rendered/branches/migration/2026.0.1-template-v0.11.0/de id="publish-box" [{{] | on 6 page(s), e.g. StructureDefinition-mii-pr-studie-ein-auschluss-kriterium-definitions.html: e applications should not use a retired {{title}} without due consideration Primitive Valu… | rendered header/footer metadata defect -- qa.txt does not report it. Fix the metadata it renders (a jurisdiction code the template cannot resolve is the measured case) | no |
| `R2-b75b07` | R2 | /private/tmp/claude-503/-Users-marcel-Development-cross-hub-patientportal/e2e22580-543a-4bf5-88cc-83677866f38a/scratchpad/studie-rendered/branches/migration/2026.0.1-template-v0.11.0/de id="ig-status" [{{] | on 1 page(s), e.g. searchform.html: Search {{title}} (Current Build) | rendered header/footer metadata defect -- qa.txt does not report it. Fix the metadata it renders (a jurisdiction code the template cannot resolve is the measured case) | no |
| `R2-ea1019` | R2 | /private/tmp/claude-503/-Users-marcel-Development-cross-hub-patientportal/e2e22580-543a-4bf5-88cc-83677866f38a/scratchpad/studie-rendered/branches/migration/2026.0.1-template-v0.11.0/en id="publish-box" [{{] | on 6 page(s), e.g. StructureDefinition-mii-pr-studie-ein-auschluss-kriterium-definitions.html: e applications should not use a retired {{title}} without due consideration Primitive Valu… | rendered header/footer metadata defect -- qa.txt does not report it. Fix the metadata it renders (a jurisdiction code the template cannot resolve is the measured case) | no |
| `R2-bcaede` | R2 | /private/tmp/claude-503/-Users-marcel-Development-cross-hub-patientportal/e2e22580-543a-4bf5-88cc-83677866f38a/scratchpad/studie-rendered/branches/migration/2026.0.1-template-v0.11.0/en id="ig-status" [{{] | on 1 page(s), e.g. searchform.html: Search {{title}} (Current Build) | rendered header/footer metadata defect -- qa.txt does not report it. Fix the metadata it renders (a jurisdiction code the template cannot resolve is the measured case) | no |

### NICHT PRÜFBAR — not a pass; each needs a human

| id | Check | Subject | Why not mechanisable | Who does what |
|---|---|---|---|---|
| `C3-c33506` | C3 | source guide pages | no harvest manifest and no source pagecontent to enumerate | supply --harvest-tsv or --source; a migration whose source page set is unknown cannot claim conservation |
| `C4-fee309` | C4 | narrative text runs | no harvested source narrative (./migration-log/guide-harvest/pagecontent) and no source pagecontent | supply --harvest-dir or --source; without a source text there is nothing to conserve against |
| `C6-cc9590` | C6 | content placement | no harvested source narrative to place | supply --harvest-dir or --source |
| `F1-7bae24` | F1 | license | no source value (neither the source tree nor the claims ledger yields one) | supply it at Gate A -- an identity field nobody can compare is not a field that matches |
| `F2-fd0e73` | F2 | hl7.fhir.uv.crmi | target-only dependency 2.0.0 (not in the source) | confirm at Gate A that this is template machinery (hl7.fhir.uv.crmi is) and not an accidental addition |
| `F2-047205` | F2 | hl7.fhir.uv.extensions.r4 | target-only dependency 5.3.0 (not in the source) | confirm at Gate A that this is template machinery (hl7.fhir.uv.crmi is) and not an accidental addition |
| `F2-8f9355` | F2 | hl7.terminology.r4 | target-only dependency 7.3.0 (not in the source) | confirm at Gate A that this is template machinery (hl7.fhir.uv.crmi is) and not an accidental addition |
| `F3-1a29c4` | F3 | license | target declares CC-BY-4.0 with NO tier evidence behind it (no claim in identity-claims.tsv) | read the source's LICENSE (repo-identity.sh) and claim it, or confirm the value at Gate A. The template's literal CC-BY-4.0 reaches here unflagged otherwise |
| `R1-76f413` | R1 | source-versus-target rendering | no harvested source HTML (./migration-log/guide-harvest/html) and/or no page map | harvest with --keep-html and write the page map; without a source rendering, 'non-empty where non-empty in the source' has no reference |
| `L2-07bdbb` | L2 | 5.1c simplifier-discover | no line in the log; the step is conditional (no rendered-IG URL was supplied) | confirm the condition did not hold -- Without the discovery chain the guide is not found, and a migration then ships the template's starter pages. |
| `L2-930ba2` | L2 | 5.1d guide-harvest | no line in the log; the step is conditional (the narrative is not in the repository) | confirm the condition did not hold -- This is the step whose absence shipped the template's starter pages under a module's name. |
| `L2-a85d96` | L2 | 5.5 gen-page-title-po | no line in the log; the step is conditional (bilingual target) | confirm the condition did not hold -- Page titles fall back to the default language with no error anywhere. |
| `L4-106e61` | L4 | conversion count | no `gofsh-convert … actual=` line in the log | shape B only; for shape A there is nothing to convert |
| `L4-f17740` | L4 | page count | no harvested count in the log and/or no harvest manifest | harvest the guide (step 2c) where the narrative is not in the repo |

**Inputs:** target `.` · source `/private/tmp/claude-503/-Users-marcel-Development-cross-hub-patientportal/e2e22580-543a-4bf5-88cc-83677866f38a/scratchpad/studie-src` · rendered `/private/tmp/claude-503/-Users-marcel-Development-cross-hub-patientportal/e2e22580-543a-4bf5-88cc-83677866f38a/scratchpad/studie-rendered/branches/migration/2026.0.1-template-v0.11.0` · log `./migration-log/run.log`
