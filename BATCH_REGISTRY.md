# SpaceApp Batch Registry

## Purpose

The Batch Registry tracks all batch processing jobs
within the SpaceApp platform.

Examples:

- Replay jobs
- Historical backfills
- Analytics processing
- Data imports
- Schema migrations
- Launch correlation processing

---

## Batch States

REGISTERED

RUNNING

COMPLETED

FAILED

CANCELLED

---

## Batch Types

REPLAY

BACKFILL

ANALYTICS

IMPORT

MIGRATION

CORRELATION

---

## Event Contract

BatchRegistryEvent.json

Schema:

schemas/BatchRegistryEvent.schema.json

Current Version:

1.0
