# Handy M0100: Wireless Speech-to-Text Mouse Firmware

This repository contains the firmware for the [Handy M0100](https://workshop.cjpais.com/projects/handy-m0100) project.

The Handy M0100 transforms a vintage 1985 Apple M0100 mouse into a wireless Bluetooth speech-to-text button for your computer.

**Learn more about the full project build, including hardware details, 3D models, and the backstory, on the official blog post:**

➡️ **[Handy M0100 Project Blog Post](https://workshop.cjpais.com/projects/handy-m0100)**

## Firmware Overview

*   Uses the [ZMK Firmware](https://zmk.dev/) for wireless connectivity (Bluetooth).
*   Designed for the [Seeed XIAO BLE nRF52840](https://www.seeedstudio.com/Seeed-XIAO-BLE-nRF52840-p-5201.html) microcontroller.
*   Configured to trigger a specific key combination (default: `Right Control + Right Meta`) when the mouse button is pressed.

## Getting Started (Flashing the Firmware)

1.  **Get the Firmware File:** Download the latest `.uf2` firmware file from the [GitHub Actions builds](https://github.com/cjpais/Handy-M0100-Firmware/actions/runs/14579988506) (look for the latest successful build and download the `firmware-uf2` artifact).
2.  **Connect the Xiao:** Plug your Seeed XIAO BLE nRF52840 into your computer via USB-C.
3.  **Enter Bootloader:** Double-click the tiny button on the Xiao board to put it into bootloader mode. A new drive (like `XIAO-BLE` or `RPI-RP2`) should appear on your computer.
4.  **Flash:** Drag and drop the downloaded `.uf2` file onto the new drive. The Xiao will automatically flash and reboot.

The mouse should now be ready to connect via Bluetooth to your computer. Press the mouse button to wake it up if it has gone to sleep.

## Customization

The keymap is defined in this repository. You can modify it or use tools like [ZMK Studio](https://zmk.studio/) to generate a custom `.uf2` file for your specific needs.

## Building the Hardware

Detailed instructions, parts lists, soldering information, and links to the 3D models for the custom baseplate or using the original PCB can be found in the main [Handy M0100 Blog Post](https://workshop.cjpais.com/projects/handy-m0100).

## Need Help?

If you have questions about the firmware or project, feel free to reach out!

📧 [cj@cjpais.com](mailto:cj@cjpais.com)
