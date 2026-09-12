# Community Review Questions

[Open the CIM review form](https://github.com/PhysioVerse-OSE/mps-model-system-descriptors/issues/new?template=cim-proposal-review.yml) · [Proposal overview](README.md)

Review one question at a time with a real use case or source where available.

| Topic | Review question |
|---|---|
| Experimental-unit identity | Should `Chip` be one type of a general experimental-unit or model-instance concept? How would a non-chip organoid be described? |
| Design versus execution | Which properties belong to a reusable model design, and which vary by experimental run, culture, reagent lot, or device? |
| Biological source | What donor, cell-line, differentiation, and batch information is needed without exposing identifying or restricted information? |
| Replication | How should independent biological units, technical repeats, repeated time points, and between-laboratory observations be distinguished? |
| Assays and modalities | Is a scalar `Measurement` sufficient for the initial scope? How should file-based and array-based outputs link to the same experiment? |
| Interventions | Is the first scope limited to compounds? What would be needed to describe non-compound interventions without misleading labels? |
| Timing | What event defines each time origin? How do culture age, exposure-relative time, collection, and assay execution relate? |
| Units and value sets | Which quantities need explicit units or denominators? What are the proposed meanings and allowed values for named status/category types? |
| Provenance | How should a result link to input data, processing activities, software versions, parameters, and responsible agents? |
| Reproducibility assessment | How are `maxCV`, `icc`, scope, and status defined? What endpoint, sample structure, method, uncertainty, and context support an interpretation? |
| Structural rules | Which checks test record structure, and which require scientific review? How should a failed structural check be distinguished from insufficient scientific evidence? |
| Versioning | How should changes to the CIM and mappings be documented while preserving original identifiers and prior interpretations? |

## Suggested Review Submission

State the affected concept, use case, current limitation, proposed revision, supporting source, and expected effect on other concepts. Record disagreements and missing evidence explicitly. Submitting a proposal does not establish community consensus.
