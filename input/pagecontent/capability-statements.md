<!-- markdownlint-disable MD041 -->
<!-- TODO:REVIEW machine translation of the German source (Gate C) -->
To enable decentralized data analysis via the Deutsches Forschungsdatenportal
für Gesundheit of the MII, the
[capabilities interaction](https://www.hl7.org/fhir/http.html#capabilities)
MUST be supported, so that the FHIR server exposes a CapabilityStatement at
`[BASE_URL]/metadata`. Within this CapabilityStatement it MUST be stated which
profiles (including version) and which search parameters are supported.

Conformance to the module's CapabilityStatement MUST additionally be declared
in the respective CapabilityStatement instance via
[`CapabilityStatement.instantiates`](https://www.hl7.org/fhir/capabilitystatement-definitions.html#CapabilityStatement.instantiates).

Canonical:
`https://www.medizininformatik-initiative.de/fhir/modul-studie/CapabilityStatement/metadata`

{% lang-fragment CapabilityStatement-MII-CPS-Metadata-Studie.xhtml %}
