BioSamples metadata model
=========================

The BioSamples archive stores metadata about samples, such as collection date, location, and organism type, to aid in their discovery and re-analysis. These samples can be associated with data derived from them, which is deposited in other archives such as ENA. Samples must first be submitted to BioSamples prior to submitting data to ENA.

Samples only have a few mandatory fields:

- sample name
- release date (publication date for the sample)
- organism name
- collection date
- geographic location (country and/or sea).

However, partners should submit rich metadata where possible as this will enable discovery and reuse of registered samples. BioSamples allows submitters to add as many custom metadata attributes as desired.

# Sample Checklists

To ensure that each sample is registered with at least a minimum amount of metadata, ENA provides GSC-based “Sample Checklists”. These provide a set of minimal attributes which you should provide for a given sample. Registering a BioSample with an ENA checklist is a requirement for submitting data using this sample to ENA.

These checklists are developed in collaboration with different research communities to ensure that they are relevant and realistic for their context. Explore the full range of sample checklists here. Note that each checklist provides a set of mandatory values which must always be provided, as well as recommended values which should be provided wherever possible, and optional values which are suggested values not relevant to every case. When registering a sample, it is important to choose the most relevant sample checklist available and provide the most metadata possible.

If you cannot provide a value for a mandatory field within a checklist, please use one of the INDSC accepted terms (https://ena-docs.readthedocs.io/en/latest/submit/samples/missing-values.html) for missing value reporting.


# Sample Relationships in BioSamples

Sample relationships describe the relationship between two biosamples. The relationships can be submission, technical, or biological relationships. It links different samples together and supports relationship-based graph searches.
The sample relationship is submitted to Biosamples by providing the source, type, and target. Below is an example of sample relationships in Biosamples.


When the submitter provides relationship information in one sample, the reverse relationships in corresponding samples will be generated automatically. BioSamples doesn’t validate the type, direction, or the logic of the relationships.
BioSamples currently supports four types of sample relationships

Relationship types
- Reverse relationships
- Description
- derived from
- derived from (reverse)


Sample A is derived from Sample B.



For samples in the same project or study, it is recommended to provide the project or study information as an attribute, rather than providing has member relationships to avoid duplication.