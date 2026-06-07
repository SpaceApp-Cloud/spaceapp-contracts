# Deprecated Contracts

## LaunchEvent.json

Status: Deprecated

Reason:

Superseded by LaunchDetectedEvent.json

LaunchDetectedEvent provides:

- event_id
- event_type
- source
- timestamp
- vehicle
- launch window boundaries
- confidence scoring

All future launch detection workflows should use:

events/LaunchDetectedEvent.json
