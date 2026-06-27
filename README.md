# Research Agent

Evidence-first research workflow for Web3 financial infrastructure, on-chain data, and DeFi risk analysis.

## Status

Active rebuild. This repository began as an experimental workflow using research-agent components and prompt-based research tasks. It is being refactored into a small, reproducible research tool during summer 2026.

The first target is not a general news summarizer. It is a research workflow that helps users collect evidence, separate facts from interpretations, compare conflicting sources, and produce citation-linked research notes.

## Problem

Web3 research often combines protocol documentation, governance discussions, on-chain activity, market data, incident reports, and secondary research. These sources differ in authority, timing, and reliability.

This project aims to make that process more explicit:

* store sources with metadata and retrieval time
* distinguish source-backed facts, interpretations, and hypotheses
* surface conflicting claims and missing evidence
* connect research notes to their supporting sources
* preserve a reviewable trail instead of producing unsupported summaries

## Initial Use Case

The first use case is incident and risk analysis for Web3 financial infrastructure.

Example questions:

* What verification assumption failed in a bridge or oracle incident?
* Which lending markets could receive the affected asset as collateral?
* What on-chain evidence supports a claimed risk-transmission path?
* Which parts of a conclusion are observed facts, and which remain hypotheses?

The KelpDAO rsETH / LayerZero incident is the initial reference case.

## Scope

### Included

* Public-source collection and metadata storage
* Source classification by type and reliability
* Claim, evidence, and uncertainty records
* Citation-linked research notes
* Human review before final conclusions
* Read-only analysis of public data and documents

### Excluded

* Autonomous trading decisions
* Order execution
* Wallet signing or private-key handling
* Automatic publication without review
* Unsupported investment recommendations

## Summer 2026 Roadmap

### Phase 1 — Foundation

* Define source, claim, evidence, and research-note schemas
* Build a CLI workflow for one research question
* Store retrieved sources and run logs locally
* Add tests for schemas and citation integrity

### Phase 2 — Web3 Research MVP

* Add adapters for protocol docs, governance forums, news, and selected on-chain data sources
* Generate structured evidence tables
* Produce a citation-linked markdown research note
* Test the workflow with the KelpDAO rsETH incident case

### Phase 3 — Evaluation and Documentation

* Create a small benchmark set of research questions
* Measure citation coverage, unsupported-claim rate, and source conflicts surfaced
* Publish architecture notes, known limitations, and example runs
* Track work through public GitHub issues and milestones

## Development Principles

* Small working MVPs before multi-agent orchestration
* Human review for analytical conclusions
* Explicit separation between fact, interpretation, and hypothesis
* Read-only permissions by default
* Reproducible logs and source provenance
* No direct connection between research output and trading execution

## License

MIT License. Add the LICENSE file before the first public release.
