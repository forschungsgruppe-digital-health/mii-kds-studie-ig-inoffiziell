<!-- markdownlint-disable MD041 -->
<!-- Quelle: MIIIGModulStudie @1394b43 (kerndatensatzmodul-studie v2026.0.1) -->
Um eine dezentrale Datenauswertung mittels des Deutschen
Forschungsdatenportals für Gesundheit der Medizininformatik-Initiative zu
ermöglichen, MUSS die
[capabilities-Interaktion](https://www.hl7.org/fhir/http.html#capabilities)
unterstützt werden, sodass durch den FHIR-Server unter `[BASE_URL]/metadata`
ein CapabilityStatement exponiert wird. Innerhalb dieses CapabilityStatements
MUSS angegeben werden, welche Profile inkl. Version sowie welche Suchparameter
unterstützt werden.

Darüber hinaus MUSS eine Konformität zu dem CapabilityStatement des Moduls in
der jeweiligen CapabilityStatement-Instanz unter
[`CapabilityStatement.instantiates`](https://www.hl7.org/fhir/capabilitystatement-definitions.html#CapabilityStatement.instantiates)
angegeben werden.

Canonical:
`https://www.medizininformatik-initiative.de/fhir/modul-studie/CapabilityStatement/metadata`

{% lang-fragment CapabilityStatement-MII-CPS-Metadata-Studie-html.xhtml %}
