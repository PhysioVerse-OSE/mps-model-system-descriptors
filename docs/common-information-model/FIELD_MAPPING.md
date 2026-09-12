# Field and Concept Mapping

[Proposal overview](README.md) · [PhysioVerse metadata guide](https://physioverse.org/contributor-metadata)

**Candidate alignment worksheet. No equivalence or implementation is asserted.**

Compare each CIM concept with the metadata already in use and relevant external definitions. Preserve current source identifiers and field names until an explicit mapping is reviewed. A shared label does not prove that two concepts have the same meaning.

## Alignment Questions

| CIM concept | Candidate alignment area | Question for review |
|---|---|---|
| `Study` and `Protocol` | Existing study records and the ISA study/process structure | How are study identity, protocol definitions, and actual protocol executions distinguished? |
| `MPSModel` and `Chip` | PhysioVerse model descriptors and experimental-unit identity | Which fields describe a design and which describe a particular culture, device, or sample? |
| `CellPopulation` | Biological-source metadata and permitted donor or cell-line descriptors | Where are source, differentiation, batch, and replicate relationships recorded? |
| `Treatment` and `Compound` | Experimental-condition and intervention descriptors | How are units, exposure route, time origin, and interventions other than compounds represented? |
| `Assay` and `Measurement` | Assay/endpoint terminology and ISA assay/data relationships | What identifies the endpoint, method, measured unit, data object, and observation time? |
| Proposed dataset/file relationships | Multimodal linkage guidance and source manifests | How are numerical readouts, images, omics matrices, videos, and sensor traces connected? |
| Proposed processing/provenance relationships | W3C PROV-O entity, activity, and agent concepts | How can a derived result be traced to its inputs and documented transformations? |
| `ReproducibilityAssessment` | Source-supported validation and reproducibility evidence | What scope, independent units, endpoint, method, and uncertainty support the assessment? |

## One Mapping Record

| Item | Information to provide |
|---|---|
| CIM class and attribute or relationship | Exact source name |
| Source definition and version | Link and relevant location |
| Existing PhysioVerse field or concept | Exact field or descriptor, not an assumed match |
| External standard or vocabulary | Identifier, version, and source link |
| Proposed relationship | Exact, broader, narrower, related, or unresolved, with rationale |
| Unit, value-set, or identifier conversion | Rule and source, if a conversion is proposed |
| Information lost or not represented | Explicit limitations |
| Evidence and open questions | Public examples and unresolved differences |
| Review outcome | Issue or pull request and recorded decision |

## Background Specifications

[ISA Abstract Model](https://isa-specs.readthedocs.io/en/latest/isamodel.html) and [W3C PROV-O](https://www.w3.org/TR/prov-o/) provide concepts to evaluate. Mapping to either resource requires a reviewed definition, not just a matching name. The [FAIR principles](https://doi.org/10.1038/sdata.2016.18) guide reuse but do not prescribe this specific CIM.
