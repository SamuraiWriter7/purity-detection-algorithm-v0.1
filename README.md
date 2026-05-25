# Epicenter Preservation OS Protocol v0.1

**Status:** Draft v0.1.1  
**Version:** 0.1.1  
**Release Date:** 2026-05-25

Epicenter Preservation OS Protocol is a draft specification for preserving primary sources, reference traces, value circulation, and model-collapse monitoring in AI civilization.

This protocol defines a minimal structure for identifying and preserving **Epicenters** — primary sources of thought, expression, observation, practice, and structural invention — while making AI reference events, purity signals, and royalty-readiness review more traceable.

The goal is not to prohibit AI-assisted creation.

The goal is to preserve the source ecology of AI civilization.

---

## Concept

AI systems increasingly depend on human-created sources:

- articles
- books
- notes
- logs
- datasets
- talks
- protocols
- structural concepts
- firsthand observations

However, when AI systems consume, summarize, rewrite, and recursively reuse these sources, the original Epicenter can become difficult to identify.

This creates several risks:

- primary sources become invisible
- reference events are not recorded
- creators are not credited or compensated
- synthetic data begins to replace natural data
- model-collapse risk increases
- AI civilization loses source diversity

Epicenter Preservation OS Protocol proposes a minimal structure for addressing these risks.

```text
Epicenter
↓
ReferenceEvent
↓
TraceProtocol
↓
PurityProtocol
↓
CollapseMonitor
↓
RoyaltyProtocol / Allocation Review
```

---

## Core Idea

The protocol separates five layers:

1. **Epicenter Layer**  
   Identifies the original source unit.

2. **Reference Layer**  
   Records when an AI system references or uses an Epicenter.

3. **Purity Layer**  
   Estimates the origin composition of a source, including natural, synthetic, hybrid, or recursive synthetic signals.

4. **Collapse Monitoring Layer**  
   Observes ecosystem-level risks caused by declining natural-data ratios or recursive synthetic reuse.

5. **Royalty / Value Circulation Layer**  
   Provides a path toward auditable value return, without directly automating final allocation decisions.

---

## Design Principles

### 1. Preserve the Source

AI civilization depends on primary sources.

If the source layer collapses, downstream AI systems become increasingly shallow, repetitive, and derivative.

### 2. Trace Before Allocation

Reference events must be recorded before any royalty or compensation logic is applied.

```text
No trace
↓
No reliable allocation
```

### 3. Purity Is Not Moral Judgment

Origin purity is not a measure of artistic value, legal authorship, or human worth.

It is an ecological signal for understanding data composition.

```text
Purity ≠ Value
Purity ≠ Copyright
Purity ≠ Authorship
Purity = estimated origin composition
```

### 4. AI-Assisted Creation Is Not Invalid

The protocol does not reject AI-assisted work.

Instead, it distinguishes:

- human-origin sources
- AI-assisted sources
- hybrid sources
- synthetic sources
- recursively generated sources

### 5. Review Before Royalty

Purity scores and trace records should support review.

They should not automatically determine legal ownership or final payment.

---

## Repository Structure

```text
.
├── README.md
├── LICENSE
├── CHANGELOG.md
├── CITATION.cff
├── spec/
│   └── epicenter-preservation-os-v0.1.yaml
├── schemas/
│   ├── epicenter-preservation-os.schema.json
│   └── purity-assessment.schema.json
├── docs/
│   └── purity-detection-algorithm.md
├── examples/
│   ├── epicenter.sample.yaml
│   ├── reference-event.sample.yaml
│   ├── royalty-record.sample.yaml
│   ├── model-profile.sample.yaml
│   └── purity-assessment.sample.yaml
└── .github/
    └── workflows/
        └── validate-examples.yml
```

---

## Key Documents

### `spec/epicenter-preservation-os-v0.1.yaml`

Defines the core entities and protocol layers of the Epicenter Preservation OS, including:

- `Epicenter`
- `ReferenceEvent`
- `RoyaltyRecord`
- `ModelProfile`
- `TraceProtocol`
- `RoyaltyProtocol`
- `PurityProtocol`
- `CollapseMonitor`

---

### `docs/purity-detection-algorithm.md`

Defines the draft algorithmic framework for estimating:

- `origin_purity_score`
- `ai_generated_ratio`
- `warning_flags`

This document supports:

- natural / synthetic data separation
- hybrid data classification
- recursive synthetic data risk detection
- model-collapse monitoring
- reference auditing
- royalty-readiness review

---

### `schemas/epicenter-preservation-os.schema.json`

Provides a simplified machine-readable schema for validating the main protocol objects.

---

### `schemas/purity-assessment.schema.json`

