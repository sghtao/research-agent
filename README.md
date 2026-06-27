# Research Agent

An early-stage, evidence-first research workflow for Web3 financial infrastructure, on-chain data, and DeFi risk analysis.

## Status

This repository is an active rebuild. It is not a production-ready agent and does not yet provide automated data collection or completed research workflows.

The project is being developed as a reproducible research tool that helps organize sources, preserve provenance, distinguish evidence from interpretation, and support human-reviewed research notes.

## Problem

Web3 research often combines protocol documentation, governance discussions, on-chain data, incident reports, market data, and secondary research. These sources differ in authority, timing, and reliability.

This project aims to make the research process more explicit by separating:

* observed facts
* interpretations
* analytical hypotheses
* open questions requiring further verification

## Initial Use Case

The first use case is incident and risk analysis for Web3 financial infrastructure.

The KelpDAO rsETH / LayerZero incident is used as an initial reference case for designing the workflow. It is not treated as a fully automated or complete implementation.

Example questions include:

* What verification premise failed in a bridge or oracle incident?
* Which claims are directly supported by on-chain or primary-source evidence?
* Which lending markets could receive an affected asset as collateral?
* What evidence supports or contradicts a proposed risk-transmission path?
* Which parts of an analysis remain hypotheses rather than observed facts?

## Intended Workflow

```text
Research question
→ source collection
→ source metadata and provenance
→ claim / evidence / uncertainty classification
→ human review
→ citation-linked research note
```

## Scope

### Included

* Source metadata and provenance tracking
* Classification of facts, interpretations, hypotheses, and uncertainty
* Citation-linked research notes
* Human review before conclusions
* Read-only analysis of public documents and public data
* Reproducible research logs and examples

### Excluded

* Autonomous trading
* Order execution
* Wallet signing
* Transaction signing
* Private-key handling
* Direct trading instructions
* Automated market actions
* Any direct connection between research output and trading execution

## Summer 2026 Roadmap

### Phase 1 — Foundation

* Define schemas for sources, claims, evidence, and uncertainty
* Build a small local CLI workflow for one research question
* Store source metadata and execution logs
* Add basic validation for citation integrity

### Phase 2 — Web3 Research MVP

* Support selected protocol documentation, governance discussions, news, and on-chain data inputs
* Generate structured evidence tables
* Produce citation-linked markdown research notes
* Test the workflow with the KelpDAO reference case

### Phase 3 — Evaluation and Documentation

* Create a small set of reproducible research questions
* Define evaluation criteria for citation coverage and unsupported claims
* Publish architecture notes, limitations, and example runs
* Prepare a small reproducible v0.1.0 example

## Development Principles

* Build small working MVPs before adding complexity
* Preserve source provenance and uncertainty
* Keep analytical conclusions reviewable by humans
* Do not present hypotheses as facts
* Keep the system read-only by default
* Do not connect research outputs directly to trading execution

## Contributing

This is an early-stage project. Feedback on research workflow design, provenance tracking, evidence classification, and reproducibility is welcome through issues and discussions.
