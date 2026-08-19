# Library-relatedArtifactUrl - MII Implementation Guide Medizinisches Forschungsvorhaben v2026.0.1

* [**Inhaltsverzeichnis**](toc.md)
* [**Artefaktübersicht**](artifacts.md)
* **Library-relatedArtifactUrl**

## SearchParameter: Library-relatedArtifactUrl 

| | |
| :--- | :--- |
| *Offizielle URL*:https://www.medizininformatik-initiative.de/fhir/modul-studie/SearchParameter/Library-relatedArtifactUrl | *Version*:2026.0.1 |
| Active Stand: 2026-08-19 | *Maschinenlesbarer Name*:SP_MII_Studie_RelatedArtifactUrl |

 
Suchparameter für Library.relatedArtifact.document.url 



## Resource Content

```json
{
  "resourceType" : "SearchParameter",
  "id" : "Library-relatedArtifactUrl",
  "url" : "https://www.medizininformatik-initiative.de/fhir/modul-studie/SearchParameter/Library-relatedArtifactUrl",
  "version" : "2026.0.1",
  "name" : "SP_MII_Studie_RelatedArtifactUrl",
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
  "description" : "Suchparameter für Library.relatedArtifact.document.url",
  "jurisdiction" : [{
    "coding" : [{
      "system" : "urn:iso:std:iso:3166",
      "code" : "DE",
      "display" : "Germany"
    }]
  }],
  "code" : "relatedArtifactUrl",
  "base" : ["Library"],
  "type" : "uri",
  "expression" : "Library.relatedArtifact.document.url"
}

```
