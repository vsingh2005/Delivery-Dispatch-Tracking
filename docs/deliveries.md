# Deliveries

Released operations: crud.

Fields and validation rules:

```json
{
  "reference": {
    "type": "TEXT",
    "required": true
  },
  "destination": {
    "type": "TEXT",
    "required": true
  },
  "status": {
    "type": "TEXT",
    "required": true,
    "choices": [
      "pending",
      "assigned",
      "delivered",
      "failed"
    ]
  },
  "weight_kg": {
    "type": "REAL",
    "required": true,
    "min": 0
  }
}
```

API: `/api/deliveries`. CSV import: POST `/api/deliveries/import` with a JSON `csv` field when released. Summary: GET `/api/deliveries/report` when released. Search: GET `/api/deliveries?q=term&limit=50&offset=0` when released. PUT `/api/deliveries/ID` accepts `record` and the last observed `version`; stale updates are rejected.
