# Agent Instructions

These instructions apply to future coding agents working in this repository.

## Before Editing

- Inspect the repository before making changes.
- Check `git status` and avoid overwriting user work.
- Read relevant files before editing them.
- Keep changes small, scoped, and reviewable.

## Research Integrity

- Do not fabricate research claims, sources, citations, metrics, users, or benchmark results.
- Preserve provenance and uncertainty in research materials.
- Separate facts, interpretations, hypotheses, and open questions.
- Do not present simulations, assumptions, or stress-test ideas as historical facts.
- Surface conflicting claims instead of hiding them.

## Security and Configuration

- Do not read or modify `.env` files.
- Do not add API keys, tokens, default passwords, or other secrets.
- Use empty placeholders in examples and explain that users must supply local values.
- Never commit real secrets.

## Submodules

- Do not touch git submodules unless explicitly instructed.
- Do not rewrite or vendor submodule contents as part of ordinary repository cleanup.
- Treat existing submodule changes as user-owned unless the user asks otherwise.

## Tooling

- Run formatting or tests only when corresponding tooling exists in the repository.
- Do not add dependencies, package managers, Docker files, CI workflows, databases, or service integrations unless the task explicitly requires them.

## Git

- Never commit or push without explicit instruction.
- Do not create pull requests, releases, or GitHub issues unless explicitly instructed.
