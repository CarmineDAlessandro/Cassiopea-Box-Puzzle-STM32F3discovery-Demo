# Cassiopea-Box-Puzzle-STM32F3discovery-Demo
When a university project becomes a puzzle.

## Overview
This project is made for the class of Embedded Systems. The official board of the class is the STM32F3discovery and the real time operative system ChibiOS. You can find information on the board at [this link](https://www.st.com/en/evaluation-tools/stm32f3discovery.html) and on the RTOS at [this link](http://chibios.org/dokuwiki/doku.php).

The program reads data from the accellerometer and gyroscope, outputting on the leds of the puzzle and debug information on the serial port.

## DIY - Getting started
### What hardware you need
- 1 STM32F3discovery
- 5 white leds
- 3 yellow leds
- 8 electric resistances
- A breadboard
- 25 male to female jumper cables
- A box
### What software you need
- ChibiStudio correctly installed (You can download it at [this link](http://www.chibios.org/dokuwiki/doku.php?id=chibios:downloads:start))
### Make LED the circuit
PXN is the pin of the led. X indicates the letter, N the number. The used pins are: PC0, PC1, PC2, PC3, PB0, PB1, PB2, PB3.
GND is the ground pin.

Use the breadboard to make the circuit. You will not need more material than the one in the list above.

![LED circuit](https://github.com/CarmineDAlessandro/Cassiopeia-Box-Puzzle-STM32F3discovery-Demo/blob/master/led%20circuit.JPG)
## Flash and Run the code
Download the zipped code, unzip it, open ChibiStudio and import "existing project". Connect the board to an USB plug, then click on the "External Tool" icon in the upper part of the IDE and select "OpenOCD on STLink ..." and select the correct configuration file at the path "ChibiStudio\tools\openocd\scripts\board\stm32f3discovery.cfg". You are ready to run the debug configuration of the code.
