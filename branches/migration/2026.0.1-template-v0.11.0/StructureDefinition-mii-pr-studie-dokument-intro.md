<!-- TODO:REVIEW machine translation of the German source page DocumentReference.page.md @1394b43; untranslated runs remain German (Gate C). -->

---

**Description**

This profile describes a document / publication in the Medical Informatics Initiative.

Canonical: `https://www.medizininformatik-initiative.de/fhir/modul-studie/StructureDefinition/mii-pr-studie-dokument`

---

**Differential**

_The differential, snapshot and further views render directly on this artifact page, below this introduction._

---

**Notes**

| FHIR element | Explanation |
|--------------|-----------|
| DocumentReference.id      | Must-support, but optional        |
| DocumentReference.meta       | Must-support, but optional         |
| DocumentReference.meta.profile       | Mandatory for queries against the DIC repository, including the profile version. See [CapabilityStatement](capability-statements.html). Optional in all other cases.         |
| DocumentReference.content.attachment.url | This absolute URL should point at a Binary endpoint of a FHIR server. The FHIR core specification's notes on [Abruf von Binary-Ressourcen](https://www.hl7.org/fhir/r4/binary.html#rest) must be observed. |
| DocumentReference.content.attachment.title       | The title should carry a meaningful human-readable description; the element should not be used for the file name. |
| DocumentReference.custodian     | If the site is not available as an Organization resource, Reference.display or Reference.identifier may be used instead. |
| DocumentReference.author     | If the author is not available as a Practitioner resource, Reference.display or Reference.identifier may be used instead. |
|DocumentReference.context.related|Statement of the study context|

---

**Mapping**

| FHIR element | Logical data set |
|--------------|---------------------|
| DocumentReference.content.attachment.url |  Forschungsvorhaben.Publikation.url |
| DocumentReference.content.attachment.title |  Forschungsvorhaben.Publikation.Titel |
| DocumentReference.author |  Forschungsvorhaben.Publikation.Autor |

| FHIR element | Logical data set |
|--------------|---------------------|
| DocumentReference.content.attachment.title |  Forschungsvorhaben.Datennutzungsantrag.Dokument.Name |
| DocumentReference.author |  Forschungsvorhaben.Datennutzungsantrag.Dokument.Autor |
| DocumentReference.content.attachment.contentType |  Forschungsvorhaben.Datennutzungsantrag.Dokument.Dateityp |
| DocumentReference.custodian |  Forschungsvorhaben.Datennutzungsantrag.Dokument.Standort |
| DocumentReference.content.attachment.size |  Forschungsvorhaben.Datennutzungsantrag.Dokument.Dateigroesse |
| DocumentReference.content.attachment.url |  Forschungsvorhaben.Datennutzungsantrag.Dokument.url |

---

**Snapshot**



---


---

**Examples**

Example (minimal):

[mii-exa-studie-dokument](DocumentReference-mii-exa-studie-dokument.html)

---

**Search parameters**

The mandatory search parameters of this profile are described on the [Search Parameters](search-parameters.html) page.
