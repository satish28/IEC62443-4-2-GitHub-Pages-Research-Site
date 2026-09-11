# Lab Setup

## Architecture

```text
Laptop / Engineering PC
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
 Relay Driver
        |
Low-voltage DC Load
```

## Recommended hardware

- 2 × Raspberry Pi 4
- 1 × Arduino
- 1–2 × 1-channel 5 V relay modules
- Breadboard and jumper wires
- Ethernet switch and cables
- USB cables
- Low-voltage 5 V/12 V LED or lamp
- LEDs/resistors
- Optional push buttons
- Enclosure/project box
- Low-voltage DC power supply

**Do not use mains voltage.**

## Example lab network

- Pi #1: `192.168.50.10`
- Pi #2: `192.168.50.20`
- Engineering PC: `192.168.50.30`

## Initial command model

```text
RELAY-001|SET|ON
RELAY-001|SET|OFF
RELAY-001|STATUS
```

The protocol is deliberately simple so security controls can be introduced progressively.

## Progressive stages

1. Functional baseline
2. IAC — identity/authentication
3. UC — authorization
4. SI — firmware/configuration integrity
5. DC — protected information exchange
6. RDF — gateway allowlisting
7. TRE — event detection/logging
8. RA — rate limiting/recovery

## Evidence

Capture configuration, source code, packet captures, authentication/authorization results, gateway logs, event records, integrity results, test scripts and before/after component state.
