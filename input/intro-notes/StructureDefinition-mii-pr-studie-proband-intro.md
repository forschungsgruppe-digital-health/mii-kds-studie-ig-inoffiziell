<!-- TODO:REVIEW machine translation of source page ResearchSubject.page.md (de) @1394b43; untranslated runs remain in the original language (Gate C). -->

---

**Description**

Canonical: `https://www.medizininformatik-initiative.de/fhir/modul-studie/StructureDefinition/mii-pr-studie-proband`

**Differential**

_The differential, snapshot and further views render directly on this artifact page, below this introduction._

---

This profile describes a research subject in the Medical Informatics Initiative.

---

**Notes**

| FHIR element | Explanation |
|--------------|-----------|
| ResearchSubject.id      | Must-support, but optional        |
| ResearchSubject.meta       | Must-support, but optional         |
| ResearchSubject.meta.profile       | MANDATORY for queries against the DIC repository, including the profile version. See [CapabilityStatement](capability-statements.html). Optional in all other cases.         |
| Patient.identifier:subjectIdentificationCode      | Fixed NamingSystem for uniform, cross-site identifier queries (in analyses)         |
| ResearchSubject.period.start      | Start date (inclusion of the patient in the study)      |
| ResearchSubject.period.end      | End date (completion of the study or exclusion of the patient)       |
| ResearchSubject.study      | Reference to the metadata of the study the patient participates in. |
| ResearchSubject.individual      | Every research subject MUST be linked to a patient. |
| ResearchSubject.consent      | Consent to the study or a regulatory basis MUST exist. Further requirements for modelling consent may arise from other modules. |

---

**Mapping**

| FHIR element | Logical data set |
|--------------|-----------|
| ResearchSubject.identifier:subjectIdentificationCode       | Person.Studienteilnehmer.SubjektIdentifizierungscode         |
| ResearchSubject.status       | Person.Studienteilnehmer.StatusDerTeilnahme         |
| ResearchSubject.period.start       | Person.Studienteilnehmer.BeginnTeilnahme         |
| ResearchSubject.period.end       | Person.Studienteilnehmer.EndeTeilnahme         |
| ResearchSubject.consent       | Person.Studienteilnehmer.Rechtsgrundlage        |

---

**Snapshot**



---


---

**Examples**

See example (minimal):

[mii-exa-studie-proband](ResearchSubject-mii-exa-studie-proband.html)

---

**Search parameters**

The mandatory search parameters of this profile are described on the [Search Parameters](search-parameters.html) page.
