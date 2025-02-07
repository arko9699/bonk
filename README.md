# bonk
A 13u "WKL-like" row-staggered keyboard using MX switches and STM32F072 microcontroller, running QMK firmware.
 
# PCB
![PCB_BACK](https://github.com/arko9699/bonk/blob/main/pcb_back.png)

# Supported Layouts
![Supported Layouts](https://github.com/arko9699/bonk/blob/main/layouts.png)

* Support for uDB or use the USB-C connector on the board [WARNING: Do not use both at the same time]
* Cutouts for Gummy O-ring mounts

# Pics
![](https://github.com/arko9699/bonk/blob/main/assets/pic1-by-source.jpg)

![](https://github.com/arko9699/bonk/blob/main/assets/pic1-by-arko.png)

# Building 
If you want to get a few of these PCBs to build yourself or share with friends, head over to "Releases" and download the latest gerber files. Order from any PCB manufacturer of your choice however the included BOM and CPL are tailored for JLCPCB. A hot plate or hot air station is recommended to solder components yourself. 
NOTE : For cost saving, either the JST connector OR the USB-C and related components may be omitted from the BOM.

# Opening the project
* Atleast KiCAD 8.0.7 is required to open the project properly. Older versions of KiCAD will not work.
* [marbastlib](https://github.com/ebastler/marbastlib) was used for some of the footprints.

# Bill of Materials
rev1.0
|LCSC #  |Description|Value         |Package |Amount|
|--------|-----------|--------------|--------|------|
|C15195  |Capacitor  |10nF          |0402    |1     |
|C1525   |Capacitor  |100nF         |0402    |4     |
|C15849  |Capacitor  |1uF           |0603    |3     |
|C19666  |Capacitor  |4.7uF         |0603    |2     |
|C23186  |Resistor   |5.1kΩ         |0603    |2     |
|C25804  |Resistor   |10kΩ          |0603    |1     |
|C269104 |Fuse       |500mA         |0805    |1     |
|C2988369|USB-C Port |USB-7010ASV   |SMD/THT |1     |
|C318884 |Push Button|TS-1187A      |SMD     |1     |
|C5180249|ESD Prot.  |USBLC6-2SC6   |SOT-23-6|1     |
|C81598  |Diode      |1N4148W       |SOD-123 |44    |
|C81720  |MCU        |STM32F072CBTx |LQFP-48 |1     |
|C5180249|Volt. Regu.|XC6206P332MR-G|SOT-23-3|1     |
|C160404 |Opt. JST   |SM04B-SRSS-TB |SMD     |1     |

rev1.1
|LCSC #  |Description|Value         |Package |Amount|
|--------|-----------|--------------|--------|------|
|C15195  |Capacitor  |10nF          |0402    |1     |
|C1525   |Capacitor  |100nF         |0402    |4     |
|C15849  |Capacitor  |1uF           |0603    |3     |
|C19666  |Capacitor  |4.7uF         |0603    |2     |
|C25076  |Resistor   |100Ω          |0402    |1     |
|C21190  |Resistor   |1k Ω          |0603    |1     | -> Added in rev1.1
|C23186  |Resistor   |5.1kΩ         |0603    |2     | 
|C25804  |Resistor   |10kΩ          |0603    |1     | -> Added in rev1.1
|C17629  |Resistor   |330kΩ         |0805    |1     | -> Added in rev1.1
|C17629  |Resistor   |1MΩ           |0805    |1     | -> Added in rev1.1
|C269104 |Fuse       |500mA         |0805    |1     |
|C2988369|USB-C Port |USB-7010ASV   |SMD/THT |1     |
|C318884 |Push Button|TS-1187A      |SMD     |1     |
|C5180249|ESD Prot.  |USBLC6-2SC6   |SOT-23-6|1     |
|C81598  |Diode      |1N4148W       |SOD-123 |45    | -> Additional diode added in rev1.1
|C81720  |MCU        |STM32F072CBTx |LQFP-48 |1     |
|C8545   |MOSFET     |2N7002        |SOT-23  |1     | -> Added in rev1.1
|C5180249|Volt. Regu.|XC6206P332MR-G|SOT-23-3|1     |
|C160404 |Opt. JST   |SM04B-SRSS-TB |SMD     |1     |

# Changelog
* rev1.1
  - Changed reset/boot circuitry. Now there is only one button for both actions. Hold the buttom for ~30s to enter the bootloader for flashing, or quickly press and release to reset the board. Thanks to the [Acheron Project](https://acheronproject.com/reset_article_1/reset_article_1/) by Gondolindrim and others. This change adds additional components to the BoM but requires less than $1 extra for all parts.
  - Added new compiled firmware which enables a few more QMK features. This is backwards compatible with the older revision of the board.
* rev1.0
  - Initial release
