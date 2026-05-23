# IT News Archive

IT/AI/technology news collection, dedupe metadata, generated summaries, and publishing logs.

This repository is intentionally initialized as a lightweight archive target for the n8n/Hermes content automation MVP. Runtime credentials and paid/external delivery configuration stay outside this repo.

## Intended flow

1. n8n or deterministic scripts collect candidate items.
2. Deduplication/state checks run before any LLM call.
3. Hermes handles summaries, rewriting, tone, quality checks, and compliance only for new items.
4. Final artifacts and processing logs are committed here for traceability.

## Directory layout

- `sources/`: source definitions or exported feed lists, no secrets.
- `raw/`: raw collected item snapshots when useful.
- `processed/`: normalized/deduplicated records.
- `outputs/`: generated summaries, drafts, or publish-ready artifacts.
- `logs/`: lightweight processing logs or run manifests.

## Initial topic scope

- AI/LLM
- software
- cloud/devops
- security
- startup/product

## Configuration

No live credentials are committed. Use `.env.example` as a placeholder contract if repo-specific settings are needed later.
