# EvidenceVariable-characteristic-description - MII Implementation Guide Medizinisches Forschungsvorhaben v2026.0.1

* [**Inhaltsverzeichnis**](toc.md)
* [**Artefaktübersicht**](artifacts.md)
* **EvidenceVariable-characteristic-description**

## SearchParameter: EvidenceVariable-characteristic-description 

| | |
| :--- | :--- |
| *Offizielle URL*:https://www.medizininformatik-initiative.de/fhir/modul-studie/SearchParameter/EvidenceVariable-characteristic-description | *Version*:2026.0.1 |
| Active Stand: 2026-08-20 | *Maschinenlesbarer Name*:SP_MII_Studie_CharacteristicDescription |

 
Suchparameter für EvidenceVariable.characteristic.description 



## Resource Content

```json
{
  "resourceType" : "SearchParameter",
  "id" : "EvidenceVariable-characteristic-description",
  "url" : "https://www.medizininformatik-initiative.de/fhir/modul-studie/SearchParameter/EvidenceVariable-characteristic-description",
  "version" : "2026.0.1",
  "name" : "SP_MII_Studie_CharacteristicDescription",
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
  "description" : "Suchparameter für EvidenceVariable.characteristic.description",
  "jurisdiction" : [{
    "coding" : [{
      "system" : "urn:iso:std:iso:3166",
      "code" : "DE",
      "display" : "Germany"
    }]
  }],
  "code" : "characteristicDescription",
  "base" : ["EvidenceVariable"],
  "type" : "string",
  "expression" : "EvidenceVariable.characteristic.description"
}

```