Provides a machine-readable validation schema for purity assessment records, including:

- signal scores
- confidence values
- warning flags
- review status
- downstream-use permissions

---

### `examples/`

Contains sample objects for:

- Epicenter registration
- AI reference logging
- royalty records
- model profiles
- purity assessment results

---

## Start Here

The recommended reading order is:

### 1. Core Protocol

Start with:

```text
spec/epicenter-preservation-os-v0.1.yaml
```

This file defines the main structure of the protocol.

It introduces the core entities:

- `Epicenter`
- `ReferenceEvent`
- `RoyaltyRecord`
- `ModelProfile`

And the core protocol layers:

- `TraceProtocol`
- `RoyaltyProtocol`
- `PurityProtocol`
- `CollapseMonitor`

---

### 2. Purity Detection Algorithm

Then read:

```text
docs/purity-detection-algorithm.md
```

This document explains how the system may estimate the origin purity of an Epicenter.

It defines:

- natural data
- synthetic data
- hybrid data
- recursive synthetic data
- `origin_purity_score`
- `ai_generated_ratio`
- `warning_flags`
- human / multi-wing review triggers

This layer is especially important because the protocol does not treat AI-assisted creation as invalid.

Instead, it separates ecological data-quality signals from legal authorship, copyright ownership, or final compensation decisions.

---

### 3. Purity Assessment Example

Review:

```text
examples/purity-assessment.sample.yaml
```

This file shows how a purity assessment result may be represented in practice.

It includes:

- input signal scores
- score basis notes
- `origin_purity_score`
- `ai_generated_ratio`
- `warning_flags`
- review status
- downstream-use decisions

---

### 4. Schema Layer

Review:

```text
schemas/epicenter-preservation-os.schema.json
schemas/purity-assessment.schema.json
```

These files provide machine-readable validation structures for the core protocol objects and purity assessment outputs.

---

### 5. Example Objects

Finally, review the remaining sample files in:

```text
examples/
```

These examples show how Epicenters, reference events, royalty records, model profiles, and purity assessment results may be represented in practice.

---

## Validation

This repository includes a GitHub Actions workflow for validating example files against their corresponding JSON Schemas.

The validation workflow is defined in:

```text
.github/workflows/validate-examples.yml
```

Current validation targets:

```text
examples/purity-assessment.sample.yaml
↓
schemas/purity-assessment.schema.json
```

The workflow checks that the sample purity assessment object conforms to the schema definition, including:

- required fields
- score ranges from `0.0` to `1.0`
- allowed `method` values
- allowed `warning_flags`
- review status structure
- downstream-use permission structure
- ISO 8601 date-time format for `assessed_at`

This validation layer supports the `PurityProtocol` defined in the core protocol by ensuring that `origin_purity_score`, `ai_generated_ratio`, and `warning_flags` can be represented in a machine-readable and testable format.

To run the validation automatically, push changes to the `main` branch or open a pull request.

The workflow can also be triggered manually from the GitHub Actions tab.

### Local Validation Concept

The GitHub Actions workflow uses:

```text
Python 3.12
jsonschema
PyYAML
```

The validation process is:

```text
Load YAML example
↓
Load JSON Schema
↓
Validate example against schema
↓
Report pass / fail
```

If validation fails, the workflow prints the failing field path and the corresponding schema error.

This makes the protocol easier to maintain as the specification evolves.

---

## Core Entities

### Epicenter

An Epicenter is a primary source unit.

It may represent:

- an article
- a note
- a book
- a talk
- a log
- a dataset
- a protocol
- a structural concept

Example fields include:

- `id`
- `type`
- `source_platform`
- `author_id`
- `created_at`
- `updated_at`
- `language`
- `tags`
- `structure_fingerprint`
- `origin_purity_score`
- `ai_generated_ratio`
- `metadata`

---

### ReferenceEvent

A ReferenceEvent records when an AI system references, uses, retrieves, trains on, or reasons from an Epicenter.

Example fields include:

- `id`
- `model_id`
- `epicenter_id`
- `timestamp`
- `context_window_hash`
- `usage_type`
- `request_id`
- `trace_id`
- `weight`

Supported usage types may include:

- `training`
- `inference`
- `rag`
- `fine_tune`

---

### RoyaltyRecord

A RoyaltyRecord represents a possible value-circulation record derived from reference activity.

Example fields include:

- `id`
- `epicenter_id`
- `creator_id`
- `total_reference_weight`
- `amount`
- `period`
- `settlement_status`
- `settlement_channel`

This object does not automatically prove legal payment entitlement.

It represents a candidate accounting layer for future review and settlement.

---

### ModelProfile

A ModelProfile describes model-side purity and source-dependency characteristics.

