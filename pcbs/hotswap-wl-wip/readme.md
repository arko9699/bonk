# Flashing

The following steps assume you have a PCB and the latest firmware downloaded

 Steps:
1. Plug in the PCB to the computer using an USB cable (either using uDB or directly)
2. Hold down button for approximately 10 seconds to enter bootloader.
3. Use [QMK Toolbox](https://qmk.fm/toolbox) on [Windows/Mac](https://docs.qmk.fm/newbs_flashing#flashing-your-keyboard-with-qmk-toolbox). Only CLI method is supported on [Linux](https://docs.qmk.fm/flashing#stm32-apm32-dfu).
4. The PCB should restart automatically after flashing and be ready to use.
5. Open [vial](https://vial.rocks/) in a USB HID supported browser (Chrome/Edge/Brave/Opera GX/Other Chromium based browsers) to modify your keymap.
