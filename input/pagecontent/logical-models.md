<!-- markdownlint-disable MD041 -->
<!-- TODO:REVIEW machine translation of the German source (Gate C) -->
The information model of the Medizinisches Forschungsvorhaben module is
represented as a FHIR Logical Model:

{% lang-fragment StructureDefinition-mii-lm-studie-logicalmodel-snapshot.xhtml %}

Note that the Logical Model aims purely at representing the data elements and
their description. Data types and cardinalities used in it are not to be
regarded as mandatory — the FHIR profiles define those conclusively. For every
element within the Logical Model there is a 1:1 mapping onto an element of a
concrete FHIR resource; the per-profile mapping tables are part of each
profile's introduction (see [Profiles](profiles.html)).
