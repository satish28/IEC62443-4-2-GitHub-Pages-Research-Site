---
layout: default
title: FR6 — Timely Response
---

# FR6 — Timely Response to Events

## What Happens When Something Goes Wrong?

Security controls are incomplete if meaningful security events disappear without detection or response.

### RELAY-001 event scenarios

- authentication failures
- unauthorized commands
- invalid messages
- repeated requests
- protected configuration changes

```text
Security event
      ↓
   Detect
      ↓
    Log
      ↓
 Alert / response
      ↓
  Evidence
```

### Evidence

Event timestamp, event type, source, affected component, response action and resulting state.

### Engineering takeaway

The objective is to make meaningful security events visible early enough to support an appropriate response.

[Next: FR7 — Resource Availability →](08-resource-availability.md)
