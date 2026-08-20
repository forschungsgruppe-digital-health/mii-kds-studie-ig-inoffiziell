<!-- markdownlint-disable MD041 -->
<!-- TODO:REVIEW machine translation of the source narrative (de); review at Gate C -->
### Context within the overall project / relations to other modules

**Relation to the PERSON module.** A minimal version of the research subject
was previously represented in the MII PERSON module and moved into the
Medizinisches Forschungsvorhaben module with this release.

**Relation to the CONSENT module.** The CONSENT module describes declarations
of consent by informed patients/subjects as well as policies for enforcing
graded usage variants. It refers to research projects for which such a consent
is to apply.

**Relation to the STRUKTURDATEN module.** The STRUKTURDATEN module (in
preparation) describes organisational structures, sites and individual service
data of organisational units in MII hospitals. The module itself has no direct
relation to research projects but is used by this module. No modelling
conflicts are currently foreseeable.

**Relation to other modules.** The module description characterizing this
module (decision of the AG Interoperabilität of 2021-03-17) mentions
dependencies on further modules. These refer to possible dependencies of
future, content-wise extended versions and are not addressed at present:

1. The present information model does not currently cover the representation
   of individual clinical parameters as collected, for example, in CRFs.
2. The present information model does not currently use extended metadata for
   provenance or quality.

No further dependencies on other modules are known to the team.

### Organization (reused profile)

The Core Dataset already defines the concept "Organisation" in the
STRUKTURDATEN module; that specification is reused by this module and is
**not yet finally balloted**. See the profile
["Profile - MI-I - Organisation - Organization"](https://simplifier.net/guide/modulstruktur-leitfaden-version1.0?version=current)
(draft), canonical
`https://www.medizininformatik-initiative.de/fhir/core/modul-strukturdaten/StructureDefinition/Organization`.
The mapping of the logical data set's contact and site elements onto
Organization is described in the [Profiles](profiles.html) section.

### References

This version was discussed with representatives of the
[Deutsches Forschungsdatenportal Gesundheit](https://forschen-fuer-gesundheit.de/)
(FDPG). The draft was discussed with representatives of the
[Nationale Forschungsdateninfrastruktur für personenbezogene Gesundheitsdaten](https://www.nfdi4health.de/)
(NFDI4Health), and prepared together with representatives from other publicly
funded networks and industry partners; attention was paid to potential
conflicts of interest arising from this.
