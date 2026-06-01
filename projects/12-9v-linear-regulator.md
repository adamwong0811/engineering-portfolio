# DC Power Supply - 9 V Linear Regulator

**CV priority:** 12  
**Date:** January 2025  
**Type:** Electrical Circuit Analysis project  
**Tools:** Breadboard, transformer, bridge rectifier, LM7809, oscilloscope, DMM  
**Source report:** `ECAL Project Report Adam Wong 7.pdf`

## Project Summary

This project designed and built a linear DC power supply that converts 240 VAC mains input into a regulated 9 V DC output. The design demonstrates the major stages of a simple linear supply: step-down transformer, bridge rectifier, filter capacitor, and voltage regulator.

## Circuit Stages

| Stage | Component/Function |
| --- | --- |
| Step-down | 240 VAC to 12 VAC transformer |
| Rectification | Four 1N4007 diodes in bridge configuration |
| Filtering | 470 uF, 35 V capacitor |
| Regulation | LM7809 linear voltage regulator |
| Indication | LED with series resistor |

## Key Results

| Measurement Point | Result |
| --- | --- |
| Transformer output | 11.791 V AC measured |
| Rectifier peak | About 15.57 V pulsating DC |
| Regulated output | 9.005 V DC |
| Output observation | Stable DC with no noticeable fluctuation after regulation |

## What I Learned

- How AC waveform stages transform from sinusoidal to rectified to filtered to regulated DC.
- Why capacitor sizing matters for ripple reduction.
- How regulator dropout/headroom affects stable output.
- How to troubleshoot measurement errors, including a faulty multimeter and incorrect resistor selection.

## Recruiter Notes

This project is an early but useful demonstration of power electronics fundamentals and practical lab troubleshooting. It supports later projects by showing comfort with measurement instruments and real circuit construction.

## Next Improvements

- Add oscilloscope waveform screenshots for each stage.
- Add final prototype photo.
- Include a short safety note for mains-powered work.
