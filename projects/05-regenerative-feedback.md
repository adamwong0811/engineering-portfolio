# Regenerative Feedback Circuits and Multivibrator Design

**CV priority:** 05  
**Date:** March 2026  
**Type:** Mixed-Signal Systems Laboratory  
**Tools:** PSpice, TL082 op-amps, ASLK Pro Board, oscilloscope  
**Source report:** `Group 9 MSSL Lab 3 Report.pdf`

## Project Summary

This project investigated positive-feedback op-amp circuits: Schmitt triggers, astable multivibrators, and monostable one-shot pulse generators. The laboratory combined design calculations, PSpice simulation, and physical validation.

## Technical Approach

- Designed inverting and non-inverting Schmitt trigger circuits.
- Varied feedback ratio beta to study hysteresis width and switching threshold movement.
- Converted the regenerative feedback structure into an astable oscillator.
- Designed a monostable pulse generator using diode clamping for stable one-shot behavior.
- Compared simulated and measured timing/frequency results.

## Key Results

| Metric | Result |
| --- | --- |
| Astable target frequency | About 1.4 kHz |
| Simulated astable frequency | 1.372 kHz |
| Practical astable frequency | 1.405 kHz |
| Simulation vs practical error | About 2.35% |
| Monostable output | About 10 ms pulse-width target |

## What I Learned

- How positive feedback creates switching thresholds and hysteresis.
- Why increasing beta widens the hysteresis loop and improves noise immunity.
- How RC timing, op-amp slew rate, parasitic capacitance, and component tolerances affect measured oscillation frequency.
- How diode clamping stabilizes a monostable pulse generator.

## Recruiter Notes

This project is a strong analog fundamentals example because it connects op-amp non-idealities to practical waveform behavior. It also shows the habit of comparing simulation with measured results instead of treating simulation as final truth.

## Next Improvements

- Add waveform screenshots for Schmitt trigger hysteresis, astable output, and monostable pulse.
- Add ASLK Pro Board photos.
- Include calculated beta values and threshold table.
