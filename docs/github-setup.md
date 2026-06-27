# GitHub Setup Guide

This guide lists recommended GitHub metadata for the repository. It does not create issues, milestones, releases, or repository settings.

## Repository Description

Evidence-first research workflow for Web3 financial infrastructure and DeFi risk analysis.

## Suggested Topics

- web3
- defi
- onchain-analysis
- risk-analysis
- research-tools
- provenance
- citations
- incident-analysis
- reproducibility
- open-source

## Initial Issue Ideas

1. Define source metadata schema
   - Propose the minimum fields needed to track source title, URL or path, access date, publication date, source type, and reliability notes.

2. Define claim and evidence schema
   - Draft a small schema for factual claims, interpretations, hypotheses, citations, confidence, and uncertainty.

3. Create KelpDAO reference-case fixture
   - Convert the KelpDAO rsETH / LayerZero reference case into a small curated fixture without treating hypotheses as facts.

4. Design local read-only CLI workflow
   - Sketch the minimal commands needed to validate local research notes and citation coverage.

5. Add unsupported-claim checks
   - Define lightweight checks that identify factual claims without citations or with unclear source provenance.

6. Draft reproducible research-note template
   - Create a template that separates observed facts, interpretations, hypotheses, conflicting claims, and open questions.

## Suggested Milestones

- Phase 1: Schemas and Local Workflow
- Phase 2: Web3 Research MVP
- Phase 3: Reproducible Example and v0.1.0

## First Release Target

Suggested first release target: `v0.1.0`

The release should wait until the repository has a demonstrable local workflow, clear schemas, and one reproducible example. It should not claim production readiness.
