
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


## VGA Implementation Details

In this project, we developed a system to display a preprocessed image on a VGA monitor using an Altera DE2-115 board, following a specific resolution of 640x350 pixels. The image, centrally positioned and sized at 128x128 pixels, represents a location in Barranquilla, distinct from the Uninorte campus.

### Key Components:
- **Python Preprocessing**: The image undergoes preprocessing using a Python script to adjust its size and convert the RGB values into an 8-bit binary format suitable for VHDL processing.
- **VHDL Display Logic**: Implemented in VHDL, the system reads the binary color vectors and calculates the correct starting position on the screen to ensure the image is centered.
- **Technical Compliance**: The system adheres to the VGA protocol standards, ensuring compatibility with a standard VGA monitor.

### Challenges and Solutions:
- **Image Positioning**: Ensuring the image is exactly centered involved precise calculations within the VHDL code to align the image properly on the VGA display.
- **Memory and Format Constraints**: The image data, stored in three separate .txt files for each RGB component, had to be efficiently managed to fit the FPGA's memory constraints while maintaining high visual fidelity.

This VGA implementation demonstrates the capability of FPGA-based systems to handle complex image processing tasks while adhering to strict technical specifications.


## Audio Implementation Details

The audio functionality of this project involves playing back vowel sounds on a Nios II soft-processor. Initially, audio files for each vowel were recorded and meticulously edited to fit within the memory constraints of the NIOS II, with each sound optimized to last only 1 second and stored as vectors of 4252 elements. The software logic detects vowel key presses, accesses the corresponding audio vector, and plays the sound until the end of the vector is reached. The system then resets the key register and waits for the next interaction. Exception handling is integrated to ensure the FPGA software operates correctly under these conditions.


## Team

- Felipe Jose Benitez Avilez
- Laura Sofía Gómez Rosales
- Fernando Mateo Valencia Gómez
