# Proof of Concept - Live Coding Interview Tool

## Scope
- App category: Health & Wellness
- Entity model: Live Coding Care Record
- Deployable stack: Flask + SQLAlchemy + Gunicorn + Docker + CI

## Dynamic Field Configuration
- Patient/User: `patient_or_user` (text)
- Wellness Metric: `wellness_metric` (number)
- Care Notes: `care_notes` (textarea)

## Run Evidence Commands
```bash
python app.py
curl http://localhost:5000/api/health
curl http://localhost:5000/api/schema
curl -X POST http://localhost:5000/api/records   -H "Content-Type: application/json"   -d '{"title":"Demo Record","status":"monitoring","payload":{"patient_or_user":"Demo value","wellness_metric":12,"care_notes":"seed note"}}'
curl http://localhost:5000/api/metrics
```

## Metadata
- Idea number: 50
- Generated UTC: 2026-03-24T15:52:22.114771+00:00
- Status: Phase-2 complete
