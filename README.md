# research-agent

`research-agent` is an early-stage, evidence-first research workflow for Web3 financial infrastructure and DeFi risk analysis.

## Current Status

This repository is an active rebuild. It is not production-ready, does not yet provide a working research agent, and should not be treated as an autonomous analysis, trading, or execution system.

The current repository contains:

- project documentation for the intended direction
- a legacy KelpDAO prompt used as prior research context
- external submodules that are preserved for reference
- an environment example that documents local configuration placeholders

It does not yet prove automated data collection, benchmark results, production usage, or end-to-end agent capabilities for this project.

## Problem Statement

Web3 incident and risk research often mixes facts, assumptions, interpretations, market narratives, and incomplete data. For DeFi protocols, bridges, restaking assets, lending markets, and oracle-dependent systems, this makes it hard to reproduce a research note or understand which claims are actually supported by evidence.

This project aims to make that workflow more disciplined. The target workflow should help researchers collect sources, preserve provenance, identify conflicting claims, separate observed facts from analysis, and produce citation-linked notes that are easier for humans to review.

## Initial Use Case

The initial use case is Web3 incident and risk analysis. The first reference case is the KelpDAO rsETH / LayerZero incident context, especially how cross-chain asset assumptions, bridge messaging, liquidity, lending markets, and liquidation mechanics can interact during a stressed event.

The repository should eventually help a researcher ask questions such as:

- What happened, according to primary and secondary sources?
- Which claims are directly supported by cited evidence?
- Which claims conflict across sources?
- What facts are still missing or uncertain?
- What interpretations depend on assumptions rather than observed records?
- What downstream risk channels should be analyzed before drawing conclusions?
- How should a research note preserve source links, timestamps, and uncertainty?

## Project Scope

Included scope:

- read-only research workflows by default
- source collection planning
- source metadata and provenance tracking
- claim, evidence, and uncertainty classification
- separation of facts, interpretations, and hypotheses
- surfacing conflicting claims
- citation-linked research notes
- human review and reproducibility
- local-first schemas and CLI workflow design

Excluded scope:

- autonomous trading
- order execution
- wallet signing, transaction signing, or private-key handling
- portfolio management
- market-making or liquidation bots
- systems that directly turn research output into trading decisions
- production data pipelines before the project scope is validated
- dashboards, API servers, databases, scrapers, or multi-agent orchestration before the technical stack is chosen

## Facts, Interpretations, and Hypotheses

Research output should clearly label the status of each claim:

- Facts: claims supported by cited evidence, such as transaction records, protocol documentation, official incident statements, governance posts, or archived public data.
- Interpretations: analytical conclusions drawn from facts, with assumptions and reasoning stated explicitly.
- Hypotheses: plausible explanations or risk scenarios that require more verification before they are treated as findings.

The workflow should make uncertainty visible instead of smoothing it away.

## Reference Case: KelpDAO rsETH / LayerZero

The initial reference case is the KelpDAO rsETH / LayerZero incident context. It is useful because it touches several research surfaces at once:

- cross-chain asset representation and bridge messaging
- liquid staking and restaking asset assumptions
- lending-market collateral behavior
- liquidity and oracle-risk questions
- downstream effects on DeFi integrations

The repository includes a legacy prompt at `prompts/kelp_rsETH_aave_composability.txt`. That file is preserved as historical working material, not as verified project output. See `examples/kelpdao/README.md` for a cleaner reference-case framing.

## Summer 2026 Roadmap

### Phase 1: Schemas and Local CLI Workflow

- define minimal schemas for sources, claims, evidence, uncertainty, and notes
- design a local read-only CLI workflow
- create fixtures for the KelpDAO reference case
- document how provenance should be recorded
- avoid adding external services until the data model is stable

### Phase 2: Web3 Research MVP

- implement a small local workflow that turns curated source inputs into structured research notes
- support manual source entry and citation tracking
- separate facts, interpretations, hypotheses, and unresolved questions
- add checks for missing citations and unsupported claims
- keep the MVP read-only and human-reviewed

### Phase 3: Evaluation, Documentation, and Reproducible Example

- create a reproducible KelpDAO reference example
- document expected inputs and outputs
- add lightweight evaluation criteria for citation quality, uncertainty labeling, and reproducibility
- improve contributor documentation
- prepare a small `v0.1.0` release once the workflow is demonstrable

## Development Principles

- Evidence comes first; analysis must point back to sources.
- Provenance should be preserved at every step.
- Claims should be labeled by confidence and evidence type.
- Conflicting claims should be surfaced rather than hidden.
- The default workflow should be read-only.
- Humans should review outputs before publication or downstream use.
- The project should avoid overstating maturity or capability.
- Technical choices should stay small until the research model is clear.

## Contributing

Issues, questions, and feedback are welcome. Good early contributions include improving documentation, proposing schemas, identifying reproducibility gaps, and suggesting careful reference cases. Please avoid adding production infrastructure or broad agent architecture before the project scope and technical stack are finalized.
