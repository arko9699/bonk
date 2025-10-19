# bonk
A 13u "WKL-like" row-staggered keyboard using MX switches and STM32F072 microcontroller, running QMK firmware.
 
* Support for uDB or use the USB-C connector on the board [WARNING: Do not use both at the same time]
* Cutouts for Gummy O-ring mounts
* ISO/ANSI Enter [added in rev2]

# Pics
![](https://github.com/arko9699/bonk/blob/main/assets/pic1-by-source.jpg)

# Building 
If you want to get a few of these PCBs to build yourself or share with friends, head over to "Releases" and download the latest gerber files. Order from any PCB manufacturer of your choice however the included BOM and CPL are tailored for JLCPCB. A hot plate or hot air station is recommended to solder components yourself. 
NOTE : For cost saving, either the JST connector OR the USB-C and related components may be omitted from the BOM.

# Changelog
* rev2
  - Expanded layout options including ISO Enter, more flexible Split Left Shift, new 3u spacebar option. 7u spacebar layout has been removed due to lack of usability and its presence as more of a gimmick.
* rev1.1
  - Changed reset/boot circuitry. Now there is only one button for both actions. Hold the buttom for ~30s to enter the bootloader for flashing, or quickly press and release to reset the board. Thanks to the [Acheron Project](https://acheronproject.com/reset_article_1/reset_article_1/) by Gondolindrim and others. This change adds additional components to the BoM but requires less than $1 extra for all parts.
  - Added new compiled firmware which enables a few more QMK features. This is backwards compatible with the older revision of the board.
* rev1.0
  - Initial release
