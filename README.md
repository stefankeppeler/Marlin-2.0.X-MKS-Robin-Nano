# Marlin Firmware adapted for the MKS Robin Nano 1.1/1.2


## Marlin 2.0<img align="right" width=175 src="buildroot/share/pixmaps/logo/marlin-250.png" />


Marlin 2.0 takes this popular RepRap firmware to the next level by adding support for much faster 32-bit and ARM-based boards while improving support for 8-bit AVR boards. Read about Marlin's decision to use a "Hardware Abstraction Layer" below.

Download earlier versions of Robin Nano Firmware on the [Releases page](https://github.com/le3tspeak/Marlin-2.0.X-Sapphire-PRO/releases).

## Building Marlin 2.0

To build Marlin 2.0 you'll need [PlatformIO](http://docs.platformio.org/en/latest/ide.html#platformio-ide). Detailed build and install instructions are posted at:

 
  - [Installing Marlin (VSCode)](http://marlinfw.org/docs/basics/install_platformio_vscode.html).

### Supported Platforms

  Platform|MCU| Board
  --------|---|-------
  [MKS Robin Nano](https://makerbase.com.cn/en/)|ARM® Cortex-M3 / STM32F103VET6| MKS Robin Nano 1.1 
  [MKS Robin Nano](https://makerbase.com.cn/en/)|ARM® Cortex-M3 / STM32F103VET6| MKS Robin Nano 1.2
  
### Features of the Configuration of Branch MKS Robin Nano

  Features|Active|Value
  --------|------|-----
  Fast Config Switch Sapphire Pro/Plus|True|Pro
  UI Type|-|Classic Marlin
  EEPROM|True|SDCARD EEPROM EMULATION
  G0 Support|True|-
  G2/G3 Arc Support|True|-
  Classic Jerk|False|-
  Bézier curve acceleration|True|-
  Junction Deviation|True|0.05
  Mesh Bed Leveling|True|-
  Filament sensor|True|-
  TMC UART|-|Ready
  TMC SPI|-|in progress
  TMC 2209 HW Serial|-|Ready
  Neopixel|-|Ready
  Cancel Objects|True|-


  Axes|Pro|Plus
  ----|----|----
  X|TMC2208 Standalone|TMC2208 Standalone
  Y|TMC2208 Standalone|TMC2208 Standalone
  Z|A4988|A4988
  E|A4988|TMC2208 Standalone

  Memory consumption|Value
  --------------------|-------------------------------------------
  RAM:    |56.4% (used 36944 bytes from 65536 bytes)
  Flash:  |42.6% (used 223380 bytes from 524288 bytes)

  
## Submitting Changes

- Please submit your questions and concerns to the [Issue Queue](https://github.com/le3tspeak/Marlin-2.0.X-MKS-Robin-Nano/issues).




## License

Marlin is published under the [GPL license](/LICENSE) because we believe in open development. The GPL comes with both rights and obligations. Whether you use Marlin firmware as the driver for your open or closed-source product, you must keep Marlin open, and you must provide your compatible Marlin source code to end users upon request. The most straightforward way to comply with the Marlin license is to make a fork of Marlin on Github, perform your modifications, and direct users to your modified fork.

While we can't prevent the use of this code in products (3D printers, CNC, etc.) that are closed source or crippled by a patent, we would prefer that you choose another firmware or, better yet, make your own.
