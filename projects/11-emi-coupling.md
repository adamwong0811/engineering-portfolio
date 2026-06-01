# EMI Coupling Analysis into Shielded Cable

**CV priority:** 11  
**Date:** October 2025  
**Type:** Electromagnetic Compatibility Laboratory  
**Tools:** Altair FEKO, CADFEKO, POSTFEKO  
**Source evidence:** CV details; full FEKO report or model files still needed

## Project Summary

This project modeled electromagnetic coupling between a monopole antenna and an RG58 coaxial cable over a 1-35 MHz frequency range. The goal was to identify frequency regions where shielded cable structures are more susceptible to coupled interference.

## Technical Scope

- Built an EM coupling model in Altair FEKO.
- Simulated a monopole antenna source near an RG58 coaxial cable.
- Swept 51 frequency points from 1 MHz to 35 MHz.
- Used POSTFEKO results to identify resonant coupling peaks.

## Key Results from CV

| Metric | Result |
| --- | --- |
| Frequency sweep | 1-35 MHz |
| Number of points | 51 |
| Cable | RG58 coaxial cable |
| Identified coupling peaks | 6, 12, 18, 25, and 31 MHz |

## What I Learned

- How EMC/EMI problems can be studied through field simulation before hardware testing.
- Why cable geometry, shielding, and resonant frequency behavior matter in real systems.
- How to interpret frequency-domain coupling peaks as practical design risks.

## Recruiter Notes

This project broadens the portfolio beyond circuits into system-level electromagnetic behavior. It is relevant to hardware validation, EMC pre-compliance, cable routing, and interference analysis.

## Missing Before Publishing

- Full lab report or FEKO model files.
- CADFEKO geometry screenshot.
- POSTFEKO coupling-vs-frequency plot.
- Clarification of the measured quantity used for coupling, such as induced current, voltage, or field strength.
