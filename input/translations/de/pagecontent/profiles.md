<!-- markdownlint-disable MD041 -->
<!-- Quelle: MIIIGModulStudie @1394b43 (kerndatensatzmodul-studie v2026.0.1) -->
Die Arbeiten der Kerndatensatzspezifikationen basieren, wo möglich, auf
internationalen Standards und Terminologien — insbesondere der
[International Patient Summary](http://hl7.org/fhir/uv/ips/history.html). Eine
Anpassung an die allgemeinen Gegebenheiten des deutschen Gesundheitswesens
erfolgt durch die Verwendung der
[Deutschen Basisprofile](https://ig.fhir.de/basisprofile-de/stable/Home.html)
von HL7 Deutschland.

Alle Elemente des Kerndatensatzes, angepasst an die Details und Anforderungen
für die Use Cases der Medizininformatik-Initiative, werden in Form von FHIR
StructureDefinitions beschrieben. Die Notwendigkeit der Anpassung wird je
Profil in dessen Einleitung direkt auf der Artefaktseite erläutert:

| Profil | FHIR-Ressource |
| --- | --- |
| [Studie](StructureDefinition-mii-pr-studie-studie.html) | ResearchStudy |
| [Proband:in](StructureDefinition-mii-pr-studie-proband.html) | ResearchSubject |
| [Register](StructureDefinition-mii-pr-studie-register.html) | Library |
| [Ein- und Ausschlusskriterium](StructureDefinition-mii-pr-studie-ein-auschluss-kriterium.html) | EvidenceVariable |
| [Studieneinschlussempfehlung](StructureDefinition-mii-pr-studie-studieneinschluss-anfrage.html) | ServiceRequest |
| [Dokument](StructureDefinition-mii-pr-studie-dokument.html) | DocumentReference |
| [Beteiligte Person](StructureDefinition-mii-pr-studie-beteiligte-person.html) | PractitionerRole |

Das Konzept **Organisation** wird aus dem Modul STRUKTURDATEN wiederverwendet
(siehe [Anleitung für Implementierende](implementer-guidance.html)).

**Verpflichtende / must-support Elemente:** Für verpflichtende oder als
must-support markierte Elemente gelten die entsprechenden
[Regeln der IPS](http://hl7.org/fhir/uv/ips/STU1/design.html#must-support) auch
für diesen ImplementationGuide.
