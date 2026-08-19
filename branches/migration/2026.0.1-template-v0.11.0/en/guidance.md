# Guidance - MII Implementation Guide Medizinisches Forschungsvorhaben v2026.0.1

* [**Table of Contents**](toc.md)
* **Guidance**

## Guidance

### Module description

The MII CDS module Medizinisches Forschungsvorhaben was created as a module of the [Core Dataset (KDS) of the Medical Informatics Initiative (MII)](https://www.medizininformatik-initiative.de/de/der-kerndatensatz-der-medizininformatik-initiative).

Medical research projects in the context of medical informatics are planned experimental clinical and epidemiological investigations that rely on structured data collection, mostly from human subjects. They span a broad range of types with differing degrees of regulatory requirements. Explicitly included in this module are:

* **Clinical trials** serve to demonstrate the superiority and safety of new therapies. They can be interventional as well as observational. A common field of application are drug approval studies, whose conduct is subject to strict legal requirements protecting the trial participants. Clinical trials are characterized by comparatively small subject collectives, a delimited research question, a specific but manageable data catalogue, and a fixed project duration. Many clinical trials divide the study collective into sub-collectives (arms), which may follow different data collection procedures. Clinical trials are frequently conducted at several sites (multicentric). Typical for clinical trials is active data management but a low degree of standardization of individual data elements across studies.
* **Registers** serve the longitudinal investigation of defined disease areas. The legal basis of data collection can vary. The subject collective is often larger than in clinical trials and is observed permanently, frequently until death, which creates specific challenges for tracking subjects (tracking, record linkage). Registers are usually non-interventional and single-arm, mono- or multicentric, with active or minimal data management depending on resources.
* **Cohorts** are investigations of a large number of volunteer subjects intended to represent a cross-section of the target population. Cohorts investigate very broad research questions that are not fully defined at the outset. They are long-term undertakings; unlike registers, the active investigation phase is often limited to one or few time points with a very detailed, comprehensive data catalogue, after which only little information is collected (e.g. vital status, state of health). Cohorts often are monocentric, but large multicentric cohorts exist (e.g. NAKO). Typical for cohorts is a broad data corpus of structured data, images, genomic data, biosamples and more, with instruments, devices and analysis methods changing over the long project duration.
* **Public health / surveillance** projects cover very divergent research questions with and without subject contact, with project-specific data collection or as secondary use of data collected elsewhere. The investigated collectives tend to be larger; a particular feature is a large share of patient surveys as paper-based or electronic questionnaires.
* **Use cases** of the MII are not a special type of medical research: any of the four types above qualifies, as well as free project-specific research based on existing data — consortium-internal and cross-consortium use cases, retrospective analyses, feasibility studies, or projects applying artificial intelligence methods. They are patient-oriented in the sense that tracking of included or includable patients of a site is required, that assignment to responsible organisational units is needed, or that projects follow a structured process description with defined responsibilities — in particular the basic process points of the Deutsches Forschungsdatenportal für Gesundheit (formerly ZARS).

### Use-case scenarios

The module team initially developed a large set of possible scenarios that would influence the shape and scope of the module. To arrive at a first consentable version, the model focuses on the following priorities:

1. Support of the concept of a research study as a structured project, with characteristics for identifying and managing a research project and for representing its basic characterizing features (study register).
1. Support of the concept of a research subject as an identifiable individual, with the basic characterizing features for tracking and findability.
1. Support of the concept of eligibility: the ability to define structured inclusion and exclusion criteria against which it can be decided — at least semi-automatically — whether an individual with its intrinsic properties belongs to the target population.

