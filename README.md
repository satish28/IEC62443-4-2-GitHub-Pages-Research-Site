# IEC 62443-4-2 Component Cybersecurity Lab

### From a simple relay to a secure industrial component

> A practical research and engineering demonstrator for understanding component-level cybersecurity through the seven foundational requirements of IEC 62443-4-2.

**[Explore the Lab](docs/lab.md)** · **[Read the Series](docs/blog/index.md)** · **[Security Journey](docs/security-journey.md)** · **[Evidence & Testing](docs/evidence.md)**

---

## Why this project?

Industrial cybersecurity cannot stop at the firewall.

The component that ultimately performs an industrial function must also be designed to resist unauthorized access, misuse, tampering, information exposure, unwanted communication, security events and resource exhaustion.

This project explores that problem using a deliberately simple **RELAY-001** industrial component demonstrator.

The relay starts as a basic functional device. Across the project, security capabilities are progressively introduced and tested against the seven foundational requirements:

**IAC → UC → SI → DC → RDF → TRE → RA**

---

## The industrial question

| IEC 62443-4-2 FR | Industrial question |
|---|---|
| **FR1 — IAC** | **Who are you?** |
| **FR2 — UC** | **What are you allowed to do?** |
| **FR3 — SI** | **Can I trust what you are running?** |
| **FR4 — DC** | **What information must be protected?** |
| **FR5 — RDF** | **Who can talk to you?** |
| **FR6 — TRE** | **What happens when something goes wrong?** |
| **FR7 — RA** | **Can you keep operating?** |

---

## Lab architecture

```text
Engineering PC
      |
   Ethernet
      |
Pi #1 — Test Client
      |
   Ethernet
      |
Pi #2 — Security Gateway / Monitoring
      |
   USB Serial
      |
Arduino — RELAY-001
      |
Relay Driver → Relay → Low-voltage DC Load
```

The lab is isolated and uses low-voltage DC loads.

---

## From requirement to evidence

```text
Requirement
     ↓
Security Objective
     ↓
Threat Scenario
     ↓
Component Design
     ↓
Security Control
     ↓
Security Test
     ↓
Evidence
     ↓
Assessment
```

A successful configuration is not automatically proof that a security objective is satisfied. The project therefore connects controls with repeatable negative testing and evidence.

---

## Eight-part publication series

1. **Executive:** Why Industrial Components Need Cybersecurity
2. **FR1 — IAC:** Who Are You?
3. **FR2 — UC:** What Are You Allowed To Do?
4. **FR3 — SI:** Can We Trust the Component?
5. **FR4 — DC:** What Information Must Be Protected?
6. **FR5 — RDF:** Who Can Talk to the Component?
7. **FR6 — TRE:** What Happens When Something Goes Wrong?
8. **FR7 — RA:** Can You Keep Operating?

**[Read the full series →](docs/blog/index.md)**

---

## Repository structure

```text
.
├── README.md
├── LAB_SETUP.md
├── BLOG_SERIES.md
├── docs/
│   ├── index.md
│   ├── lab.md
│   ├── security-journey.md
│   ├── evidence.md
│   └── blog/
│       ├── index.md
│       └── 01–08 articles
├── lab/
│   ├── arduino/
│   └── raspberry-pi/
├── tests/
└── evidence/
```

## Safety and disclaimer

This is an independent educational and technical research project. It is not an official IEC publication and does not constitute certification or conformity assessment.

Keep the lab isolated from production OT/ICS environments. Use only low-voltage DC loads.

Official reference: [IEC 62443-4-2:2019](https://webstore.iec.ch/en/publication/34421)
