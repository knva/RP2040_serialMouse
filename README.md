# README: Controlling RP2040 Development Board via Arduino

This guide will walk you through the process of connecting an RP2040 development board, compiling a program using Arduino, and utilizing serial communication to control the board. Specifically, you will be able to send commands to trigger actions such as mouse clicks and relative cursor movement.

## Table of Contents

- [Introduction](#introduction)
- [Requirements](#requirements)
- [Instructions](#instructions)
  - [1. Connecting the RP2040 Board](#1-connecting-the-rp2040-board)
  - [2. Compiling and Uploading the Program](#2-compiling-and-uploading-the-program)
  - [3. Opening the Serial Connection](#3-opening-the-serial-connection)
  - [4. Sending Commands](#4-sending-commands)
- [Commands](#commands)
- [Contributing](#contributing)
- [License](#license)

## Introduction

This guide provides step-by-step instructions for interacting with an RP2040 development board using the Arduino IDE. You'll be able to compile and upload programs to the board and establish a serial connection to send commands that trigger various actions, including mouse clicks and relative cursor movement.

## Requirements

To follow this guide, you'll need:

- An RP2040 development board
- USB cable for connecting the board to your computer
- Arduino IDE installed on your computer
- Basic familiarity with the Arduino IDE and C++ programming

## Instructions

### 1. Connecting the RP2040 Board

Connect the RP2040 development board to your computer using a USB cable. Make sure the board is properly powered and detected by your computer.

### 2. Compiling and Uploading the Program

1. Launch the Arduino IDE.
2. Open the provided Arduino program.
3. Select the appropriate board from the "Tools" menu.
4. Click the "Upload" button to compile and upload the program to the RP2040 board.

### 3. Opening the Serial Connection

1. In the Arduino IDE, open the Serial Monitor.
2. Choose the correct baud rate in the bottom-right corner.
3. The Serial Monitor should display the board's output.

### 4. Sending Commands

You can now send commands to the RP2040 board via the Serial Monitor. Use the following commands:

- **"shoot"**: Triggers a left mouse click.
- **"100:200"**: Moves the cursor 100 pixels to the right and 200 pixels down (relative movement).

Remember, the RP2040 board interprets these commands, so make sure they are sent accurately.

## Commands

Here are the supported commands you can send via the Serial Monitor:

- **"shoot"**: Initiates a left mouse click action.
- **"[x]:[y]"**: Moves the cursor relative to its current position. Replace `[x]` with the desired horizontal movement and `[y]` with the desired vertical movement.

## Contributing

If you find any issues or have suggestions for improvement, feel free to contribute by opening an issue or submitting a pull request on the project's GitHub repository.

## License

This project is licensed under the [MIT License](LICENSE). Feel free to use and modify the code as needed.
