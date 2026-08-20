<!-- Quelle: MIIIGModulStudie/TechnischeImplementierung/FHIR-Profile/EvidenceVariable.page.md @1394b43 (v2026.0.1). -->

---

**Beschreibung**

Dieses Profil beschreibt ein Ein- und Auschlusskriterium innerhalb einer Studie in der Medizininformatik-Initiative.

Canonical: `https://www.medizininformatik-initiative.de/fhir/modul-studie/StructureDefinition/mii-pr-studie-ein-auschluss-kriterium`

---

**Differential**

_Differential, Snapshot und weitere Sichten werden unterhalb dieser Einleitung direkt auf der Artefaktseite dargestellt._

---

**Hinweise**

| FHIR-Element | Erklärung |
|--------------|-----------|
| EvidenceVariable.id      | Must-support, jedoch optional        |
| EvidenceVariable.meta       | Must-support, jedoch optional         |
| EvidenceVariable.meta.profile       | Verpflichtend für die Abfrage im DIZ-Repository inkl. Versionsnummer des Profils. Siehe [CapabilityStatement](capability-statements.html). In allen anderen Fällen optional.         |
|EvidenceVariable.characteristic.description|Textuelle Beschreibung dess Kriteriums|
|EvidenceVariable.characteristic.definition[x]| In den dazugehöirgen Backport-Extensions aus FHIR R5 sind weitere Datentypen als in FHIR R4 erlaubt. Sollte z.B. die Extension definitionByCombination oder definitionByTypeAndValue verwendet werden, so muss definitionCodeableConcept mit dem Data-Absent-Reason Code "unknown" befüllt werden, sodass die Kardinalität von 1..1 erfüllt bleibt.|
|EvidenceVariable.characteristic.exclude|Boolesches Element welches definiert, ob es sich um ein Einschluss- oder Ausschlusskriterium handelt|

---

**Mapping**

| FHIR Element | Logischer Datensatz |
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

**Beispiele**

Beispiel (minimal):

[mii-exa-studie-ein-auschluss-kriterium](EvidenceVariable-mii-exa-studie-ein-auschluss-kriterium.html)

---

**Suchparameter**

Die verpflichtenden Suchparameter dieses Profils sind auf der Seite [Search Parameters](search-parameters.html) beschrieben.
