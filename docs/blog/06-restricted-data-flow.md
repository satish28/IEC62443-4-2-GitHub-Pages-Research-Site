---
layout: default
title: FR5 — Restricted Data Flow
---

# FR5 — Restricted Data Flow

## Who Can Talk to the Component?

The RELAY-001 architecture introduces a gateway between the test client and the component.

```text
Approved client
      |
      v
+-------------+
|   Gateway   |
| Allowlisting|
+------+------+
       |
       v
  RELAY-001

Unapproved source → blocked
```

### Demonstration

1. approved client → allowed
2. unapproved source → blocked
3. direct component access → prevented where architecture requires it

### Evidence

Gateway configuration, allowed/blocked connections, logs and packet captures.

### Engineering takeaway

Restricted data flow is an architectural control as much as a filtering rule.

[Next: FR6 — Timely Response →](07-timely-response.md)
