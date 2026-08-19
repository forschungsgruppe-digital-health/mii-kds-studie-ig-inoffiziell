<!-- Quelle: MIIIGModulStudie/TechnischeImplementierung/FHIR-Profile/PractitionerRole.page.md @1394b43 (v2026.0.1). -->

---

**Beschreibung**

Dieses Profil beschreibt eine beteiligte Person innerhalb einer Studie in der Medizininformatik-Initiative.

Canonical: `https://www.medizininformatik-initiative.de/fhir/modul-studie/StructureDefinition/mii-pr-studie-beteiligte-person`

---

**Differential**

_Differential, Snapshot und weitere Sichten werden unterhalb dieser Einleitung direkt auf der Artefaktseite dargestellt._

---

**Hinweise**

| FHIR-Element | Erklärung |
|--------------|-----------|
| PractitionerRole.id      | Must-support, jedoch optional        |
| PractitionerRole.meta       | Must-support, jedoch optional         |
| PractitionerRole.meta.profile       | Verpflichtend für die Abfrage im DIZ-Repository inkl. Versionsnummer des Profils. Siehe [CapabilityStatement](capability-statements.html). In allen anderen Fällen optional.         |
| PractitionerRole.code      | Hausinterne Kodierung kann hier verwendet werden. Die nächste Version des vorliegenden Moduls wird hier voraussichtlich weitere Vorgaben zur Standardisierung eines ValueSets fordern. |
| PractitionerRole.telecom      | Es ist drauf zu achten, dass hier nur Informationen exponiert werden, die bereits durch die Studie ansich veröffentlicht wurden |
| PractitionerRole.organization | Um alle zu einer Studie zugehörigen Personen zu finden ist die Verwendung von Referenz.reference anstelle von Referent.identifier zu bevorzugen.|

---

**Mapping**

| FHIR Element | Logischer Datensatz |
|--------------|---------------------|
| PractitionerRole.code |  Forschungsvorhaben.Beteiligter.Rolle |
| PractitionerRole.telecom |  Forschungsvorhaben.Beteiligter.Kontakt |
| PractitionerRole.organization |  Forschungsvorhaben.Beteiligter.Standort |

| FHIR Element | Logischer Datensatz |
|--------------|---------------------|
| PractitionerRole.code |  Forschungsvorhaben.Studienleiter |
| PractitionerRole.telecom |  Forschungsvorhaben.Studienleiter.Kontakt |
| PractitionerRole.organization |  Forschungsvorhaben.Studienleiter.Standort |

---

**Snapshot**



---


---

**Beispiele**

Beispiel (minimal):

[mii-exa-studie-beteiligte-person](PractitionerRole-mii-exa-studie-beteiligte-person.html)

---

**Suchparameter**

Die verpflichtenden Suchparameter dieses Profils sind auf der Seite [Search Parameters](search-parameters.html) beschrieben.
