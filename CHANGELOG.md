## [0.1.1] - 2026-05-25

### Added

- Added `docs/purity-detection-algorithm.md` to define the draft algorithmic framework for estimating origin purity.
- Added `examples/purity-assessment.sample.yaml` as a sample purity assessment output.
- Added `schemas/purity-assessment.schema.json` for validating purity assessment records.
- Added `.github/workflows/validate-examples.yml` to validate YAML examples against JSON Schemas.
- Added a `Validation` section to `README.md`.

### Changed

- Updated `README.md` Repository Structure to include `purity-assessment.sample.yaml` and `purity-assessment.schema.json`.
- Updated `README.md` Start Here section to include the Purity Detection Algorithm and Purity Assessment Example.
- Expanded the `PurityProtocol` layer from a conceptual protocol component into a documented, example-backed, and CI-validated specification layer.

### Notes

This release strengthens the purity assessment layer of the Epicenter Preservation OS Protocol.

The added purity layer supports:

- natural / synthetic data separation
- hybrid data classification
- recursive synthetic data risk detection
- model collapse monitoring
- reference auditing
- royalty readiness review

This update does not define legal authorship, copyright ownership, or final royalty allocation.  
It provides a review-support and ecosystem-health layer for future protocol development.
