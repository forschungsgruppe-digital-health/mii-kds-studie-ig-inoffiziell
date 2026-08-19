<!-- markdownlint-disable MD041 -->
<!-- TODO:REVIEW machine translation of the German source (Gate C) -->
The module's search parameters are grouped per profile below; the 15 SearchParameter artifacts
themselves are listed in the [artifacts summary](artifacts.html).

### Study (ResearchStudy) — `mii-pr-studie-studie`

The following search parameters are relevant for the Studie module, including in combination:

1. The search parameter "_id" MUST be supported:

    Examples:

    ```GET [base]/ResearchStudy?_id=103270```

    Usage notes: further information on searching by "_id" can be found in the [FHIR base specification - section "Parameters for all resources"](http://hl7.org/fhir/R4/search.html#all).

2. The search parameter "_profile" MUST be supported:

    Examples:

    ```GET [base]/ResearchStudy?_profile=https://www.medizininformatik-initiative.de/fhir/modul-studie/StructureDefinition/mii-pr-studie-studie```

    Usage notes: further information on searching by "_profile" can be found in the [FHIR base specification - section "Parameters for all resources"](http://hl7.org/fhir/R4/search.html#all).

3. The search parameter "identifier" MUST be supported:

    Examples

    ```GET [base]/ResearchStudy?identifier=DRKS00031294```

    Usage notes: further information on searching by "ResearchStudy.identifier" can be found in the [FHIR base specification - section "token"](http://hl7.org/fhir/R4/search.html#token).

4. The search parameter "title" MUST be supported:

    Examples

    ```GET [base]/ResearchStudy?title=Frontale transkranielle Gleichstromstimulation (tDCS) als potentielle Behandlungsmethode von Long-COVID bedingter Fatigue```

    Usage notes: further information on searching by "ResearchStudy.title" can be found in the [FHIR base specification - section "string"](http://hl7.org/fhir/R4/search.html#string).

5. The search parameter "status" MUST be supported:

    Examples

    ```GET [base]/ResearchStudy?status=active```

    Usage notes: further information on searching by "ResearchStudy.status" can be found in the [FHIR base specification - section "token"](http://hl7.org/fhir/R4/search.html#token).

6. The search parameter "partOf" MUST be supported:

    Examples

    ```GET [base]/ResearchStudy?partOf=ResearchStudy/researchstudy-test```

    Usage notes: further information on searching by "ResearchStudy.partOf" can be found in the [FHIR base specification - section "reference"](http://hl7.org/fhir/R4/search.html#reference).

7. The search parameter "category" MUST be supported:

    Examples

    ```GET [base]/ResearchStudy?category=interventional```

    Usage notes: further information on searching by "ResearchStudy.category" can be found in the [FHIR base specification - section "token"](http://hl7.org/fhir/R4/search.html#token).

8. The search parameter "armName" MUST be supported:

    Examples

    ```GET [base]/ResearchStudy?armName=frontale anodale tDCS  (verum condition)```

    Usage notes: further information on searching by "ResearchStudy.arm.name" can be found in the [FHIR base specification - section "string"](http://hl7.org/fhir/R4/search.html#string).

9. The search parameter "category" MUST be supported:

    Examples

    ```GET [base]/ResearchStudy?category=Long-COVID bedingter Fatigue```

    Usage notes: further information on searching by "ResearchStudy.extension:Studienfokus" can be found in the [FHIR base specification - section "string"](http://hl7.org/fhir/R4/search.html#string).

10. The search parameter "keyword" MUST be supported:

    Examples

    ```GET [base]/ResearchStudy?keyword=COVID```

    Usage notes: further information on searching by "ResearchStudy.extension:Schlagwort" can be found in the [FHIR base specification - section "string"](http://hl7.org/fhir/R4/search.html#string).

11. The search parameter "label" MUST be supported:

    Examples

    ```GET [base]/ResearchStudy?label=Frontale transkranielle Gleichstromstimulation (tDCS) als potentielle Behandlungsmethode von Long-COVID bedingter Fatigue```

    Usage notes: further information on searching by "ResearchStudy.extension:Label" can be found in the [FHIR base specification - section "string"](http://hl7.org/fhir/R4/search.html#string).

12. The search parameter "studienregister" MUST be supported:

    Examples

    ```GET [base]/ResearchStudy?studienregister=Library/example```

    Usage notes: further information on searching by "ResearchStudy.extension:Studienregister" can be found in the [FHIR base specification - section "reference"](http://hl7.org/fhir/R4/search.html#reference).      

13. The search parameter "rekrutierungsstand-datum" MUST be supported:

    Examples

    ```GET [base]/ResearchStudy?rekrutierungsstand-datum=2023-02-17```

    Usage notes: further information on searching by "ResearchStudy.extension:Rekrutierung.extension:rekrutierungsstand-datum" can be found in the [FHIR base specification - section "date"](http://hl7.org/fhir/R4/search.html#date).

14. The search parameter "rekrutierungsstand-genauigkeit" MUST be supported:

    Examples

    ```GET [base]/ResearchStudy?rekrutierungsstand-genauigkeit=good```

    Usage notes: further information on searching by "ResearchStudy.extension:Rekrutierung.extension:rekrutierungsstand-genauigkeit" can be found in the [FHIR base specification - section "string"](http://hl7.org/fhir/R4/search.html#string). 

15. The search parameter "rekrutierungsstand-rekrutierungsstand" MUST be supported:

    Examples

    ```GET [base]/ResearchStudy?rekrutierungsstand=35```

    Usage notes: further information on searching by "ResearchStudy.extension:Rekrutierung.extension:rekrutierungsstand" can be found in the [FHIR base specification - section "number"](http://hl7.org/fhir/R4/search.html#number).

16. The search parameter "rekrutierungsstand-rekrutierungsziel" MUST be supported:

    Examples

    ```GET [base]/ResearchStudy?rekrutierungsziel=40```

    Usage notes: further information on searching by "ResearchStudy.extension:Rekrutierung.extension:rekrutierungsziel" can be found in the [FHIR base specification - section "number"](http://hl7.org/fhir/R4/search.html#number).

17. The search parameter "rekrutierungsstand-rekrutierungsstart" MUST be supported:

    Examples

    ```GET [base]/ResearchStudy?rekrutierungsstart=2023-01-12```

    Usage notes: further information on searching by "ResearchStudy.extension:Rekrutierung.extension:rekrutierungsstart" can be found in the [FHIR base specification - section "date"](http://hl7.org/fhir/R4/search.html#date).

### Research subject (ResearchSubject) — `mii-pr-studie-proband`

The following search parameters are relevant for the Medizinisches Forschungsvorhaben module, including in combination:

1. The search parameter "_id" MUST be supported:

    Examples:

    ```GET [base]/ResearchSubject?_id=103270```

    Usage notes: further information on searching by "_id" can be found in the [FHIR base specification - section "Parameters for all resources"](http://hl7.org/fhir/R4/search.html#all).

2. The search parameter "_profile" MUST be supported:

    Examples:

    ```GET [base]/ResearchSubject?_profile=https://www.medizininformatik-initiative.de/fhir/core/modul-person/StructureDefinition/ResearchSubject```

    Usage notes: further information on searching by "_profile" can be found in the [FHIR base specification - section "Parameters for all resources"](http://hl7.org/fhir/R4/search.html#all).

3. The search parameter "identifier" MUST be supported:

    Examples:

    ```GET [base]/ResearchSubject?identifier=http://fhir.krankenhaus.example/sid/subjectIdentificationCode|1032702```

    Usage notes: further information on searching by "ResearchSubject.identifier" can be found in the [FHIR base specification - section "Token Search"](http://hl7.org/fhir/R4/search.html#token).

4. The search parameter "status" MUST be supported:

    Examples:

    ```GET [base]/ResearchSubject?status=candidate```

    Usage notes: further information on searching by "ResearchSubject.status" can be found in the [FHIR base specification - section "Token Search"](http://hl7.org/fhir/R4/search.html#token).


5. The search parameter "date" MUST be supported:

    Examples:

    ```GET [base]/ResearchSubject?date=2022-01-01```

    Usage notes: further information on searching by "ResearchSubject.period" can be found in the [FHIR base specification - section "Date Search"](http://hl7.org/fhir/R4/search.html#date).

6. The search parameter "study" MUST be supported:

    Examples:

    ```GET [base]/ResearchSubject?study=ResearchStudy/study```

    Usage notes: further information on searching by "ResearchStudy.study" can be found in the [FHIR base specification - section "reference"](http://hl7.org/fhir/R4/search.html#reference).

7. The search parameter "individual" MUST be supported:

    Examples:

    ```GET [base]/ResearchSubject?individual=Patient/test```

    Usage notes: further information on searching by "ResearchStudy.individual" can be found in the [FHIR base specification - section "reference"](http://hl7.org/fhir/R4/search.html#reference).

8. The search parameter "consent" MUST be supported:

    Examples:

    ```GET [base]/ResearchSubject?consent=Consent/test```

    Usage notes: further information on searching by "ResearchStudy.consent" can be found in the [FHIR base specification - section "reference"](http://hl7.org/fhir/R4/search.html#reference).

### Register (Library) — `mii-pr-studie-register`

The following search parameters are relevant for the Studie module, including in combination:

1. The search parameter "_id" MUST be supported:

    Examples:

    ```GET [base]/Library?_id=103270```

    Usage notes: further information on searching by "_id" can be found in the [FHIR base specification - section "Parameters for all resources"](http://hl7.org/fhir/R4/search.html#all).

2. The search parameter "_profile" MUST be supported:

    Examples:

    ```GET [base]/Library?_profile=https://www.medizininformatik-initiative.de/fhir/modul-studie/StructureDefinition/mii-pr-studie-register```

    Usage notes: further information on searching by "_profile" can be found in the [FHIR base specification - section "Parameters for all resources"](http://hl7.org/fhir/R4/search.html#all).

3. The search parameter "name" MUST be supported:

    Examples:

    ```GET [base]/Library?name=DRKS - Deutsches Register Klinischer Studien```

    Usage notes: further information on searching by "Library.name" can be found in the [FHIR base specification - section "String Search"](http://hl7.org/fhir/R4/search.html#string).

4. The search parameter "identifier" MUST be supported:

    Examples

    ```GET [base]/Library?identifier=DRKS```

    Usage notes: further information on searching by "Library.identifier" can be found in the [FHIR base specification - section "token"](http://hl7.org/fhir/R4/search.html#token).

5. The search parameter "quellregister" MUST be supported:

    Examples

    ```GET [base]/Library?quellregister=true```

    Usage notes: further information on searching by "Library.extension:QuellRegister" can be found in the [FHIR base specification - section "token"](http://hl7.org/fhir/R4/search.html#token).

6. The search parameter "type" MUST be supported:

    Examples

    ```GET [base]/Library?type=http://terminology.hl7.org/CodeSystem/library-type|asset-collection```

    Usage notes: further information on searching by "Library.type" can be found in the [FHIR base specification - section "token"](http://hl7.org/fhir/R4/search.html#token).

7. The search parameter "relatedArtifactUrl" MUST be supported:

    Examples

    ```GET [base]/Library?relatedArtifactUrl=https://drks.de/```

    Usage notes: further information on searching by "Library.relatedArtifact.document.url" can be found in the [FHIR base specification - section "uri"](http://hl7.org/fhir/R4/search.html#uri).

### Inclusion and exclusion criterion (EvidenceVariable) — `mii-pr-studie-ein-auschluss-kriterium`

The following search parameters are relevant for the Studie module, including in combination:

1. The search parameter "_id" MUST be supported:

    Examples:

    ```GET [base]/ResearchStudy?_id=103270```

    Usage notes: further information on searching by "_id" can be found in the [FHIR base specification - section "Parameters for all resources"](http://hl7.org/fhir/R4/search.html#all).

2. The search parameter "_profile" MUST be supported:

    Examples:

    ```GET [base]/ResearchStudy?_profile=https://www.medizininformatik-initiative.de/fhir/modul-studie/StructureDefinition/mii-pr-studie-ein-auschluss-kriterium```

    Usage notes: further information on searching by "_profile" can be found in the [FHIR base specification - section "Parameters for all resources"](http://hl7.org/fhir/R4/search.html#all).

3. The search parameter "status" MUST be supported:

    Examples

    ```GET [base]/ResearchStudy?status=active```

    Usage notes: further information on searching by "EvidenceVariable.status" can be found in the [FHIR base specification - section "token"](http://hl7.org/fhir/R4/search.html#token).

4. The search parameter "characteristicDescription" MUST be supported:

    Examples

    ```GET [base]/EvidenceVariable?characteristicDescription=Höchstalter```

    Usage notes: further information on searching by "EvidenceVariable.characteristic.description" can be found in the [FHIR base specification - section "string"](http://hl7.org/fhir/R4/search.html#string).

### Study inclusion recommendation (ServiceRequest) — `mii-pr-studie-studieneinschluss-anfrage`

The following search parameters are relevant for the Studie module, including in combination:

1. The search parameter "_id" MUST be supported:

    Examples:

    ```GET [base]/ServiceRequest?_id=12345```

    Usage notes: further information on searching by "_id" can be found in the [FHIR base specification - section "Parameters for all resources"](http://hl7.org/fhir/R4/search.html#all).

2. The search parameter "_profile" MUST be supported:

    Examples:

    ```GET [base]/ServiceRequest?_profile=https://www.medizininformatik-initiative.de/fhir/modul-studie/StructureDefinition/mii-pr-studie-studieneinschluss-anfrage```

    Usage notes: further information on searching by "_profile" can be found in the [FHIR base specification - section "Parameters for all resources"](http://hl7.org/fhir/R4/search.html#all).

3. The search parameter "status" MUST be supported:

    Examples

    ```GET [base]/ServiceRequest?status=active```

    Usage notes: further information on searching by "status" can be found in the [FHIR base specification - section "token"](http://hl7.org/fhir/R4/search.html#token).

4. The search parameter "intent" MUST be supported:

    Examples

    ```GET [base]/ServiceRequest?status=proposal```

    Usage notes: further information on searching by "intent" can be found in the [FHIR base specification - section "string"](http://hl7.org/fhir/R4/search.html#string).

5. The search parameter "category" MUST be supported:

    Examples

    ```GET [base]/ServiceRequest?category=110465008```

    Usage notes: further information on searching by "category" can be found in the [FHIR base specification - section "token"](http://hl7.org/fhir/R4/search.html#token).

6. The search parameter "code" MUST be supported:

    Examples

    ```GET [base]/ServiceRequest?code=02475000```

    Usage notes: further information on searching by "code" can be found in the [FHIR base specification - section "reference"](http://hl7.org/fhir/R4/search.html#token).

7. The search parameter "supporting-info" MUST be supported:

    Examples

    ```GET [base]/ServiceRequest?supporting-info=ResearchStudy/example```

    Usage notes: further information on searching by "supporting-info" can be found in the [FHIR base specification - section "string"](http://hl7.org/fhir/R4/search.html#reference).

### Document / publication (DocumentReference) — `mii-pr-studie-dokument`

The following search parameters are relevant for the Studie module, including in combination:

1. The search parameter "_id" MUST be supported:

    Examples:

    ```GET [base]/DocumentReference?_id=103270```

    Usage notes: further information on searching by "_id" can be found in the [FHIR base specification - section "Parameters for all resources"](http://hl7.org/fhir/R4/search.html#all).

2. The search parameter "_profile" MUST be supported:

    Examples:

    ```GET [base]/DocumentReference?_profile=https://www.medizininformatik-initiative.de/fhir/modul-studie/StructureDefinition/mii-pr-studie-dokument```

    Usage notes: further information on searching by "_profile" can be found in the [FHIR base specification - section "Parameters for all resources"](http://hl7.org/fhir/R4/search.html#all).

3. The search parameter "author" MUST be supported:

    Examples

    ```GET [base]/DocumentReference?author=Practitioner/practitioner-test```

    Usage notes: further information on searching by "DocumentReference.author" can be found in the [FHIR base specification - section "reference"](http://hl7.org/fhir/R4/search.html#reference).


4. The search parameter "custodian" MUST be supported:

    Examples

    ```GET [base]/DocumentReference?custodian=Organization/organization-test```

    Usage notes: further information on searching by "DocumentReference.custodian" can be found in the [FHIR base specification - section "reference"](http://hl7.org/fhir/R4/search.html#reference).

5. The search parameter "status" MUST be supported:

    Examples

    ```GET [base]/DocumentReference?status=current```

    Usage notes: further information on searching by "PractitionerRole.status" can be found in the [FHIR base specification - section "token"](http://hl7.org/fhir/R4/search.html#token).

6. The search parameter "location" MUST be supported:

    Examples

    ```GET [base]/DocumentReference?location=https://example.com/fhir/Binary/document```

    Usage notes: further information on searching by "DocumentReference.content.attachment.url" can be found in the [FHIR base specification - section "uri"](https://www.hl7.org/fhir/r4/search.html#uri).

7. The search parameter "contenttype" MUST be supported:

    Examples

    ```GET [base]/DocumentReference?contenttype=application/pdf```

    Usage notes: further information on searching by "DocumentReference.content.attachment.contentType" can be found in the [FHIR base specification - section "token"](https://www.hl7.org/fhir/r4/search.html#token).

8. The search parameter "title" MUST be supported:

    Examples:

    ```GET [base]/DocumentReference?title=Beispiel Dokument```

    Usage notes: further information on searching by "DocumentReference.content.attachment.title" can be found in the [FHIR base specification - section "String Search"](http://hl7.org/fhir/R4/search.html#string).

9. The search parameter "size" MUST be supported:

    Examples:

    ```GET [base]/DocumentReference?size=1000```

    Usage notes: further information on searching by "DocumentReference.content.attachment.size" can be found in the [FHIR base specification - section "Number Search"](http://hl7.org/fhir/R4/search.html#number).

10. The search parameter "related" MUST be supported:

    Examples:

    ```GET [base]/DocumentReference?related=ResearchStudy/example```

    Usage notes: further information on searching by "DocumentReference.context.related" can be found in the [FHIR base specification - section "reference"](http://hl7.org/fhir/R4/search.html#reference).

### Involved person (PractitionerRole) — `mii-pr-studie-beteiligte-person`

The following search parameters are relevant for the Studie module, including in combination:

1. The search parameter "_id" MUST be supported:

    Examples:

    ```GET [base]/PractitionerRole?_id=103270```

    Usage notes: further information on searching by "_id" can be found in the [FHIR base specification - section "Parameters for all resources"](http://hl7.org/fhir/R4/search.html#all).

2. The search parameter "_profile" MUST be supported:

    Examples:

    ```GET [base]/PractitionerRole?_profile=https://www.medizininformatik-initiative.de/fhir/modul-studie/StructureDefinition/mii-pr-studie-beteiligte-person```

    Usage notes: further information on searching by "_profile" can be found in the [FHIR base specification - section "Parameters for all resources"](http://hl7.org/fhir/R4/search.html#all).

3. The search parameter "practitioner" MUST be supported:

    Examples

    ```GET [base]/PractitionerRole?practitioner=Practitioner/practitioner-test```

    Usage notes: further information on searching by "PractitionerRole.practitioner" can be found in the [FHIR base specification - section "reference"](http://hl7.org/fhir/R4/search.html#reference).

4. The search parameter "organization" MUST be supported:

    Examples

    ```GET [base]/PractitionerRole?organization=Organization/organization-test```

    Usage notes: further information on searching by "PractitionerRole.organization" can be found in the [FHIR base specification - section "reference"](http://hl7.org/fhir/R4/search.html#reference).

5. The search parameter "role" MUST be supported:

    Examples

    ```GET [base]/PractitionerRole?role=http://example.org/fhir/CodeSystem/RolleBeteiligtePerson|studienleiter```

    Usage notes: further information on searching by "PractitionerRole.code" can be found in the [FHIR base specification - section "token"](http://hl7.org/fhir/R4/search.html#token).

6. The search parameter "telecom" MUST be supported:

    Examples

    ```GET [base]/PractitionerRole?telecom=phone|+4915232584956```

    Usage notes: further information on searching by "PractitionerRole.telecom" can be found in the [FHIR base specification - section "reference"](http://hl7.org/fhir/R4/search.html#token).

