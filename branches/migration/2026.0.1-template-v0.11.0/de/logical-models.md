# Logische Modelle - MII Implementation Guide Medizinisches Forschungsvorhaben v2026.0.1

* [**Inhaltsverzeichnis**](toc.md)
* **Logische Modelle**

## Logische Modelle

 Diese Seite enthält Übersetzungen aus der Originalsprache, in der der Leitfaden verfasst wurde. Informationen zu diesen Übersetzungen und Anweisungen zum Abgeben von Feedback zu den Übersetzungen finden Sie [hier](translationinfo.md). 

Das Informationsmodell für das Modul Medizinisches Forschungsvorhaben wurde als FHIR Logical Model abgebildet:

> **Bekannter Quell-Defekt (Korrektur upstream erforderlich):** Das Element `Studiendesign.Studienarm.Studienarm` des Logical Models deklariert eine `contentReference` mit dem bloßen Namen `Studienarm` (Quelle `input/fsh/LogicalModel.fsh`, Zeile 100); der Tabellengenerator des IG Publishers kann sie nicht auflösen, die Baumansicht rendert daher derzeit einen Fehler statt einer Tabelle. Bis zur Korrektur (voller Pfad) siehe die [Artefaktseite des Logical Models](StructureDefinition-mii-lm-studie-logicalmodel.md) (Tab „Definitions") für die Elementliste.

Es ist zu beachten, dass das Logical Model rein auf die Abbildung der Datenelemente und deren Beschreibung abzielt. Verwendete Datentypen und Kardinalitäten sind nicht als verpflichtend anzusehen; dies wird abschließend durch die FHIR-Profile festgelegt. Für jedes Element innerhalb des Logical Models existiert ein 1:1-Mapping auf ein Element einer konkreten FHIR-Ressource; die Mapping-Tabellen je Profil sind Teil der jeweiligen Profil-Einleitung (siehe [Profile](profiles.md)).

