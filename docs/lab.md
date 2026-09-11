---
layout: default
title: Lab
---

# Laboratory

## RELAY-001 Component Cybersecurity Demonstrator

```text
Engineering PC
      |
   Ethernet
      |
Pi #1 — Test Client
      |
   Ethernet
      |
Pi #2 — Security Gateway
      |
   USB/Serial
      |
Arduino — RELAY-001
      |
Relay / DC Load
```

## Lab principles

1. Isolate the environment.
2. Use low-voltage DC loads.
3. Separate testing from the component.
4. Capture evidence for every experiment.
5. Change one security capability at a time.
6. Repeat tests after each security change.

## Experiment flow

```text
Baseline → Threat Scenario → Security Objective
        → Control → Negative Test
        → Expected Behaviour → Evidence → Conclusion
```
