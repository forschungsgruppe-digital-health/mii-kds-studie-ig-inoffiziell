<!-- Quelle: MIIIGModulStudie/TechnischeImplementierung/FHIR-Profile/Library.page.md @1394b43 (v2026.0.1). -->

---

**Beschreibung**

Dieses Profil beschreibt ein Forschungsregister in der Medizininformatik-Initiative.

Canonical: `https://www.medizininformatik-initiative.de/fhir/modul-studie/StructureDefinition/mii-pr-studie-register`

---

**Differential**

_Differential, Snapshot und weitere Sichten werden unterhalb dieser Einleitung direkt auf der Artefaktseite dargestellt._

---

**Hinweise**

| FHIR-Element | Erklärung |
|--------------|-----------|
| Library.id      | Must-support, jedoch optional        |
| Library.meta       | Must-support, jedoch optional         |
| Library.meta.profile       | Verpflichtend für die Abfrage im DIZ-Repository inkl. Versionsnummer des Profils. Siehe [CapabilityStatement](capability-statements.html). In allen anderen Fällen optional.         |
| Library.name | Es sollte ein geeigneter menschenlesbarer Name verwendet werden |
| Library.identifier | In den meisten Fällen existiert bisher kein NamingSystem für die Vergabe der RegisterIds. Ein eigenes lokales NamingSystem sollte daher verwendet werden. |
| Library.relatedArtifact.document.url | Homepage des Registers bzw. Link zur weiterführenden Dokumentation |

---

**Mapping**

| FHIR Element | Logischer Datensatz |
|--------------|---------------------|
| Library.name |  Forschungsvorhaben.Studienregister.Registername |
| Library.identifier |  Forschungsvorhaben.Studienregister.RegisterId |
| Library.relatedArtifact.document.url |  Forschungsvorhaben.Studienregister.url |

---

**Snapshot**



---


---

**Beispiele**

Beispiel (minimal):

[mii-exa-studie-register](Library-mii-exa-studie-register.html)

---

**Suchparameter**

Die verpflichtenden Suchparameter dieses Profils sind auf der Seite [Search Parameters](search-parameters.html) beschrieben.
