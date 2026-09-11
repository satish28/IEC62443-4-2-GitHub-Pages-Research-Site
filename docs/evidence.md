---
layout: default
title: Evidence & Testing
---

# Evidence & Testing

## Evidence model

| Test area | Example evidence |
|---|---|
| IAC | Authentication result, logs, packet capture |
| UC | Role/action matrix, authorization result, audit event |
| SI | Integrity metadata, modified-package rejection |
| DC | Protected/unprotected capture comparison |
| RDF | Allowlist, blocked traffic, gateway logs |
| TRE | Event records, alerts, response evidence |
| RA | Rate-limit behaviour, recovery evidence |

## Test pattern

```text
Test Objective
      ↓
Preconditions
      ↓
Test Action
      ↓
Expected Result
      ↓
Observed Result
      ↓
Evidence
      ↓
Conclusion
```
