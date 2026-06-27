# Roadmap

This roadmap covers the intended summer 2026 rebuild. Scope should stay small until the research model, schemas, and review workflow are clear.

## Phase 1: Schemas and Local CLI Workflow

Goal: define the basic research objects and a local workflow before adding integrations.

Milestones:

- define source metadata fields
- define claim, evidence, uncertainty, and note schemas
- document the difference between facts, interpretations, hypotheses, and open questions
- create a small local fixture for the KelpDAO rsETH / LayerZero reference case
- sketch a read-only CLI flow for validating local research notes
- add basic documentation for provenance expectations

Out of scope:

- live web collection
- external databases
- hosted APIs
- dashboards
- autonomous agents

## Phase 2: Web3 Research MVP

Goal: demonstrate a small, human-reviewed workflow for Web3 incident and risk analysis.

Milestones:

- accept manually curated source inputs
- produce a structured draft research note
- flag missing citations for factual claims
- preserve source metadata in outputs
- surface unresolved questions and conflicting claims
- keep all actions read-only by default

Out of scope:

- order execution
- trading recommendations
- automated financial decisions
- broad multi-agent orchestration
- production ingestion pipelines

## Phase 3: Evaluation, Documentation, and Reproducible Example

Goal: make the initial workflow easier to review, reproduce, and improve.

Milestones:

- publish a reproducible KelpDAO reference example
- document setup and expected inputs
- define lightweight evaluation criteria for citation quality and uncertainty labeling
- add contributor guidance for new reference cases
- prepare a small `v0.1.0` release target when the workflow is demonstrable

Out of scope:

- claims of production readiness
- benchmark claims that are not produced by this repository
- new infrastructure unrelated to the reference workflow
