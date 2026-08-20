# ResearchStudy-armName - MII Implementation Guide Medizinisches Forschungsvorhaben v2026.0.1

* [**Inhaltsverzeichnis**](toc.md)
* [**Artefaktübersicht**](artifacts.md)
* **ResearchStudy-armName**

## SearchParameter: ResearchStudy-armName 

| | |
| :--- | :--- |
| *Offizielle URL*:https://www.medizininformatik-initiative.de/fhir/modul-studie/SearchParameter/ResearchStudy-armName | *Version*:2026.0.1 |
| Active Stand: 2026-08-20 | *Maschinenlesbarer Name*:SP_MII_Studie_ArmName |

 
Suchparameter für ResearchStudy.arm.name 



## Resource Content

```json
{
  "resourceType" : "SearchParameter",
  "id" : "ResearchStudy-armName",
  "url" : "https://www.medizininformatik-initiative.de/fhir/modul-studie/SearchParameter/ResearchStudy-armName",
  "version" : "2026.0.1",
  "name" : "SP_MII_Studie_ArmName",
  "status" : "active",
  "experimental" : false,
  "date" : "2026-08-20T09:52:29+00:00",
  "publisher" : "NUM-DIZ",
  "_publisher" : {
    "extension" : [{
      "extension" : [{
        "url" : "lang",
        "valueCode" : "de"
      },
      {
        "url" : "content",
        "valueString" : "NUM-DIZ"
      }],
      "url" : "http://hl7.org/fhir/StructureDefinition/translation"
    }]
  },
  "contact" : [{
    "name" : "NUM-DIZ",
    "telecom" : [{
      "system" : "url",
      "value" : "https://www.netzwerk-universitaetsmedizin.de"
    }]
  }],
  "description" : "Suchparameter für ResearchStudy.arm.name",
  "jurisdiction" : [{
    "coding" : [{
      "system" : "urn:iso:std:iso:3166",
      "code" : "DE",
      "display" : "Germany"
    }]
  }],
  "code" : "armName",
  "base" : ["ResearchStudy"],
  "type" : "string",
  "expression" : "ResearchStudy.arm.name"
}

```
