<!-- markdownlint-disable MD041 -->
<!-- TODO:REVIEW machine translation of the German source (Gate C) -->
The Core Dataset specifications build, where possible, on international
standards and terminologies — notably the
[International Patient Summary](http://hl7.org/fhir/uv/ips/history.html).
Adaptation to the general conditions of the German health-care system is
achieved through the
[German base profiles](https://ig.fhir.de/basisprofile-de/stable/Home.html) of
HL7 Deutschland.

All elements of the Core Dataset, adapted to the details and requirements of
the MII use cases, are described as FHIR StructureDefinitions. The rationale
for each profile is explained in its introduction, directly on the artifact
page:

| Profile | FHIR resource |
| --- | --- |
| [Studie](StructureDefinition-mii-pr-studie-studie.html) | ResearchStudy |
| [Proband:in](StructureDefinition-mii-pr-studie-proband.html) | ResearchSubject |
| [Register](StructureDefinition-mii-pr-studie-register.html) | Library |
| [Ein- und Ausschlusskriterium](StructureDefinition-mii-pr-studie-ein-auschluss-kriterium.html) | EvidenceVariable |
| [Studieneinschlussempfehlung](StructureDefinition-mii-pr-studie-studieneinschluss-anfrage.html) | ServiceRequest |
| [Dokument](StructureDefinition-mii-pr-studie-dokument.html) | DocumentReference |
| [Beteiligte Person](StructureDefinition-mii-pr-studie-beteiligte-person.html) | PractitionerRole |

The **Organization** concept is reused from the STRUKTURDATEN module (see
[Guidance for Implementers](implementer-guidance.html)).

**Mandatory / must-support elements:** for mandatory or must-support-marked
elements, the corresponding
[IPS rules](http://hl7.org/fhir/uv/ips/STU1/design.html#must-support) apply to
this implementation guide as well.
