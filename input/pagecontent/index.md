<!-- markdownlint-disable MD041 -->
<!-- TODO:REVIEW machine translation of the German source (Gate C) -->
### Introduction

This specification describes the FHIR representation of the Core Dataset (CDS)
extension module **Medizinisches Forschungsvorhaben** (medical research project,
"Studie") of the Medical Informatics Initiative (MII). It covers the module's
use cases and the associated FHIR profiles and terminology resources in their
normative form.

| Publication |               |
|-------------|---------------|
| Date        | 2026-01-09    |
| Version     | 2026.0.1 (CalVer `YYYY.n.n`) |
| Status      | active        |
| Realm       | DE            |

The first release is available at
[2025.0.0](https://www.medizininformatik-initiative.de/Kerndatensatz/KDS_Medizinische_Forschungsvorhaben_V2025/ImplementationGuide-1.x-TechnischeImplementierung-Organization.html).

### Target audience

<div class="ig-highlight ig-highlight-blue">
<h5>Implementers</h5>
<p>Data Integration Centers (DIC), software developers and system architects building FHIR-based solutions.<br/>
→ see <a href="profiles.html">Profiles</a> and <a href="logical-models.html">Logical Models</a>.</p>
</div>

### Contents

- **[Guidance](guidance.html)** — module description and use-case scenarios.
- **Conformance** — the KDS-wide conformance rules (requirements language,
  Must Support, handling missing data) are maintained centrally by the
  [Meta module](https://github.com/medizininformatik-initiative/kerndatensatz-meta/wiki/Conformance);
  the module-specific [Security and Privacy](security-and-privacy.html)
  considerations are part of this guide.
- **[Profiles](profiles.html)** and the further
  **[artifact pages](artifacts.html)** — the technical artifacts.
- **[Examples](examples.html)** — example instances.
- **[Dependencies](ImplementationGuide-mii-ig-studie.html)** — the
  ImplementationGuide resource with the dependency table, cross-version
  analysis and copyright statements.

### Related guides

This module is part of the MII Core Dataset; the other KDS modules and their
dependencies are described at
[medizininformatik-initiative.de](https://www.medizininformatik-initiative.de/de/der-kerndatensatz-der-medizininformatik-initiative).

### Legal notice (Impressum)

This guide was produced within the Medical Informatics Initiative and is, per
its governance process, subject to the ballot procedure of the Technical
Committee of HL7 Deutschland e. V.

### Contact

* Matthias Löbe, Inst. for Medical Informatics (IMISE), University of Leipzig
* Karoline Buckow, TMF – Technologie- und Methodenplattform für die vernetzte
  medizinische Forschung e. V.

Questions about this publication can be raised at any time on
[chat.fhir.org](https://chat.fhir.org/#narrow/stream/179307-german.2Fmi-initiative)
in the stream 'german/mi-initiative'. Comments and criticism are welcome as
issues in the
[GitHub repository](https://github.com/medizininformatik-initiative/kerndatensatzmodul-studie/issues).

### Authors (in alphabetical order)

* Bartow, Martin
* Brix, Tobias
* Gatrio, Margaux
* Gulden, Christian
* Löbe, Matthias
* Macho, Philipp Marten
* Rinaldi, Eugenia
* Scherer, Clemens
* Strauch, Natalia
* Ulbrich, Florian
* Vella, Gustav
* Zautke, Alexander

### Copyright and license

© 2019+ TMF e. V., Charlottenstraße 42, 10117 Berlin. This work is licensed
under the
[Creative Commons Attribution 4.0 International License](https://creativecommons.org/licenses/by/4.0/).

For the usage rights of the underlying FHIR technology, see the FHIR base
specification. Some code systems used are published and maintained by other
organisations; the copyright of the respective publisher applies.

### Disclaimer

The content of this document is public. Note that parts of this document are
based on FHIR version R4, for which the copyright of HL7 International applies.

Although this publication was prepared with the greatest care, the authors
cannot accept any liability for direct or indirect damage arising from the
content of this specification.
