---
layout: default
title: IEC 62443-4-2 Component Cybersecurity Lab
---

# IEC 62443-4-2 Component Cybersecurity Lab

## From a simple relay to a secure industrial component

A practical research and engineering demonstrator exploring **component-level industrial cybersecurity** through seven foundational requirements.

**[Explore the Lab](lab.md)** · **[Read the Series](blog/index.md)** · **[Security Journey](security-journey.md)** · **[Evidence & Testing](evidence.md)**

---

## The question

Industrial cybersecurity cannot stop at the firewall.

The component that ultimately performs an industrial function must also be designed to resist unauthorized access, misuse, tampering, unwanted communication, information exposure, security events and resource exhaustion.

This project makes those concepts visible using **RELAY-001**.

---

## Seven questions. One component.

| Requirement | Question |
|---|---|
| **FR1 — IAC** | Who are you? |
| **FR2 — UC** | What are you allowed to do? |
| **FR3 — SI** | Can I trust what you are running? |
| **FR4 — DC** | What information must be protected? |
| **FR5 — RDF** | Who can talk to you? |
| **FR6 — TRE** | What happens when something goes wrong? |
| **FR7 — RA** | Can you keep operating? |

---

## The lab

```text
Test Client
 Raspberry Pi #1
      |
   Ethernet
      |
Security Gateway
 Raspberry Pi #2
      |
   USB Serial
      |
Arduino RELAY-001
      |
  Relay / DC Load
```

---

## The engineering chain

**Requirement → Security Objective → Threat Scenario → Design → Control → Test → Evidence → Assessment**

---

## Eight-part series

1. Executive — **Why Industrial Components Need Cybersecurity**
2. FR1 — **Who Are You?**
3. FR2 — **What Are You Allowed To Do?**
4. FR3 — **Can We Trust the Component?**
5. FR4 — **What Information Must Be Protected?**
6. FR5 — **Who Can Talk to the Component?**
7. FR6 — **What Happens When Something Goes Wrong?**
8. FR7 — **Can You Keep Operating?**

**[Start the series →](blog/index.md)**

---

## Project philosophy

> **Start simple. Introduce one security objective at a time. Test it. Capture evidence. Then move to the next requirement.**

---

## Disclaimer

This is an independent educational and technical research project. It is not an official IEC publication, is not affiliated with IEC, and does not constitute certification or conformity assessment.

**Safety:** keep the laboratory isolated from production networks and use only low-voltage DC loads.

[Official IEC 62443-4-2 publication](https://webstore.iec.ch/en/publication/34421)
