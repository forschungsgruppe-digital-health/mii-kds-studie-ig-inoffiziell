# Profiles - MII Implementation Guide Medizinisches Forschungsvorhaben v2026.0.1

* [**Table of Contents**](toc.md)
* **Profiles**

## Profiles

The Core Dataset specifications build, where possible, on international standards and terminologies — notably the [International Patient Summary](http://hl7.org/fhir/uv/ips/history.html). Adaptation to the general conditions of the German health-care system is achieved through the [German base profiles](https://ig.fhir.de/basisprofile-de/stable/Home.html) of HL7 Deutschland.

All elements of the Core Dataset, adapted to the details and requirements of the MII use cases, are described as FHIR StructureDefinitions. The rationale for each profile is explained in its introduction, directly on the artifact page:

| | |
| :--- | :--- |
| [Studie](StructureDefinition-mii-pr-studie-studie.md) | ResearchStudy |
| [Proband:in](StructureDefinition-mii-pr-studie-proband.md) | ResearchSubject |
| [Register](StructureDefinition-mii-pr-studie-register.md) | Library |
| [Ein- und Ausschlusskriterium](StructureDefinition-mii-pr-studie-ein-auschluss-kriterium.md) | EvidenceVariable |
| [Studieneinschlussempfehlung](StructureDefinition-mii-pr-studie-studieneinschluss-anfrage.md) | ServiceRequest |
| [Dokument](StructureDefinition-mii-pr-studie-dokument.md) | DocumentReference |
| [Beteiligte Person](StructureDefinition-mii-pr-studie-beteiligte-person.md) | PractitionerRole |

The **Organization** concept is reused from the STRUKTURDATEN module (see [Guidance for Implementers](implementer-guidance.md)).

**Mandatory / must-support elements:** for mandatory or must-support-marked elements, the corresponding [IPS rules](http://hl7.org/fhir/uv/ips/STU1/design.html#must-support) apply to this implementation guide as well.

