# Enterprise Model Selection Board

![Demo Screenshot](demo/screenshot.png)

## Overview

Rank candidate models across cost, latency, safety, and task performance for enterprise deployment committees.

## Real-world problem

- User: Platform leads and enterprise architecture teams
- Problem: Teams compare models ad hoc without a shared view of cost, safety, and task-fit tradeoffs.
- Decision improved: Choose the right model for deployment by balancing benchmark quality against operating constraints.
- KPI target: Improve model selection speed and reduce deployment rework.

## Why this matters

This repo is positioned as a real product for a real team, not a framework-only demo. The goal is to show how research-backed AI, analytics, or graph systems become deployable workflows with docs, UI, screenshots, and business-facing outputs.

## Project profile

- Domain: AI Procurement and Benchmarking
- Project type: `llm`
- Tags: benchmarking, procurement, llm, enterprise

## Workflow

1. Ingest the operational context for the user and case.
2. Score risk, quality, or opportunity using the project API.
3. Compare current signals against a business baseline.
4. Generate a recommendation or operator brief for the next step.

## Quick start

```bash
python -m venv .venv
source .venv/bin/activate
pip install -r requirements.txt
python scripts/bootstrap_data.py
uvicorn src.app.main:app --host 0.0.0.0 --port 8000 --reload
```

Open `http://localhost:8000/` to use the interactive application.

## Key endpoints

- `GET /`
- `GET /health`
- `GET /bootstrap`
- `GET /project`
- `POST /score`
- `POST /analyze`
- `POST /query`
- `POST /recommend`

## Documentation

- [Architecture](docs/architecture.md)
- [Evaluation](docs/evaluation.md)
- [Runbook](docs/runbook.md)
- [Innovation memo](research/innovation_memo.md)
- [Upstream audit](research/upstream_audit.md)
