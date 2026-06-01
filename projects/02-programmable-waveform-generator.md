# Digitally Programmable Square and Triangular Wave Oscillator

**CV priority:** 02  
**Date:** April 2026  
**Type:** Mixed-Signal Systems Laboratory project  
**Tools:** PSpice, DAC7821/`DAC12break`, TL082 op-amps  
**Source report:** `Mixed Signal System Lab Report Group 9.pdf`

## Project Summary

This project designed a digitally controlled oscillator that generates square and triangular waveforms. Instead of setting the oscillator frequency only through fixed resistors and capacitors, the circuit uses a 12-bit multiplying DAC to make the frequency programmable through a digital input word.

The oscillator is based on an integrator-comparator architecture. The MDAC controls the effective current into the integrator, so changing the digital code changes the capacitor charging rate and therefore the oscillation frequency.

## Technical Approach

- Built a mixed-signal oscillator around a DAC7821 MDAC model and TL082 op-amps.
- Derived the frequency relationship between digital input code and integrator current.
- Ran PSpice transient sweeps across selected digital codes.
- Compared calculated and simulated frequency values.
- Checked that square-wave and triangular-wave amplitudes remain constant as frequency changes.

## Key Results

| Metric | Result |
| --- | --- |
| Frequency range | 50 Hz to 400 Hz |
| Control method | 12-bit digital input word through MDAC |
| Output waveforms | Square wave and triangular wave |
| Frequency accuracy | Under 0.66% discrepancy against theoretical model |
| Main non-ideality identified | Finite op-amp gain-bandwidth effects |

## What I Learned

- How an MDAC can convert a digital control word into an analog timing current.
- How mixed-signal systems combine mathematical transfer functions with analog limitations.
- Why frequency remains programmable while amplitude can remain constant in a well-structured oscillator.
- How to compare theoretical, simulated, and practical sources of error.

## Recruiter Notes

This project shows mixed-signal thinking: digital control, analog waveform generation, and validation against a derived model. It is relevant to signal generation, sensor interfaces, test equipment, and embedded analog front-end work.

## Next Improvements

- Add PSpice schematic and waveform screenshots.
- Include the calculation table for each digital code.
- Confirm whether the design was physically implemented or simulation-only.
