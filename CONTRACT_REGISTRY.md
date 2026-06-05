# SpaceApp Contract Registry

## Purpose

This registry defines all canonical event contracts
used throughout the SpaceApp platform.

---

## MissionEvent

Version:
1.0

Schema:

schemas/MissionEvent.schema.json

Contract:

MissionEvent.json

Purpose:

Mission lifecycle events.

---

## TelemetryEvent

Version:
1.0

Schema:

schemas/TelemetryEvent.schema.json

Contract:

TelemetryEvent.json

Purpose:

Vehicle telemetry reporting.

---

## TrajectoryEvent

Version:
1.0

Schema:

schemas/TrajectoryEvent.schema.json

Contract:

TrajectoryEvent.json

Purpose:

Trajectory processing.

---

## LaunchEvent

Version:
1.0

Schema:

schemas/LaunchEvent.schema.json

Contract:

LaunchEvent.json

Purpose:

Launch detection and launch status.

---

## BatchEvent

Version:
1.0

Schema:

schemas/BatchEvent.schema.json

Contract:

BatchEvent.json

Purpose:

Batch processing and replay operations.

---

## Governance

Versioning Rules:
VERSION.md

Replay Rules:
REPLAY.md

Validation:
.github/workflows/validate-contracts.yml
