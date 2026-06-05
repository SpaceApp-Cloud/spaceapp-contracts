# SpaceApp Mission Data Contract Versioning Rules

## Purpose

This document defines versioning requirements for all
Mission Data Contracts, Event Schemas, and API payloads.

---

## Version Format

Version format:

MAJOR.MINOR

Examples:

1.0
1.1
2.0

---

## Minor Version Changes

Increment MINOR version when changes are backward compatible.

Examples:

- Adding optional fields
- Adding new event types
- Adding metadata fields
- Extending enumerations

Examples:

1.0 → 1.1
1.1 → 1.2

Consumers must continue functioning without modification.

---

## Major Version Changes

Increment MAJOR version when changes are not backward compatible.

Examples:

- Renaming fields
- Removing fields
- Changing field data types
- Modifying required fields
- Changing event semantics

Examples:

1.0 → 2.0
2.0 → 3.0

Consumers may require updates before processing.

---

## Consumer Requirements

All event consumers must:

- Support the current version
- Support previous minor versions
- Ignore unknown fields
- Validate event_version before processing

Example:

Consumer supports:

1.0
1.1
1.2

Consumer rejects:

2.0

until upgraded.

---

## Producer Requirements

All event producers must:

- Publish the latest contract version
- Include event_version in every event
- Maintain schema compliance
- Publish valid timestamps

Example:

{
  "event_version": "1.1",
  "event_type": "MISSION_CREATED"
}

---

## Replay Compatibility

Historical event replay must preserve:

- Original event_version
- Original event payload
- Original timestamps

Replayed events must never be rewritten.

---

## Deprecation Policy

Deprecated fields:

- Must remain available for one minor version
- Must be documented
- Must include migration guidance

Example:

1.1 = field deprecated

1.2 = field still supported

2.0 = field removed

---

## Contract Governance

Changes to event contracts require:

1. Schema review
2. Version review
3. Consumer impact assessment
4. Documentation update

before deployment.

---

## Current Contract Version

MissionEvent Schema:
1.0

TelemetryEvent Schema:
1.0

MissionSummary Schema:
1.0
