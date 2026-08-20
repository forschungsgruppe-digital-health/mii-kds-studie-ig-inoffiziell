# Logical Models - MII Implementation Guide Medizinisches Forschungsvorhaben v2026.0.1

* [**Table of Contents**](toc.md)
* **Logical Models**

## Logical Models

The information model of the Medizinisches Forschungsvorhaben module is represented as a FHIR Logical Model:

> **Known source defect (upstream fix needed):** the Logical Model's element `Studiendesign.Studienarm.Studienarm` declares a `contentReference` by the bare name `Studienarm` (source `input/fsh/LogicalModel.fsh`, line 100); the IG Publisher's table generator cannot resolve it, so the model's tree view currently renders an error instead of a table. Until the reference is corrected upstream to the full path, see the [Logical Model artifact page](StructureDefinition-mii-lm-studie-logicalmodel.md) (Definitions tab) for the element list.

Note that the Logical Model aims purely at representing the data elements and their description. Data types and cardinalities used in it are not to be regarded as mandatory — the FHIR profiles define those conclusively. For every element within the Logical Model there is a 1:1 mapping onto an element of a concrete FHIR resource; the per-profile mapping tables are part of each profile's introduction (see [Profiles](profiles.md)).

