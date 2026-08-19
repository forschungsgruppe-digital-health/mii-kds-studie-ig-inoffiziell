<!-- Quelle: MIIIGModulStudie/TechnischeImplementierung/FHIR-Profile/ResearchSubject.page.md @1394b43 (v2026.0.1). -->

---

**Beschreibung**

Canonical: `https://www.medizininformatik-initiative.de/fhir/modul-studie/StructureDefinition/mii-pr-studie-proband`

**Differential**

_Differential, Snapshot und weitere Sichten werden unterhalb dieser Einleitung direkt auf der Artefaktseite dargestellt._

---

Dieses Profil beschreibt eine ProbandIn in der Medizininformatik-Initiative.

---

**Hinweise**

| FHIR-Element | Erklärung |
|--------------|-----------|
| ResearchSubject.id      | Must-support, jedoch optional        |
| ResearchSubject.meta       | Must-support, jedoch optional         |
| ResearchSubject.meta.profile       | VERPFLICHTEND für die Abfrage im DIZ-Repsoitory inkl Versionsnummer des Profils. Siehe [CapabilityStatement](capability-statements.html). In allen anderen Fällen optional.         |
| Patient.identifier:subjectIdentificationCode      | Fixes NamingSystem zur einheitlichen, standort-übergreifenden Abfrage des Identifiers (bei Auswertungen)         |
| ResearchSubject.period.start      | Startdatum (Einschluss der PatientIn in die Studie)      |
| ResearchSubject.period.end      | Enddatum (Abschluss der Studie oder Ausschluss der PatientIn)       |
| ResearchSubject.study      | Referenz auf die Metadaten der Studie an welcher die PatientIn teilnimmt. |
| ResearchSubject.individual      | Jede ProbandIn MUSS einer PatientIn zugeordnet werden. |
| ResearchSubject.consent      | Einwilligung in die Studie oder regulatorische Grundlage MUSS vorliegen. Weitere Vorgaben für die Modellierung des Consents können durch andere Module entstehen. |

---

**Mapping**

| FHIR-Element | Logischer Datensatz |
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

**Beispiele**

Siehe Beispiel (minimal):

[mii-exa-studie-proband](ResearchSubject-mii-exa-studie-proband.html)

---

**Suchparameter**

Die verpflichtenden Suchparameter dieses Profils sind auf der Seite [Search Parameters](search-parameters.html) beschrieben.
