---
layout: default
title: FR1 — Identification & Authentication
---

# FR1 — Identification & Authentication Control

## Who Are You?

Authentication is the first security question for RELAY-001:

> **Can the component distinguish an authorized source from an unknown or invalid source?**

```text
Pi #1 Test Client
       |
       v
Pi #2 Gateway
       |
       v
RELAY-001
```

### Demonstration

Compare:

- valid authenticated request
- invalid credentials
- unknown request source
- repeated failed authentication

### Expected behaviour

```text
Valid identity → authentication succeeds → request proceeds

Invalid/unknown → authentication fails → command rejected → event recorded
```

### Evidence

Authentication configuration, accepted/rejected requests, logs and packet captures where appropriate.

### Engineering takeaway

Authentication is part of controlling which sources are trusted to initiate security-relevant actions.

[Next: FR2 — Use Control →](03-use-control.md)
