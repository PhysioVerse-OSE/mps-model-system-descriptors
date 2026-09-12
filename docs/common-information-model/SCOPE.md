# Scope and Use Cases

[Proposal overview](README.md) · [Review questions](REVIEW_QUESTIONS.md)

**Proposed initial scope. Community review is needed before adoption.**

## Starting Boundary

Begin with a study that compares MPS experimental units under defined conditions and reports numerical assay measurements. Use the original class diagram as the review artifact. Do not assume that it already describes every model architecture, intervention, file type, or study design.

## Questions to Test Against Real Studies

| Use case | Questions to answer | Evidence to retain |
|---|---|---|
| Identify what was studied | Which model design, device or culture instance, cell source, and protocol were used? | Original study and model identifiers, reported versions, publication and protocol locations |
| Interpret a numerical measurement | What was measured, on which unit, with which assay, unit, and time reference? | Endpoint definition, measurement value, units, assay context, original sample or device ID |
| Compare treatment groups | How are treatments and independent experimental units assigned to groups? | Group definitions, controls, reported dose and duration, replicate structure |
| Trace a reported result | Which raw observations and processing steps support the result? | Source files or accessions, protocol execution, processing description, software and version when reported |
| Evaluate reproducibility evidence | Which units, runs, batches, or laboratories support the assessment? | Assessment method, scope, sample structure, endpoint, uncertainty, limitations, and evidence source |

For each case, document what the diagram captures, what requires a proposed extension, and what cannot be determined from the source study.

## Extension Questions

Review a general experimental-unit concept for non-chip systems; donor, cell-line, and batch identity; sampled material; protocol execution; file and dataset references; longitudinal observations; non-compound interventions; and explicit provenance relationships. These are proposed review topics, not silently added classes.

## Outside This Initial Proposal

The initial diagram does not define a production database migration, a complete API, implemented validation software, universal acceptance thresholds, or a regulatory decision process. It also does not establish a single ranking across different MPS uses.

## Record a Scope Decision

For each proposed inclusion or exclusion, record the use case, rationale, affected classes, source evidence, unresolved questions, and the Issue or pull request where the decision is reviewed.
