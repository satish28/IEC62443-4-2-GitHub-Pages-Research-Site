---
layout: default
title: FR3 — System Integrity
---

# FR3 — System Integrity

## Can We Trust What the Component Is Running?

A component can be authenticated and authorized and still be unsafe if its software or security-relevant configuration has been modified.

### RELAY-001 experiment

```text
Expected package
       |
 Integrity check
       |
   +---+---+
 valid   modified
   |        |
 accept   reject
```

A valid package is compared with a deliberately modified copy.

### Evidence

Integrity metadata, verification result, rejection result, component/event log and test record.

### Engineering takeaway

Integrity protection should be tied to an explicit security objective and verified with negative testing.

[Next: FR4 — Data Confidentiality →](05-data-confidentiality.md)
