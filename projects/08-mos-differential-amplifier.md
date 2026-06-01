# MOS Differential Amplifier Design and Simulation

**CV priority:** 08  
**Date:** January 2026  
**Type:** Mixed-Signal Systems Laboratory  
**Tools:** PSpice, BS107A NMOS models, TL082 op-amp model  
**Source report:** `GROUP 9 LAB 2 MSSL.pdf`

## Project Summary

This project designed and simulated a basic NMOS differential amplifier with current-source biasing. The circuit was analyzed for differential gain, common-mode response, and Common-Mode Rejection Ratio behavior.

## Design Targets and Biasing

- Differential pair using BS107A NMOS models.
- Target drain currents: ID1 = ID2 = 3 mA.
- Tail current: 6 mA under balanced input conditions.
- Target VDS around 4 V.
- Drain resistors derived from the bias point.

## Key Results

| Metric | Result |
| --- | --- |
| Differential gain | About 9.90 |
| Input test signal | 20 mV peak at 1 kHz |
| Output swing for differential test | About 195.928 mV peak |
| Tail current | 6 mA |
| Common-mode output variation | About 21.806 uV for 20 mV input |

## What I Learned

- How a MOS differential pair steers current between two branches.
- How common-mode signals can be rejected when the bias source has high output resistance.
- Why small-signal input amplitude must stay within the linear region.
- How to extract differential-mode and common-mode behavior from transient simulations.

## Recruiter Notes

This project is directly relevant to analog IC design fundamentals. Differential pairs and current-source biasing are core building blocks in op-amps, comparators, sensor front ends, and mixed-signal ICs.

## Next Improvements

- Add PSpice schematic and gain plots.
- Include calculated CMRR value if available in the final simulation results.
- Add a short explanation of saturation-region limits.
