<!-- TODO:REVIEW machine translation of source page ResearchStudy.page.md (de) @1394b43; untranslated runs remain in the original language (Gate C). -->

---

**Description**

This profile describes a study in the Medical Informatics Initiative.

Canonical: `https://www.medizininformatik-initiative.de/fhir/modul-studie/StructureDefinition/mii-pr-studie-studie`

---

**Differential**

_The differential, snapshot and further views render directly on this artifact page, below this introduction._

---

**Notes**

| FHIR element | Explanation |
|--------------|-----------|
| ResearchStudy.id      | Must-support, but optional        |
| ResearchStudy.meta       | Must-support, but optional         |
| ResearchStudy.meta.profile       | Mandatory for queries against the DIC repository, including the profile version. See [CapabilityStatement](capability-statements.html). Optional in all other cases.         |
| ResearchStudy.identifier | In most cases no NamingSystem will exist for assigning business IDs; a local NamingSystem should therefore be used. |
| ResearchStudy.extension:RekrutierungsstandGenauigkeit      | In-house coding may be used here. The next version of this module is expected to add further requirements towards a standardized ValueSet. |
| ResearchStudy.extension:Randomisierungsmethode      | In-house coding may be used here. The next version of this module is expected to add further requirements towards a standardized ValueSet. |
| ResearchStudy.extension:associatedParty | This extension can be used when more contact persons need to be stated for the study than the cardinality of ResearchStudy.principalInvestigator or ResearchStudy.sponsor allows. |
| ResearchStudy.category    | In-house coding may be used here. The next version of this module is expected to add further requirements towards a standardized ValueSet. |

---

**NamingSystems**

For the following study registers, preferred URLs for the corresponding NamingSystems are already defined:

| Register | URL |
|----------|-----|
| clinicaltrials.gov | https://clinicaltrials.gov |
| Deutsches Register Klinischer Studien (DRKS) | https://www.medizininformatik-initiative.de/fhir/modul-studie/sid/drks |
| Universal Trial Number (UTN) | https://www.medizininformatik-initiative.de/fhir/modul-studie/sid/utn |
| EudraCT | https://www.medizininformatik-initiative.de/fhir/modul-studie/sid/eudract |

---

**Mapping**

| FHIR element | Logical data set |
|--------------|---------------------|
| ResearchStudy.title |  Forschungsvorhaben.Titel  |
| ResearchStudy.focus |  Forschungsvorhaben.Studienfokus |
| ResearchStudy.keyword |  Forschungsvorhaben.Schlagwort |
| ResearchStudy.extension:OeffentlicherTitel |  Forschungsvorhaben.Titel.OeffentlicherTitel |
| ResearchStudy.extension:WissenschaftlicherTitel |  Forschungsvorhaben.Titel.WissenschaftlicherTitel |
| ResearchStudy.extension:Akronym |  Forschungsvorhaben.Titel.Akronym |
| ResearchStudy.extension:Rekrutierungsstart |  Forschungsvorhaben.Studiendesign.Rekrutierungsstart |
| ResearchStudy.arm.name |  Forschungsvorhaben.Studiendesign.Studienarm.Name |
| ResearchStudy.category |  Forschungsvorhaben.Studiendesign.Studientyp |
| ResearchStudy.extension:Rekrutierungsziel |  Forschungsvorhaben.Studiendesign.Rekrutierungsziel |
| ResearchStudy.extension:Rekrutierungsstand |  Forschungsvorhaben.Studiendesign.Rekrutierungsstand |
| ResearchStudy.extension:RekrutierungsstandGenauigkeit |  Forschungsvorhaben.Studiendesign.Rekrutierungsstand.RekrutierungsstandGenauigkeit |
| ResearchStudy.extension:RekrutierungsstandDatum |  Forschungsvorhaben.Studiendesign.Rekrutierungsstand.RekrutierungsstandDatum |
| ResearchStudy.category |  Forschungsvorhaben.Studiendesign.Randomisierungsmethode |

| FHIR element | Logical data set |
|--------------|---------------------|
| ResearchStudy.extension:finanzierung |  Forschungsvorhaben.Finanzierung |

| FHIR element | Logical data set |
|--------------|---------------------|
| ResearchStudy.identifier.value |  Forschungsvorhaben.BusinessID.id |
| ResearchStudy.identifier.system |  Forschungsvorhaben.BusinessID.System |

---

**Snapshot**



---


---

**Examples**

See example (minimal):

[mii-exa-studie-studie](ResearchStudy-mii-exa-studie-studie.html)

---

**Search parameters**

The mandatory search parameters of this profile are described on the [Search Parameters](search-parameters.html) page.
