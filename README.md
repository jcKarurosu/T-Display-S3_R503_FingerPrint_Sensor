# T-Display-S3 and R503 FingerPrint sensor [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)

Example of how to use the R503 FingerPrint sensor using the T-Display S3 board from LILYGO. The code creates a simple screen menu on the display to control the main functions of the sensor.

![project-pic](https://github.com/jcKarurosu/PuertaDigital/blob/master/sensor_project.jpg?raw=true)

## Files

There are 4 files:

- `main.py`: This file displays a text styled menu to the user, allowing them to test the functionality of the sensor. It also shows how to control and display simple text on the board's display.

- `r503_sensor.py`: Located within the `jcLibs` folder, this file contains the core functions necessary for interacting with the sensor. It is the primary file you should use to quickly implement a program that works with the R503 sensor. 

- `tft_buttons.py`: Defines the Buttons class.

- `tft_config.py` : Sets pin numbers and defines functions to init and deinit the display.

## Hardware

- [R503 Fingerprint Sensor 3.3V version](https://zjgrow.com/grow-r503-new-circular-round-two-color-ring-indicator-led-control-dc33v-mx10-6pin-capacitive-fingerprint-module-sensor-scanner-p2112363.html)
- [T-Display-S3](https://lilygo.cc/products/t-display-s3)
- Optional but nice to work with your T-Display-S3: [3D printed case for T-Display-S3 board](https://cults3d.com/es/modelo-3d/artilugios/case-for-lilygo-t-display-s3)

## Software

- Thonny
- Micropython on the T-Display-S3, specific Micropython firmware from [here](https://github.com/russhughes/s3lcd/tree/main)

## Setting the Hardware

Make the connections that are shown in the next table

![Conections Screenshot](https://github.com/jcKarurosu/PuertaDigital/blob/3e25b58e8b9a72f8de88a6904444b84a41dc4ec0/T-Display-S3_R503_Sensor/Conections.png)

Use a USB type-C cable to connect the T-Display-S3 to a USB port on your PC.

## Running the software

1. Open [Thonny](https://thonny.org/)
2. Set the Interpreter in Thonny by: Menu Tools > Options > Interpreter tab > MicroPython (ESP32)
	![Thonny interpreter config](https://github.com/jcKarurosu/PuertaDigital/blob/80c16f2bb748203de4a7a5a559c7a55a0b3d94e6/T-Display-S3_R503_Sensor/Thonny_interprete.png)
3. At the lower right corner click on the menu and select MicroPython (ESP32) on your COM port (The port number could be different on your computer) In order to see the Micropython option here, your board has to be already connected to you PC.
	![Selecting Board MicroPython](https://github.com/jcKarurosu/PuertaDigital/blob/8ce96a8e7f4b7a91a6f0fc7d72dadc7cc567d57c/T-Display-S3_R503_Sensor/Select_Board.png)
4. On the top file explorer pane (left side of the screen) open the folder where you saved the files, then select all of them (3 files, and 1 folder with 1 file), rigth click and from the menu click on `Upload to / `
	![Uploading files to board](https://github.com/jcKarurosu/PuertaDigital/blob/8ce96a8e7f4b7a91a6f0fc7d72dadc7cc567d57c/T-Display-S3_R503_Sensor/Subir_archivos_a_tarjeta.png)
5. The files will be uploaded to the T-Display-S3 and will appear on the bottom file explorer pane. Double-click on the file main.py, you will see the code. Then Click on the `Run Script`  button (green arrow icon) or press `F5`.
6. Have fun