Example fields include:

- `id`
- `provider`
- `type`
- `training_data_purity`
- `collapse_risk_score`
- `epicenter_dependency_index`

This object helps monitor whether AI systems remain connected to diverse primary sources or drift toward recursive synthetic dependency.

---

## Protocol Layers

### TraceProtocol

Defines the minimum requirements for recording reference events.

Required fields include:

- `ReferenceEvent.id`
- `ReferenceEvent.epicenter_id`
- `ReferenceEvent.model_id`
- `ReferenceEvent.timestamp`
- `ReferenceEvent.usage_type`
- `ReferenceEvent.trace_id`

Expected guarantees include:

- immutability
- auditability
- creator accessibility
- regulator accessibility

---

### PurityProtocol

Defines how the protocol may estimate the origin composition of an Epicenter.

Input signals may include:

- `ai_generated_ratio`
- structure-fingerprint similarity to known AI patterns
- author self-declaration
- provenance evidence
- revision lineage
- citation transparency
- structural originality

Outputs may include:

- `origin_purity_score`
- `ai_generated_ratio`
- `warning_flags`

The detailed algorithm is defined in:

```text
docs/purity-detection-algorithm.md
```

---

### CollapseMonitor

Defines how ecosystem-level risk may be monitored.

Inputs may include:

- model training-data purity
- synthetic-data ratio
- natural-data ratio
- reference statistics
- collapse-risk score
- Epicenter production decline

Possible alerts include:

- `natural_data_ratio_below_threshold`
- `epicenter_production_decline`
- `model_collapse_risk_high`

---

### RoyaltyProtocol

Defines an abstract structure for aggregating reference weight into possible value-circulation records.

A draft formula may look like:

```text
Σ(ReferenceEvent.weight.value) × rate_table[usage_type]
```

Possible modifiers include:

- `origin_purity_score`
- `ai_generated_ratio`
- review status
- dispute status
- platform policy
- creator permission

RoyaltyProtocol is intentionally abstract in v0.1.1.

It should not be treated as a final legal or financial settlement mechanism.

---

## Example Flow

```text
1. A creator publishes an original article.
   ↓
2. The article is registered as an Epicenter.
   ↓
3. The Epicenter receives a structure fingerprint and metadata.
   ↓
4. An AI system references the Epicenter through RAG or inference.
   ↓
5. A ReferenceEvent is logged.
   ↓
6. A purity assessment estimates origin composition.
   ↓
7. CollapseMonitor uses aggregated purity signals.
   ↓
8. RoyaltyProtocol may prepare candidate value-circulation records.
   ↓
9. Human / multi-wing review determines readiness.
```

---

## Non-Goals

This repository does not attempt to:

- define final copyright ownership
- prove legal authorship
- automatically determine payment
- ban AI-assisted creation
- classify all AI-generated content as low value
- replace human review
- provide a production-ready payment system
- define universal originality
- make moral judgments about creators or content

This protocol is a draft structural layer for traceability, review, and ecosystem-health monitoring.

---

## Relationship to Other Concepts

Epicenter Preservation OS Protocol may relate to:

- Trace Protocol
- Structure Fingerprint
- Royalty OS
- Allocation Readiness
- Model Collapse monitoring
- RAG provenance
- AI data governance
- creator compensation systems
- natural / synthetic data separation
- AI reference auditing

---

## Version History

See:

```text
CHANGELOG.md
```

Current version:

```text
0.1.1
```

### v0.1.1

Adds the PurityProtocol implementation layer:

- purity detection algorithm document
- purity assessment sample
- purity assessment JSON Schema
- GitHub Actions validation workflow
- README validation documentation

### v0.1.0

Initial draft protocol.

Defined the core entities and high-level protocol layers:

- `Epicenter`
- `ReferenceEvent`
- `RoyaltyRecord`
- `ModelProfile`
- `TraceProtocol`
- `RoyaltyProtocol`
- `PurityProtocol`
- `CollapseMonitor`

---

## Citation

If you use this specification, please cite it using:

```text
CITATION.cff
```

---

## License

This repository is released under the license defined in:

```text
LICENSE
```

---

## Summary

Epicenter Preservation OS Protocol v0.1.1 defines a draft structure for preserving primary sources in AI civilization.

It connects:

```text
source preservation
↓
reference tracing
↓
purity assessment
↓
collapse monitoring
↓
value-circulation readiness
```

The protocol does not claim to solve legal authorship or compensation automatically.

Instead, it provides a machine-readable foundation for preserving the source layer that AI civilization depends on.

In short:

```text
If AI civilization is a river,
Epicenters are the springs.
This protocol is a first draft of the water-source registry.
```
