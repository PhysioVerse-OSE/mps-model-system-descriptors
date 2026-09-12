# Concept Inventory of the Initial Diagram

[Proposal overview](README.md) · [Original diagram](mps-cim-original.png)

This inventory transcribes the class and attribute names visible in the initial diagram. Names and types are retained as supplied; the inventory does not establish required fields, finalized definitions, or executable validation rules. Relationship direction and multiplicity remain in the original diagram for review.

| Area | Class | Attributes and types shown |
|---|---|---|
| Model | `MPSModel` | `name: String`; `organTerm: CURIE`; `version: String` |
| Model | `DevicePlatform` | `manufacturer: String`; `model: String`; `material: Material`; `format: String` |
| Model | `CellPopulation` | `cellTypeTerm: CURIE`; `supplier: String`; `lotNumber: String`; `passage: Integer`; `seedingDensity: Decimal` |
| Model | `Medium` | `name: String`; `supplier: String`; `supplements: String` |
| Model | `Chamber` | `name: String`; `volume_uL: Decimal`; `flowRate_uL_h: Decimal` |
| Study | `Study` | `id: UUID`; `title: String`; `status: StudyStatus`; `startDate: Date`; `cimVersion: String` |
| Study | `Protocol` | `id: UUID`; `name: String`; `version: String`; `documentUri: URI` |
| Study | `TreatmentGroup` | `name: String`; `description: String` |
| Study | `Chip` | `chipId: String`; `label: String` |
| Study | `Treatment` | `concentration: Decimal`; `unit: UCUMCode`; `vehicle: String`; `startTime: Duration`; `duration: Duration` |
| Study | `Compound` | `name: String`; `chebiTerm: CURIE`; `casNumber: String`; `supplier: String`; `lotNumber: String`; `cLogP: Decimal` |
| Measurement | `Measurement` | `timepoint: Duration`; `value: Decimal`; `unit: UCUMCode`; `qualityFlag: String` |
| Measurement | `Assay` | `name: String`; `targetAnalyte: CURIE`; `method: String`; `kit: String`; `category: ReadoutCategory` |
| Analysis | `ReproducibilityAssessment` | `scope: ReproScope`; `maxCV: Decimal`; `icc: Decimal`; `status: ReproStatus` |

The diagram names `Material`, `StudyStatus`, `ReadoutCategory`, `ReproScope`, and `ReproStatus` but does not display their value sets. It also does not specify every quantity's unit or every timing origin. These details remain review questions; no values or definitions are inferred here.
