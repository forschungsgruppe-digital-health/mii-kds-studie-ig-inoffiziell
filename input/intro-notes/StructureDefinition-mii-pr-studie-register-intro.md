<!-- TODO:REVIEW machine translation of source page Library.page.md (de) @1394b43; untranslated runs remain in the original language (Gate C). -->

---

**Description**

This profile describes a research register in the Medical Informatics Initiative.

Canonical: `https://www.medizininformatik-initiative.de/fhir/modul-studie/StructureDefinition/mii-pr-studie-register`

---

**Differential**

_The differential, snapshot and further views render directly on this artifact page, below this introduction._

---

**Notes**

| FHIR element | Explanation |
|--------------|-----------|
| Library.id      | Must-support, but optional        |
| Library.meta       | Must-support, but optional         |
| Library.meta.profile       | Mandatory for queries against the DIC repository, including the profile version. See [CapabilityStatement](capability-statements.html). Optional in all other cases.         |
| Library.name | A suitable human-readable name should be used |
| Library.identifier | In most cases no NamingSystem exists yet for assigning register IDs; a local NamingSystem should therefore be used. |
| Library.relatedArtifact.document.url | Homepage of the register or link to further documentation |

---

**Mapping**

| FHIR element | Logical data set |
|--------------|---------------------|
| Library.name |  Forschungsvorhaben.Studienregister.Registername |
| Library.identifier |  Forschungsvorhaben.Studienregister.RegisterId |
| Library.relatedArtifact.document.url |  Forschungsvorhaben.Studienregister.url |

---

**Snapshot**



---


---

**Examples**

Example (minimal):

[mii-exa-studie-register](Library-mii-exa-studie-register.html)

---

**Search parameters**

The mandatory search parameters of this profile are described on the [Search Parameters](search-parameters.html) page.
