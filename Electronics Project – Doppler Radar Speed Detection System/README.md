# Electronics Project – Doppler Radar Speed Detection System

## Overview
This project focused on developing a **Doppler radar speed detection prototype**, integrating analog front-end circuit design with embedded firmware and digital display.  
The system combined **filtering, ADC amplification, comparator logic, FFT-based frequency estimation, and CPLD decoding**, ultimately achieving a robust end-to-end pipeline from radar signal to real-time speed display.

---

## Features
- **Analog Signal Conditioning**
  - Designed a **3rd-order Sallen–Key bandpass filter** to isolate Doppler-shifted frequencies (~63 Hz – 825 Hz).
  - Built **low-noise ADC amplifier** to scale the radar output for STM32 acquisition.
  - Implemented **comparator stage** for clean digital pulse generation.

- **Embedded Processing**
  - Programmed STM32 firmware in C (STM32CubeIDE) for **FFT-based dominant frequency estimation**.
  - Configured ADC sampling and interrupt-driven acquisition for real-time data collection.

- **Digital Communication & Display**
  - Established **RS-485 link** between STM32 and external modules.
  - Designed **CPLD logic** (Xilinx ISE) for LED decoding, clock division, and UART signal handling.
  - Built a **LED numeric display** for live speed readout.

---

## Technical Stack
- **Hardware:** STM32 microcontroller, LT1498 op-amp, RS-485 transceiver, CPLD (Xilinx), LED decoder.  
- **Software:** STM32CubeIDE (C), FFT algorithms, UART communication, LTspice simulation, Xilinx ISE (CPLD design).  
- **Tools:** Oscilloscope validation, PCB prototyping, soldered circuit testing.

---

## Results
- Verified bandpass filter and amplifier design through LTspice and oscilloscope measurements.  
- Demonstrated **stable comparator output** suitable for digital FFT (square wave at target Doppler frequency).  
- FFT algorithm successfully estimated target velocity from radar returns.  
- CPLD logic produced clean waveform decoding and LED display output.  
- **First group in class** to deliver a fully functional radar-to-display pipeline.

---

## Visuals
- Bandpass filter output waveform (oscilloscope validation).  
- Comparator output (digital square wave, ready for FFT).  
- CPLD schematic and simulation waveforms.  
- Assembled ADC + Filter + Comparator PCB prototype.

---

## Related Area
Signal Processing • Embedded Firmware (STM32 HAL) • LTspice Simulation • RS-485 Communication • CPLD (Xilinx ISE) • Hardware Debugging • Circuit Prototyping

---

Reports, schematics, and measurement results are included in `/reports/` and `/schematics/`. Full firmware code can be provided on request.
