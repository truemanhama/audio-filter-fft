# Audio Signal Noise Filtering Application

## Overview
This project is a digital signal processing application designed to enhance audio quality by filtering out unwanted noise, such as environmental disturbances or equipment hiss. Developed as part of the **EE320: Signals and Systems** course at **Ashesi University**, the tool provides a graphical user interface (GUI) for applying various digital filters to `.wav` audio files.

The system utilizes **Infinite Impulse Response (IIR) Butterworth filters** to ensure a maximally flat frequency response in the passband, minimizing signal distortion while effectively attenuating noise.

## Features
* **User-Friendly GUI:** Built with Python's `tkinter`, allowing easy file selection and interaction.
* **Multiple Filter Types:**
    * **Low-pass:** Removes high-frequency noise (e.g., hiss).
    * **High-pass:** Removes low-frequency noise (e.g., hum, rumble).
    * **Band-pass:** Isolates a specific frequency range (e.g., speech band).
    * **Band-stop:** Rejects a specific frequency range.
* **Zero-Phase Filtering:** Implements forward-backward filtering (`filtfilt`) to prevent phase distortion in the processed signal.
* **Visual Analysis:** Real-time plotting of time-domain waveforms for both the original and filtered signals.
* **Export:** Save the processed, clean audio as a new `.wav` file.

## Installation

### Prerequisites
Ensure you have **Python 3.x** installed. You will need the following dependencies:

```bash
pip install numpy scipy matplotlib

```

*Note: `tkinter` is usually included with standard Python installations. If you are on Linux, you may need to install `python3-tk` separately.*

### Running the Application

1. Clone this repository.
2. Navigate to the project directory.
3. Run the script:
```bash
python audio_filter_app.py

```



## Usage

1. **Upload Audio:** Click "Upload Audio" to select a `.wav` file from your computer.
2. **Select Filter:** Choose between Low-pass, High-pass, Band-pass, or Band-stop from the dropdown menu.
3. **Configure Parameters:**
* **Cutoff Frequency:** For Low/High-pass filters (default: 1000 Hz).
* **Low/High Cutoff:** For Band-pass/Band-stop filters (defines the frequency range).


4. **Apply Filter:** Click "Apply Filter" to process the audio and view the waveform comparison.
5. **Save:** Click "Save Filtered Audio" to export the result.

## Technical Details

* **Filter Order:** The system uses **4th-order** Butterworth filters to achieve a balance between computational efficiency and a steep roll-off at the cutoff frequency.
* **Signal Processing:**
* **Normalization:** Input signals are normalized to ensure consistent amplitude ranges.
* **Sampling:** The application respects the Nyquist rate (0.5 * fs) when calculating normalized cutoff frequencies.



## Authors

**Group 9**

* Obadiah Safi
* Shadrack Agyei Nti
* Philip Teye Aborsi
* Trueman Hama Mabumbo

```

```
