---
layout: default
title: FR7 — Resource Availability
---

# FR7 — Resource Availability

## Can You Keep Operating?

Industrial components often have constrained resources. A security mechanism that consumes all available resources can itself become an availability problem.

### Controlled experiment

The isolated lab generates excessive requests and evaluates mechanisms such as:

- rate limiting
- request controls
- resource protection
- watchdog/recovery behaviour

```text
Excessive requests
       |
       v
Protection mechanism
       |
   +---+---+
 protect  recover
 resource safely
```

### Evidence

Request rate, component behaviour, rate-limit result, resource observations, recovery result and event logs.

### Engineering takeaway

Availability is about designing the component so abnormal activity does not unnecessarily prevent its intended function.

### The journey is complete

**Who are you? → What are you allowed to do? → Can I trust what you are running? → What information must be protected? → Who can talk to you? → What happens when something goes wrong? → Can you keep operating?**

[Back to the series →](index.md)
