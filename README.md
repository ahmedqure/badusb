# badusb
Raspberry pi pico badUSB
Overview
This project turns a Raspberry Pi Pico into a BadUSB device, similar to the Hak5 Rubber Ducky. The Pico, when connected to a target computer, acts as a keyboard and injects pre-programmed keystrokes to execute payloads automatically. This is useful for penetration testing, red teaming, and security research.

Features
Emulates a HID (Human Interface Device) keyboard
Executes predefined scripts upon plugging in
Supports DuckyScript, the language used by the original Rubber Ducky
Can be used for automated tasks, penetration testing, or educational security research
Works on Windows, Linux, and macOS

Hardware Required
Raspberry Pi Pico
Micro USB Cable

Software Requirements
MicroPython or CircuitPython
Pico-Ducky Firmware (based on DuckyScript)
Thonny IDE or Mu Editor (for programming the Pico)
Payload scripts (written in DuckyScript)

Setup Instructions
1. Install CircuitPython on Raspberry Pi Pico
Download the latest CircuitPython UF2 firmware for Raspberry Pi Pico from circuitpython.org.
Connect the Raspberry Pi Pico to your computer while holding the BOOTSEL button.
Drag and drop the UF2 file onto the mounted RPI-RP2 drive.
2. Install Required Libraries
Download the Adafruit HID Library from Adafruit GitHub.
Copy the adafruit_hid folder to the lib directory on the Pico.
3. Load a Payload
Create a new Python script (code.py) on the Pico.

Use DuckyScript syntax to define your payload.

4. Plug in and Test
Insert the Raspberry Pi Pico into a test system.
The script should execute automatically.

Payload Ideas
Open a reverse shell
Create a Wi-Fi password stealer
Download and execute scripts from the internet
Automate keyboard shortcuts for fun or productivity
VBS script
Keyboard/mouse interaction device to show online status for remote workers

Legal Disclaimer
This project is intended for educational and ethical penetration testing purposes only. Unauthorized use of this tool on systems without permission is illegal. The author is not responsible for misuse.

