# DocumentReference-title - MII Implementation Guide Medizinisches Forschungsvorhaben v2026.0.1

* [**Inhaltsverzeichnis**](toc.md)
* [**Artefaktübersicht**](artifacts.md)
* **DocumentReference-title**

## SearchParameter: DocumentReference-title 

| | |
| :--- | :--- |
| *Offizielle URL*:https://www.medizininformatik-initiative.de/fhir/modul-studie/SearchParameter/DocumentReference-title | *Version*:2026.0.1 |
| Active Stand: 2026-08-19 | *Maschinenlesbarer Name*:SP_MII_Studie_Title |

 
Suchparameter für DocumentReference.content.attachment.title 



## Resource Content

```json
{
  "resourceType" : "SearchParameter",
  "id" : "DocumentReference-title",
  "url" : "https://www.medizininformatik-initiative.de/fhir/modul-studie/SearchParameter/DocumentReference-title",
  "version" : "2026.0.1",
  "name" : "SP_MII_Studie_Title",
  "status" : "active",
  "experimental" : false,
  "date" : "2026-08-19T21:13:29+00:00",
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
  "description" : "Suchparameter für DocumentReference.content.attachment.title",
  "jurisdiction" : [{
    "coding" : [{
      "system" : "urn:iso:std:iso:3166",
      "code" : "DE",
      "display" : "Germany"
    }]
  }],
  "code" : "title",
  "base" : ["DocumentReference"],
  "type" : "string",
  "expression" : "DocumentReference.content.attachment.title"
}

```
