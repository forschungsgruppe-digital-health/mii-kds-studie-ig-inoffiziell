# Library-quellregister - MII Implementation Guide Medizinisches Forschungsvorhaben v2026.0.1

* [**Inhaltsverzeichnis**](toc.md)
* [**Artefaktübersicht**](artifacts.md)
* **Library-quellregister**

## SearchParameter: Library-quellregister 

| | |
| :--- | :--- |
| *Offizielle URL*:https://www.medizininformatik-initiative.de/fhir/modul-studie/SearchParameter/Library-quellregister | *Version*:2026.0.1 |
| Active Stand: 2026-08-20 | *Maschinenlesbarer Name*:SP_MII_Studie_Quellregister |

 
Suchparameter für Library.extension:QuellRegister 



## Resource Content

```json
{
  "resourceType" : "SearchParameter",
  "id" : "Library-quellregister",
  "url" : "https://www.medizininformatik-initiative.de/fhir/modul-studie/SearchParameter/Library-quellregister",
  "version" : "2026.0.1",
  "name" : "SP_MII_Studie_Quellregister",
  "status" : "active",
  "experimental" : false,
  "date" : "2026-08-20T10:04:57+00:00",
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
  "description" : "Suchparameter für Library.extension:QuellRegister",
  "jurisdiction" : [{
    "coding" : [{
      "system" : "urn:iso:std:iso:3166",
      "code" : "DE",
      "display" : "Germany"
    }]
  }],
  "code" : "quellregister",
  "base" : ["Library"],
  "type" : "token",
  "expression" : "Library.extension.where(url='https://www.medizininformatik-initiative.de/fhir/modul-studie/StructureDefinition/mii-ex-studie-quell-register').value"
}

```
