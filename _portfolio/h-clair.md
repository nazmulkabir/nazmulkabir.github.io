---
title: "H-CLAIR: Physical Safety Under a Compromised Automation Plane"
excerpt: "Actuation-time reference monitor that keeps industrial plants inside their safe operating envelope even when the anomaly detector, controller, and fallback are all compromised."
collection: portfolio
permalink: /portfolio/h-clair/
link: /projects-html/h-clair/
date: 2026-09-01
tags:
  - CPS Security
  - Runtime Assurance
  - Water Systems
---

- Shows that detector-gated automation can catch faults, avoid false alarms, defer on almost every attacked sample, and still drive water tanks out of their safe range.
- Moves the safety decision to actuation time: a small shield mediates the only path to the actuator and treats every request from the detector, learned controller, and fallback as untrusted.
- Maintains the set of plant states consistent with authenticated sensor records and the commands actually executed, and admits a command only if every reachable successor stays in a certified safe region.
- Proves invariant preservation against arbitrary adaptive requests, and derives an assurance horizon that marks when stale trusted state can no longer guarantee a safe command.
- Evaluated over Modbus/TCP, on a held-out nonlinear plant, on SWaT/WADI adaptive evasion, and in closed-loop BATADAL C-Town hydraulics.

[Read the full project write-up](/projects-html/h-clair/)
