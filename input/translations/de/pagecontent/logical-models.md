<!-- markdownlint-disable MD041 -->
<!-- Quelle: MIIIGModulStudie @1394b43 (kerndatensatzmodul-studie v2026.0.1) -->
Das Informationsmodell für das Modul Medizinisches Forschungsvorhaben wurde als
FHIR Logical Model abgebildet:

{% lang-fragment StructureDefinition-mii-lm-studie-logicalmodel-snapshot.xhtml %}

Es ist zu beachten, dass das Logical Model rein auf die Abbildung der
Datenelemente und deren Beschreibung abzielt. Verwendete Datentypen und
Kardinalitäten sind nicht als verpflichtend anzusehen; dies wird abschließend
durch die FHIR-Profile festgelegt. Für jedes Element innerhalb des Logical
Models existiert ein 1:1-Mapping auf ein Element einer konkreten
FHIR-Ressource; die Mapping-Tabellen je Profil sind Teil der jeweiligen
Profil-Einleitung (siehe [Profile](profiles.html)).
