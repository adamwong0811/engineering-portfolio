# High-Fidelity Class AB Headphone Amplifier

**CV priority:** 01  
**Date:** April 2026  
**Type:** Personal engineering project  
**Tools:** PSpice, breadboard prototype, KiCad in progress  
**Source report:** `NE5532_HeadphoneAmp_Report.docx`, `NE5532_HeadphoneAmp_Report.pdf`

## Visual Evidence To Add

Suggested asset filenames:

- `assets/headphone-amp-dual-supply-schematic.png`
- `assets/headphone-amp-dual-supply-transient.png`
- `assets/headphone-amp-dual-supply-thd.png`
- `assets/headphone-amp-dual-supply-ac-response.png`
- `assets/headphone-amp-single-supply-schematic.png`
- `assets/headphone-amp-single-supply-transient.png`
- `assets/headphone-amp-single-supply-thd.png`
- `assets/headphone-amp-single-supply-ac-response.png`

## Project Summary

This project is a desktop headphone amplifier designed for the Sennheiser HD490 Pro, a 130 ohm professional monitoring headphone. The amplifier uses an NE5532 dual op-amp as the voltage-gain stage and a complementary BD139/BD140 Class AB push-pull output stage to supply the current required by the headphone load.

The design was developed as a complete analog signal-chain project: target specification, hand calculation, PSpice validation, breadboard prototype, and PCB migration planning.

## Design Architecture

- NE5532 op-amp voltage stage for low-noise precision gain.
- Complementary BD139/BD140 Class AB emitter-follower output buffer.
- Global feedback path redesigned to include the transistor output stage, reducing crossover distortion.
- 18 V single-supply architecture with an active virtual ground rail splitter.
- Output coupling capacitor sized to protect the headphone from DC offset while preserving low-frequency response.

## Key Results

| Metric | Result |
| --- | --- |
| Closed-loop voltage gain | 9.35 dB, about 3 V/V |
| THD at 1 kHz | 0.064%, below the 0.1% design target |
| Phase margin | 110.6 degrees |
| Audio-band response | Flat within about +/-0.1 dB across 20 Hz-20 kHz |
| Extended bandwidth | About 10 Hz to 300 kHz within +/-0.05 dB |
| DC output offset | Less than 15 mV in the report; CV records -8.1 mV |
| Output transistor idle dissipation | About 49.2 mW per device |
| NE5532 dissipation | About 143.6 mW |

## What I Learned

- How op-amp feedback theory changes when a discrete output buffer is placed inside the loop.
- Why Class AB biasing must balance crossover distortion, idle dissipation, and thermal stability.
- How to check headphone safety through DC-offset analysis and AC coupling.
- How to read stability margins and frequency response as practical design constraints rather than isolated simulation plots.

## Recruiter Notes

This is the strongest portfolio project because it combines analog design, audio performance metrics, simulation literacy, component-level reasoning, and hardware prototyping. It is directly relevant to analog/mixed-signal internship roles, audio electronics, and hardware validation.

## Next Improvements

- Complete the two-layer KiCad PCB layout.
- Add PCB photos, schematic screenshots, and measured oscilloscope results.
- Compare breadboard measurements against PSpice simulations.
- Consider Vbe multiplier bias control and output protection relay in a future revision.
