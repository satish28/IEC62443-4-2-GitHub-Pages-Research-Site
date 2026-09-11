---
layout: default
title: FR2 — Use Control
---

# FR2 — Use Control

## What Are You Allowed To Do?

Authentication answers **who**. Use control answers **what that identity may do**.

| Role | ON/OFF | Diagnostics | Configuration | Security administration |
|---|---|---|---|---|
| Operator | ✓ | Limited | — | — |
| Engineer | ✓ | ✓ | Limited | — |
| Administrator | ✓ | ✓ | ✓ | ✓ |

### Demonstration

An authenticated Operator can issue:

```text
RELAY-001|SET|ON
```

but cannot perform protected configuration actions.

The unauthorized action is rejected and recorded.

### Evidence

Role/action matrix, authorization result, rejected operation and audit event.

### Engineering takeaway

Successful authentication should not automatically grant unrestricted authority.

[Next: FR3 — System Integrity →](04-system-integrity.md)
