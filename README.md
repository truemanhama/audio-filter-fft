# audio-filter-fft
This project focused on the design and implementation of a robust digital signal processing system aimed at enhancing audio clarity by removing unwanted environmental and equipment-induced noise.

# Audio Signal Noise Filtering Application

## Overview
[cite_start]This project is a digital signal processing application designed to enhance audio quality by filtering out unwanted noise, such as environmental disturbances or equipment hiss[cite: 12, 13]. [cite_start]Developed as part of the **EE320: Signals and Systems** course at **Ashesi University**[cite: 1, 2], the tool provides a graphical user interface (GUI) for applying various digital filters to `.wav` audio files.

[cite_start]The system utilizes **Infinite Impulse Response (IIR) Butterworth filters** to ensure a maximally flat frequency response in the passband, minimizing signal distortion while effectively attenuating noise[cite: 141, 563].

## Features
* [cite_start]**User-Friendly GUI:** Built with Python's `tkinter`, allowing easy file selection and interaction[cite: 153, 154].
* **Multiple Filter Types:**
    * [cite_start]**Low-pass:** Removes high-frequency noise (e.g., hiss)[cite: 56, 58].
    * [cite_start]**High-pass:** Removes low-frequency noise (e.g., hum, rumble)[cite: 60, 62].
    * [cite_start]**Band-pass:** Isolates a specific frequency range (e.g., speech band)[cite: 64, 66].
    * [cite_start]**Band-stop:** Rejects a specific frequency range[cite: 68].
* [cite_start]**Zero-Phase Filtering:** Implements forward-backward filtering (`filtfilt`) to prevent phase distortion in the processed signal[cite: 36, 113].
* [cite_start]**Visual Analysis:** Real-time plotting of time-domain waveforms for both the original and filtered signals[cite: 100, 118].
* [cite_start]**Export:** Save the processed, clean audio as a new `.wav` file.

## Installation

### Prerequisites
Ensure you have **Python 3.x** installed. You will need the following dependencies:

```bash
pip install numpy scipy matplotlib
