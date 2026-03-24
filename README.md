# Live Coding Interview Tool

## Solution Summary
Production-ready domain application.

This Phase-2 implementation is a domain-ready, deployable web application for **Health & Wellness** workflows.

## Core Capabilities
- Responsive dashboard with KPI cards and recent activity table
- Domain record lifecycle with full CRUD (web + API)
- Dynamic schema fields tailored to this use case
- Status pipeline: `intake, monitoring, follow-up, completed`
- Docker + Gunicorn deployment assets, CI checks, and Pytest tests

## Domain Model
- Primary entity: **Live Coding Care Record**
- Collection: **Live Coding Care Records**
- Dynamic fields:
- Patient/User (`patient_or_user` / text)
- Wellness Metric (`wellness_metric` / number)
- Care Notes (`care_notes` / textarea)

## Operational Workflow
1. Capture intake
2. Track indicators
3. Review trends
4. Close care cycle

## API
- `GET /api/health`
- `GET /api/schema`
- `GET /api/records`
- `POST /api/records`
- `GET /api/metrics`

## Run Locally
```bash
python3 -m venv .venv
source .venv/bin/activate
pip install -r requirements.txt
python app.py
```

## Docker Run
```bash
docker compose up --build
```

## Proof of Concept
- [proof-of-concept.md](proof-of-concept.md)
- [proof/demo-output.txt](proof/demo-output.txt)
- [proof/ui-preview.svg](proof/ui-preview.svg)
