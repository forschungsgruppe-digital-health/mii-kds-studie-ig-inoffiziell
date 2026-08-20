<!-- TODO:REVIEW machine translation of source page PractitionerRole.page.md (de) @1394b43; untranslated runs remain in the original language (Gate C). -->

---

**Description**

This profile describes an involved person innerhalb einer Studie in der Medizininformatik-Initiative.

Canonical: `https://www.medizininformatik-initiative.de/fhir/modul-studie/StructureDefinition/mii-pr-studie-beteiligte-person`

---

**Differential**

_The differential, snapshot and further views render directly on this artifact page, below this introduction._

---

**Notes**

| FHIR element | Explanation |
|--------------|-----------|
| PractitionerRole.id      | Must-support, but optional        |
| PractitionerRole.meta       | Must-support, but optional         |
| PractitionerRole.meta.profile       | Mandatory for queries against the DIC repository, including the profile version. See [CapabilityStatement](capability-statements.html). Optional in all other cases.         |
| PractitionerRole.code      | In-house coding may be used here. The next version of this module is expected to add further requirements towards a standardized ValueSet. |
| PractitionerRole.telecom      | Es ist drauf zu achten, dass hier nur Informationen exponiert werden, die bereits durch die Studie ansich veröffentlicht wurden |
| PractitionerRole.organization | Um alle zu einer Studie zugehörigen Personen zu finden ist die Verwendung von Referenz.reference anstelle von Referent.identifier zu bevorzugen.|

---

**Mapping**

| FHIR element | Logical data set |
|--------------|---------------------|
| PractitionerRole.code |  Forschungsvorhaben.Beteiligter.Rolle |
| PractitionerRole.telecom |  Forschungsvorhaben.Beteiligter.Kontakt |
| PractitionerRole.organization |  Forschungsvorhaben.Beteiligter.Standort |

| FHIR element | Logical data set |
|--------------|---------------------|
| PractitionerRole.code |  Forschungsvorhaben.Studienleiter |
| PractitionerRole.telecom |  Forschungsvorhaben.Studienleiter.Kontakt |
| PractitionerRole.organization |  Forschungsvorhaben.Studienleiter.Standort |

---

**Snapshot**



---


---

**Examples**

Example (minimal):

[mii-exa-studie-beteiligte-person](PractitionerRole-mii-exa-studie-beteiligte-person.html)

---

**Search parameters**

The mandatory search parameters of this profile are described on the [Search Parameters](search-parameters.html) page.
