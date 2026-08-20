<!-- Quelle: MIIIGModulStudie/TechnischeImplementierung/FHIR-Profile/DocumentReference.page.md @1394b43 (v2026.0.1). -->

---

**Beschreibung**

Dieses Profil beschreibt ein Dokument / Publikation in der Medizininformatik-Initiative.

Canonical: `https://www.medizininformatik-initiative.de/fhir/modul-studie/StructureDefinition/mii-pr-studie-dokument`

---

**Differential**

_Differential, Snapshot und weitere Sichten werden unterhalb dieser Einleitung direkt auf der Artefaktseite dargestellt._

---

**Hinweise**

| FHIR-Element | Erklärung |
|--------------|-----------|
| DocumentReference.id      | Must-support, jedoch optional        |
| DocumentReference.meta       | Must-support, jedoch optional         |
| DocumentReference.meta.profile       | Verpflichtend für die Abfrage im DIZ-Repository inkl. Versionsnummer des Profils. Siehe [CapabilityStatement](capability-statements.html). In allen anderen Fällen optional.         |
| DocumentReference.content.attachment.url | Diese absolute URL sollte auf einen Binary-Endpunkt eines FHIR-Servers verweisen. Die Hinweise der FHIR-Kernspezifikation zum [Abruf von Binary-Ressourcen](https://www.hl7.org/fhir/r4/binary.html#rest) sind zu beachten. |
| DocumentReference.content.attachment.title       | Der Titel sollte eine sinnvolle menschenlesbare Beschreibung enthalten, das Element sollte nicht für den Dateinamen verwendet werden. |
| DocumentReference.custodian     | Sollte der Standort nicht als Organization-Ressource verfügbar sein, kann auch ggf. Reference.display oder Referenz.identifier verwendet werden. |
| DocumentReference.author     | Sollte der Author nicht als Practitioner-Ressource verfügbar sein, kann auch ggf. Reference.display oder Referenz.identifier verwendet werden. |
|DocumentReference.context.related|Angabe des Studienkontexts|

---

**Mapping**

| FHIR Element | Logischer Datensatz |
|--------------|---------------------|
| DocumentReference.content.attachment.url |  Forschungsvorhaben.Publikation.url |
| DocumentReference.content.attachment.title |  Forschungsvorhaben.Publikation.Titel |
| DocumentReference.author |  Forschungsvorhaben.Publikation.Autor |

| FHIR Element | Logischer Datensatz |
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

**Beispiele**

Beispiel (minimal):

[mii-exa-studie-dokument](DocumentReference-mii-exa-studie-dokument.html)

---

**Suchparameter**

Die verpflichtenden Suchparameter dieses Profils sind auf der Seite [Search Parameters](search-parameters.html) beschrieben.
