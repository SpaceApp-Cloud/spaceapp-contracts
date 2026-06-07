# SpaceApp Event Metadata Rules

Required fields:

- event_id
- event_version
- timestamp
- source

All events are immutable.

Events are append-only.

No event updates.

New state = new event.

UUIDv4 is recommended for event_id values.
