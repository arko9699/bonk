# bonk
A 13u row-staggered keyboard using MX switches and STM32F072 microcontroller running QMK firmware.
 
# PCB
![PCB_BACK](https://github.com/arko9699/bonk/blob/main/pcb_back.png)
[Supported Layouts](https://www.keyboard-layout-editor.com/#/gists/8eda360762dda6b66eb3a1510525a45f)

* Support for uDB or use the USB-C connector on the board [WARNING: Do not use both at the same time]
* Cutouts for Gummy O-ring mounts
NOTE : For cost saving, you may decide to forego the JST connector OR the USB-C and related components from the BOM.

# Building 
If you want to get a few of these PCBs to build yourself to share with friends head over to "Releases" and download the latest gerber files. Order from any PCB manufacturer of your choice however the included BOM and CPL is tailored to JLCPCB. A hot plate or hot air station is recommended to solder components yourself. 

# Opening the project
* Atleast KiCAD 8.0.7 is required to open the project properly. Older versions of KiCAD will not work.
* [marbastlib](https://github.com/ebastler/marbastlib) was used for some of the footprints.

# Bill of Materials
|LCSC #  |Description|Value         |Package |Amount|
|--------|-----------|--------------|--------|------|
|C15195  |Capacitor  |10nF          |0402    |1     |
|C1525   |Capacitor  |100nF         |0402    |4     |
|C15849  |Capacitor  |1uF           |0603    |3     |
|C19666  |Capacitor  |4.7uF         |0603    |2     |
|C23186  |Resistor   |5,1kΩ         |0603    |2     |
|C25804  |Resistor   |10kΩ          |0603    |1     |
|C269104 |Fuse       |500mA         |0805    |1     |
|C2988369|USB-C Port |              |SMD/THT |1     |
|C318884 |Push Button|TS-1187A      |SMD     |1     |
|C5180249|ESD Prot.  |USBLC6-2SC6   |SOT-23-6|1     |
|C81598  |Diode      |1N4148W       |SOD-123 |44    |
|C81720  |MCU        |STM32F072CBTx |LQFP-48 |1     |
|C5180249|Volt. Reg. |XC6206P332MR-G|SOT-23-3|1     |
|C160404 |Opt. JST   |SM04B-SRSS-TB |SMD     |1     |
