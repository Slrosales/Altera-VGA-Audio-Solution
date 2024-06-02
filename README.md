
<div align="center">
  <h1>
    VGA Image and Audio Visualization Project
  </h1>

<h4>
    Computer Structure I
  </h4>

[![GitHub Slrosales](https://img.shields.io/badge/by-Slrosales-purple)](https://github.com/Slrosales)
[![GitHub Rubens1414](https://img.shields.io/badge/by-jfbenitezz-blue)](https://github.com/jfbenitezz)
[![GitHub JaymedDLC](https://img.shields.io/badge/by-FernandoMVG-green)](https://github.com/FernandoMVG)

</div>

## Project Description

This project is part of the Computer Structure I course at Universidad del Norte, guided by Professor Eduardo Zurek. The objectives include implementing a VGA protocol on an Altera DE2-115 board to display a preprocessed image, and programming a Nios II soft-processor to play Spanish vowel sounds when vowel keys are pressed.

## Features

- **VGA Signal Generation**: Implementation of a VGA protocol to display an image with a resolution of 640x350 pixels on a VGA monitor.
- **Image Preprocessing**: Utilization of a Python script to adapt the image to the required size and resolution.
- **Audio Output on Vowel Input**: Using the Nios II soft-processor, the system plays a specific vowel sound when the corresponding vowel key is pressed on a keyboard.
- **FPGA-Based Implementation**: Use of an Altera DE2-115 board for the development and execution of the VHDL and Assembly code.

## Installation and Usage

1. **Clone the Repository**: 
   ```bash
   git clone https://github.com/your-username/vga-image-audio-visualization.git
   ```
2. **Set Up the Hardware**: Connect the Altera DE2-115 board as per the hardware setup instructions provided in the `hardware-setup.md`.
3. **Load the VHDL and Assembly Code**: Use Quartus II to compile and load the VHDL and Assembly code onto the FPGA.
4. **Run the Python Preprocessor for Image**: 
   ```bash
   python preprocess_image.py
   ```
   Ensure you have the correct image file in the specified directory.
5. **View the Output and Listen to Audio**: Power on the FPGA with the connected VGA monitor and keyboard to see the output image displayed and hear the vowel sounds when keys are pressed.

## Solution Overview

The chosen solution involves preprocessing an image using a Python script to fit specific criteria and then using VHDL to display this image centered on a VGA monitor. Additionally, the system plays audio files when vowel keys are pressed, implementing a Nios II processor programmed in Assembly language. The system adheres to various constraints, including resolution, positioning, and audio memory constraints.

## Team

- Felipe Jose Benitez Avilez
- Laura Sofía Gómez Rosales
- Fernando Mateo Valencia Gómez
