# NMOS Current Mirror Circuit Design

**CV priority:** 09  
**Date:** January 2026  
**Type:** Mixed-Signal Systems Laboratory  
**Tools:** PSpice, BS107A NMOS model  
**Source report:** `GROUP 9 (FRIDAY SESSION)_MSSL LAB REPORT 1.pdf`

## Project Summary

This project characterized an NMOS transistor model and used the extracted parameters to design a current mirror. The objective was to generate a stable 5 mA load current and study how mirror performance changes with load voltage.

## Technical Approach

- Estimated BS107A threshold voltage from DC sweep simulation.
- Estimated conduction parameter KN from simulated VGS and drain current.
- Designed reference branch resistor for a 5 mA target current.
- Simulated the current mirror and swept load voltage to identify compliance behavior.

## Key Results

| Metric | Result |
| --- | --- |
| Estimated VT | About 1.2153 V |
| Estimated KN | About 15.59 mA/V^2 |
| Target mirror current | 5 mA |
| Simulated IREF | 4.970 mA |
| Simulated IL | 4.868 mA |
| Minimum load voltage | About 5.5663 V |

## What I Learned

- How current mirrors create bias currents in analog circuits.
- Why saturation-region operation is essential for stable mirrored current.
- How compliance voltage limits the usable output range of a current mirror.
- How transistor model parameters influence calculated versus simulated current.

## Recruiter Notes

Current mirrors are a fundamental analog IC biasing block. This project pairs device parameter extraction with circuit-level bias design, which is valuable for analog/mixed-signal design interviews.

## Next Improvements

- Add DC sweep plots for IREF, IL, VGS, and output voltage.
- Compare ideal square-law assumptions with SPICE model behavior.
- Add a small schematic image for quick readability.
