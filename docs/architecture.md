# Target Architecture

This document describes the intended high-level workflow for `research-agent`. It is a target architecture, not a description of a currently implemented system.

The project is currently an early-stage rebuild. The future architecture should stay small, read-only by default, and oriented around human review.

## Workflow

### 1. Research Question

A user starts with a scoped research question, such as:

- What claims are supported by evidence in a Web3 incident report?
- Which protocol integrations may be affected by a specific asset or bridge event?
- Which assumptions need verification before publishing a risk note?

The question should be narrow enough to support source collection and reproducible review.

### 2. Source Collection

The workflow should collect or accept sources relevant to the question. Early versions should prioritize manually supplied sources and local fixtures over automated scraping.

Potential source types include:

- protocol documentation
- governance posts
- official incident statements
- transaction or contract references
- public dashboards or exported data
- credible third-party analysis
- archived pages or snapshots

### 3. Source Metadata and Provenance

Each source should preserve metadata that helps another researcher understand where a claim came from.

Useful metadata may include:

- source title
- URL or local path
- publisher or author when available
- access date
- publication date when available
- source type
- relevant excerpts or anchors
- notes about reliability or limitations

### 4. Claim, Evidence, and Uncertainty Classification

The workflow should classify research material into:

- facts supported by cited evidence
- interpretations derived from cited evidence
- hypotheses that require additional verification
- unresolved questions
- conflicting claims across sources

Uncertainty should be represented explicitly. Unsupported claims should remain draft notes until evidence is added or the claim is removed.

### 5. Human Review

Human review is a required part of the intended workflow. The tool should help organize evidence and uncertainty, not replace judgment.

Review should check:

- whether every factual claim has a citation
- whether interpretations state assumptions
- whether hypotheses are clearly marked
- whether source limitations are visible
- whether conflicting claims are documented
- whether the final note avoids unsupported conclusions

### 6. Citation-Linked Research Note

The final artifact should be a research note that links claims back to their sources. It should distinguish facts, interpretations, hypotheses, and open questions.

The note should be reproducible enough that another researcher can follow the source trail and understand how conclusions were reached.

## Non-Goals

The target architecture is not an autonomous trading system. It should not execute orders, perform wallet signing, perform transaction signing, handle private keys, produce direct trading instructions, or convert research outputs into automated market actions.
