# Modelling of Soil–Pile Interaction of a Bridge Pier Foundation

![Cover image](../assets/images/soil-pile-cover.png)

!!! note "Context"
    Undergraduate project, Department of Civil Engineering, IIEST Shibpur.

## Overview

A bridge pier does not stand on soil so much as it stands *with* it. Under lateral load — traffic braking, wind, stream flow, seismic action — the pile group and the surrounding soil deform together, and the load a pile actually attracts depends on how stiff the soil around it is. Treating the foundation as a fixed base misses this entirely, and usually on the unsafe side for the pier.

This project models that interaction explicitly for a bridge pier pile foundation.

## Objectives

- Represent the pile group and surrounding soil as an interacting system rather than a fixed support
- Study the lateral load–deflection response of the pile group
- Examine load distribution among piles within the group, including group effects
- Compare the modelled response with the conventional fixed-base idealisation

## Methodology

**Soil characterisation.** The subsurface profile was idealised into layers with representative strength and stiffness parameters, and modulus of subgrade reaction values derived for each layer.

**Modelling approach.** The soil was represented using the **Winkler spring idealisation** — a series of discrete springs along the pile shaft, with stiffness varying with depth in accordance with the soil profile — rather than a rigid support.

**Analysis.** The pier–pile system was analysed in **STAAD.Pro** under vertical and lateral load combinations, producing deflections, bending moments and shear along the pile, together with the distribution of load among individual piles.

**Comparison.** Results were compared against a fixed-base model to quantify the effect of including soil compliance.

## Key Learnings

- Foundation flexibility materially changes the bending moment demand transmitted to the pier — a fixed-base assumption is not conservative for the superstructure.
- The depth of maximum bending moment in a laterally loaded pile is governed by relative soil–pile stiffness, not by the loading alone.
- Within a pile group, corner and edge piles attract load differently from interior piles; designing all piles for the average is inadequate.

## Tools

**STAAD.Pro** · **AutoCAD** · IS 2911 and IRC provisions for pile foundations
