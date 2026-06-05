# SpaceApp Event Compatibility Matrix

## Purpose

This document defines compatibility requirements
between event producers and consumers.

---

# Compatibility Rules

## Minor Version Updates

Minor versions are backward compatible.

Examples:

1.0 -> 1.1
1.1 -> 1.2

Consumers should continue processing events.

---

## Major Version Updates

Major versions may introduce breaking changes.

Examples:

1.0 -> 2.0

Consumers must be upgraded before processing.

---

# MissionEvent

| Producer | Consumer | Status |
|-----------|-----------|---------|
| 1.0 | 1.0 | Supported |
| 1.1 | 1.0 | Supported |
| 2.0 | 1.0 | Upgrade Required |

---

# TelemetryEvent

| Producer | Consumer | Status |
|-----------|-----------|---------|
| 1.0 | 1.0 | Supported |
| 1.1 | 1.0 | Supported |
| 2.0 | 1.0 | Upgrade Required |

---

# TrajectoryEvent

| Producer | Consumer | Status |
|-----------|-----------|---------|
| 1.0 | 1.0 | Supported |
| 1.1 | 1.0 | Supported |
| 2.0 | 1.0 | Upgrade Required |

---

# LaunchEvent

| Producer | Consumer | Status |
|-----------|-----------|---------|
| 1.0 | 1.0 | Supported |
| 1.1 | 1.0 | Supported |
| 2.0 | 1.0 | Upgrade Required |

---

# BatchEvent

| Producer | Consumer | Status |
|-----------|-----------|---------|
| 1.0 | 1.0 | Supported |
| 1.1 | 1.0 | Supported |
| 2.0 | 1.0 | Upgrade Required |

---

# Governance

Reference Documents:

- VERSION.md
- REPLAY.md
- CONTRACT_REGISTRY.md

Compatibility decisions require:

1. Contract review
2. Consumer impact review
3. Version approval
4. Documentation update
