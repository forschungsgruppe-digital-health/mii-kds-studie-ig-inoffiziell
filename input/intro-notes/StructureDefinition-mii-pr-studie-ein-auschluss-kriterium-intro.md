<!-- TODO:REVIEW machine translation of source page EvidenceVariable.page.md (de) @1394b43; untranslated runs remain in the original language (Gate C). -->

---

**Description**

This profile describes an inclusion or exclusion criterion within a study in the Medical Informatics Initiative.

Canonical: `https://www.medizininformatik-initiative.de/fhir/modul-studie/StructureDefinition/mii-pr-studie-ein-auschluss-kriterium`

---

**Differential**

_The differential, snapshot and further views render directly on this artifact page, below this introduction._

---

**Notes**

| FHIR element | Explanation |
|--------------|-----------|
| EvidenceVariable.id      | Must-support, but optional        |
| EvidenceVariable.meta       | Must-support, but optional         |
| EvidenceVariable.meta.profile       | Mandatory for queries against the DIC repository, including the profile version. See [CapabilityStatement](capability-statements.html). Optional in all other cases.         |
|EvidenceVariable.characteristic.description|Textual description of the criterion|
|EvidenceVariable.characteristic.definition[x]| The associated FHIR R5 backport extensions allow more data types than FHIR R4. When, for example, the definitionByCombination or definitionByTypeAndValue extension is used, definitionCodeableConcept must be filled with the Data-Absent-Reason code "unknown" so the 1..1 cardinality remains satisfied.|
|EvidenceVariable.characteristic.exclude|Boolean element defining whether this is an inclusion or an exclusion criterion|

---

**Mapping**

| FHIR element | Logical data set |
|--------------|---------------------|
|EvidenceVariable.characteristic.description|Forschungsvorhaben.Studiendesign.Einschlusskriterien.Kriterium|
|EvidenceVariable.characteristic.extension:definitionByTypeAndValue|Forschungsvorhaben.Studiendesign.Einschlusskriterien.Operator|
|EvidenceVariable.characteristic.extension:definitionByTypeAndValue|Forschungsvorhaben.Studiendesign.Einschlusskriterien.Masseinheit|
|EvidenceVariable.characteristic.extension:definitionByTypeAndValue|Forschungsvorhaben.Studiendesign.Einschlusskriterien.Wert|
|EvidenceVariable.characteristic.description|Forschungsvorhaben.Studiendesign.Ausschlusskriterien.Kriterium|
|EvidenceVariable.characteristic.extension:definitionByTypeAndValue|Forschungsvorhaben.Studiendesign.Ausschlusskriterien.Operator|
|EvidenceVariable.characteristic.extension:definitionByTypeAndValue|Forschungsvorhaben.Studiendesign.Ausschlusskriterien.Masseinheit|
|EvidenceVariable.characteristic.extension:definitionByTypeAndValue|Forschungsvorhaben.Studiendesign.Ausschlusskriterien.Wert|

---

**Snapshot**



---


---

**Examples**

Example (minimal):

[mii-exa-studie-ein-auschluss-kriterium](EvidenceVariable-mii-exa-studie-ein-auschluss-kriterium.html)

---

**Search parameters**

The mandatory search parameters of this profile are described on the [Search Parameters](search-parameters.html) page.
