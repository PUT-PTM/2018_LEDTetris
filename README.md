# 2018_LEDTetris

# 1. Overview 📖

Our goal was to create tetris game controlled by four buttons. The whole output is presented on two 8x8 LED matrices connected to each other.

# 2. Description 📌

Two merged matrices give us 128 diodes. We are using MAX7219 Driver which allows SPI communication. To control slowly dropping blocks during the game, we operate on 4 buttons. First is responsible for moving target one position right, second one position left, third increases speed of falling and the last one changes a shape of block.

# 3. Specification 📃

- 8x8 LED Matrix Specification

| Name | Value |
| :---: | :---: | 
| Operating Voltage | DC 4.7V~5.3V |
| Operating Current | 320mA |
| Max Operating Current | 2A |
| LED Color | Red |
| Resistor | 10kΩ |
| Ceramic capacitor | 100 nF / 25 V |
| Electrolytic capacitor | 10 uF / 25 V |


# 4. Tools 🔧

- STM32F4DISCOVERY,
- 8x8 LED Matrix + MAX7219 Driver (2x),
- Waveshare board 8 push buttons,
- Wires to connect the items.

# 5. How to run 🔥

Run program in System Workbench C/C++ Developers for STM32 and connect wires as follows

STM32F4DISCOVERY

| STM32F4DISCOVERY | Push Buttons |
| :---: | :---: | 
| GND | G |
| PE11 | K0 |
| PE12 | K5 |
| PE13 | K4 |
| PE14 | K1 |


| STM32F4DISCOVERY | Matrix 1# |
| :---: | :---: | 
| 5V | VCC |
| GND | GND |
| PA5 | CLK |
| PA7 | DIN |
| PC5 | CS |


| Matrix 1# | Matrix 2# |
| :---: | :---: | 
| VCC | VCC |
| GND | GND |
| CLK | CLK |
| DIN | DIN |
| CS | CS |


# 6. How to compile ⚡️

Run program in System Workbench Developers C/C++ for STM32.

# 7. Future improvements 🔨

Add another two matrices creating a display with 256 LED diodes.

# 8. Attributions 💾

HAL library https://github.com/petoknm/MAX7219/

# 9. License 📑

MIT license. Read license.txt for more.

# 10. Credits 🏆

- Kamil Rogowski
- Patryk Romaniak

The project was conducted during the Microprocessor Lab course held by the Institute of Control and Information Engineering, Poznan University of Technology. Supervisor: Adam Bondyra.
