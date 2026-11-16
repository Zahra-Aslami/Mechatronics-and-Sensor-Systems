# NTC Temperature Sensor Design

## Project Overview
This project involved the design and simulation of an analog circuit using an NTC thermistor to measure human body temperature (36°C to 40°C) with a precision of 0.1°C. The primary objective was to convert the nonlinear resistance changes of the NTC into a readable voltage, amplify the small signal variations, and filter out environmental and power-line noise.

## Key Design Elements
*   **Sensor & Bridge Circuit:** Modeled the NTC behavior (Steinhart-Hart equation) and designed a Wheatstone bridge with precision E12 resistors to extract the voltage difference.
*   **Signal Amplification:** Designed a two-stage non-inverting operational amplifier circuit to achieve a total gain of ~200, amplifying the tiny millivolt changes to a measurable range.
*   **Op-Amp Selection:** Evaluated different op-amps and selected a FET-input op-amp with low offset voltage (50 µV) to minimize error and bias current.
*   **Active Filtering:** Designed a band-pass filter (combining a High-Pass filter at 1 Hz and a Low-Pass filter at 10 Hz) to eliminate 1 kHz power-line noise while preserving the low-frequency physiological signal.
*   **Simulation:** Validated all theoretical calculations and circuit performance using LTspice simulations.

## Tools Used
*   **LTspice:** Circuit simulation and frequency analysis (AC sweep).
