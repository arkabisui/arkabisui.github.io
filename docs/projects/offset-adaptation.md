# A Discrete-Choice-Driven Update Frequency Framework for Cycle-Wise Offset Adaptation in Vehicle-Actuated Corridors

![Cover image](../assets/images/offset-adaptation-cover.png)

!!! note "Status"
    Ongoing M.Tech research at the Department of Civil Engineering, IIT Bombay.

## Overview

On a coordinated arterial, the offset — the time lag between the start of green at successive intersections — is what creates a green wave. On a **vehicle-actuated** corridor, however, cycle lengths and green splits move from cycle to cycle, so an offset that was optimal one cycle may be stale the next.

The obvious response is to recompute offsets every cycle. But updating is not free: every change disturbs the platoon structure the coordination was meant to protect, and frequent switching can degrade progression rather than improve it. The real question is not *what* the offset should be, but **how often it is worth changing it**.

This project develops a framework that treats the update decision itself as a modelled choice, made afresh at each cycle boundary.

## Objectives

- Formulate the cycle-wise "update or hold" decision as a **discrete choice problem**, with utilities reflecting the expected progression gain against the disruption cost of changing
- Identify the traffic-state variables — arrival profiles, queue residuals, actuated green variability — that carry the most explanatory power for that choice
- Build and calibrate the framework on a simulated vehicle-actuated corridor
- Compare against fixed-offset and every-cycle-update baselines on delay, number of stops and progression quality

## Approach

**1. Corridor modelling.** A representative vehicle-actuated coordinated corridor is built in **PTV VISSIM**, with detector-driven actuation reproducing realistic cycle-to-cycle variability.

**2. Decision formulation.** At each cycle boundary the controller faces a binary alternative — retain the current offset, or adopt a newly computed one. Each alternative is assigned a utility from observable traffic-state attributes plus a random component, yielding a choice probability rather than a hard threshold rule.

**3. Estimation.** Choice model parameters are estimated from simulated corridor data, with the observed performance outcome of each decision supplying the dependent variable.

**4. Evaluation.** The estimated framework is run in closed loop against benchmark control strategies across a range of demand levels and demand asymmetries.

## Tools & Methods

| Component | Tool |
|---|---|
| Micro-simulation | PTV VISSIM |
| Model estimation & analysis | R |
| Network-level context | PTV VISUM |

## Current Status

Model formulation and corridor build are in progress; estimation and comparative evaluation follow.

!!! info "Work in progress"
    Results, figures and the accompanying code will be published here as the study progresses.
