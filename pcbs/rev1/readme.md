# PCB
![PCB](https://github.com/arko9699/bonk/blob/main/assets/rev1.png)

# Supported Layouts
![Supported Layouts](https://github.com/arko9699/bonk/blob/main/assets/rev1-layouts.png)

# Opening the project
* Atleast KiCAD 8.0.7 is required to open the project properly. Older versions of KiCAD will not work.
* [marbastlib](https://github.com/ebastler/marbastlib) was used for some of the footprints.

# Bill of Materials
|LCSC #  |Description|Value         |Package |Amount|Comments                        |
|--------|-----------|--------------|--------|------|--------------------------------|
|C15195  |Capacitor  |10nF          |0402    |1     |                                |
|C1525   |Capacitor  |100nF         |0402    |4     |                                |
|C15849  |Capacitor  |1uF           |0603    |3     |                                |
|C19666  |Capacitor  |4.7uF         |0603    |2     |                                |
|C25076  |Resistor   |100Ω          |0402    |1     |                                |
|C21190  |Resistor   |1k Ω          |0603    |1     |Added in rev1.1                 |
|C23186  |Resistor   |5.1kΩ         |0603    |2     |                                |
|C25804  |Resistor   |10kΩ          |0603    |1     |Added in rev1.1                 |
|C17629  |Resistor   |330kΩ         |0805    |1     |Added in rev1.1                 |
|C17629  |Resistor   |1MΩ           |0805    |1     |Added in rev1.1                 |
|C269104 |Fuse       |500mA         |0805    |1     |                                |
|C2988369|USB-C Port |USB-7010ASV   |SMD/THT |1     |                                |
|C318884 |Push Button|TS-1187A      |SMD     |1     |                                |
|C5180249|ESD Prot.  |USBLC6-2SC6   |SOT-23-6|1     |                                |
|C81598  |Diode      |1N4148W       |SOD-123 |45    |Additional diode added in rev1.1|
|C81720  |MCU        |STM32F072CBTx |LQFP-48 |1     |                                |
|C8545   |MOSFET     |2N7002        |SOT-23  |1     |Added in rev1.1                 |
|C5180249|Volt. Regu.|XC6206P332MR-G|SOT-23-3|1     |                                |
|C160404 |Opt. JST   |SM04B-SRSS-TB |SMD     |1     |                                | 

# Flashing
The following steps assume you have a PCB and the latest rev1.x firmware downloaded.

Common Steps:
1. Plug in the PCB to the computer using an USB cable (either using uDB or directly)
2. Hold down button for approximately 30 seconds to enter bootloader.
3. Use [QMK Toolbox](https://qmk.fm/toolbox) on [Windows/Mac](https://docs.qmk.fm/newbs_flashing#flashing-your-keyboard-with-qmk-toolbox). Only CLI method is supported on [Linux](https://docs.qmk.fm/flashing#stm32-apm32-dfu).
4. The PCB should restart automatically after flashing and be ready to use.
5. Open [vial](https://vial.rocks/) in a USB HID supported browser (Chrome/Edge/Brave etc.) to modify your keymap.
