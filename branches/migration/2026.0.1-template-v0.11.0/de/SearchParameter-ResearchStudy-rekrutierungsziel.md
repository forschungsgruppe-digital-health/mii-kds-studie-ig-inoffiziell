# ResearchStudy-rekrutierungsziel - MII Implementation Guide Medizinisches Forschungsvorhaben v2026.0.1

* [**Inhaltsverzeichnis**](toc.md)
* [**Artefaktübersicht**](artifacts.md)
* **ResearchStudy-rekrutierungsziel**

## SearchParameter: ResearchStudy-rekrutierungsziel 

| | |
| :--- | :--- |
| *Offizielle URL*:https://www.medizininformatik-initiative.de/fhir/modul-studie/SearchParameter/ResearchStudy-rekrutierungsziel | *Version*:2026.0.1 |
| Active Stand: 2026-08-20 | *Maschinenlesbarer Name*:SP_MII_Studie_Rekrutierungsziel |

 
Suchparameter für ResearchStudy.extension:Rekrutierung.extension:rekrutierungsziel 



## Resource Content

```json
{
  "resourceType" : "SearchParameter",
  "id" : "ResearchStudy-rekrutierungsziel",
  "url" : "https://www.medizininformatik-initiative.de/fhir/modul-studie/SearchParameter/ResearchStudy-rekrutierungsziel",
  "version" : "2026.0.1",
  "name" : "SP_MII_Studie_Rekrutierungsziel",
  "status" : "active",
  "experimental" : false,
  "date" : "2026-08-20T09:40:04+00:00",
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
  "description" : "Suchparameter für ResearchStudy.extension:Rekrutierung.extension:rekrutierungsziel",
  "jurisdiction" : [{
    "coding" : [{
      "system" : "urn:iso:std:iso:3166",
      "code" : "DE",
      "display" : "Germany"
    }]
  }],
  "code" : "rekrutierungsziel",
  "base" : ["ResearchStudy"],
  "type" : "number",
  "expression" : "ResearchStudy.extension.where(url='https://www.medizininformatik-initiative.de/fhir/modul-studie/StructureDefinition/mii-ex-studie-rekrutierung').extension.where(url='rekrutierungsziel').value"
}

```
