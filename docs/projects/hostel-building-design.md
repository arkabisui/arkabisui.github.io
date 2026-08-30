# Detailed Design of a G+2 Hostel Building (RCC)

![Cover image](../assets/images/hostel-building-cover.png)

!!! note "Context"
    Undergraduate design project, Department of Civil Engineering, IIEST Shibpur.

## Overview

A complete structural design of a three-storey (ground plus two) reinforced concrete hostel building — taken from architectural layout through analysis, member design and reinforcement detailing, in accordance with Indian Standard codes.

## Scope of Work

**Planning.** Architectural layout of rooms, corridors, staircases and service areas suited to hostel occupancy, and derivation of a structural grid from it.

**Load assessment.** Dead loads from the assumed build-up, live loads per occupancy class, and lateral loads — all evaluated to the relevant IS code provisions.

**Structural analysis.** Three-dimensional frame modelling and analysis in **STAAD.Pro** under the full set of load combinations, yielding design forces for every member.

**Member design.**

- **Slabs** — two-way and one-way slabs, designed by the limit state method
- **Beams** — flexure, shear and deflection checks with reinforcement detailing
- **Columns** — axial and biaxial bending design across all three storeys
- **Foundations** — isolated and combined footings sized to safe bearing capacity
- **Staircase** — dog-legged staircase slab design

**Detailing and drawings.** Reinforcement detailing and structural drawings prepared in **AutoCAD**, following IS 13920 ductile detailing provisions where applicable.

## Codes Referenced

- **IS 456:2000** — Plain and Reinforced Concrete, Code of Practice
- **IS 875 (Parts 1–3)** — Design Loads for Buildings and Structures
- **IS 1893 (Part 1)** — Criteria for Earthquake Resistant Design
- **IS 13920** — Ductile Detailing of RC Structures
- **SP 16** — Design Aids for Reinforced Concrete

## Key Learnings

- Analysis output is a starting point, not a design — serviceability and detailing rules governed as many member sizes here as strength did.
- Regularising the structural grid early, in dialogue with the architectural layout, removed a great deal of downstream difficulty in the frame.

## Tools

**STAAD.Pro** · **AutoCAD** · **MS Excel** (design spreadsheets)
