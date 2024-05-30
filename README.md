# LVGL ported to ESP32-S3-LCD-EV-Board

## Overview

This is LVGL ported to [ESP32-S3-LCD-EV-Board](https://github.com/espressif/esp-bsp/tree/master/bsp/esp32_s3_lcd_ev_board) with using Espressif [BSP](https://github.com/espressif/esp-bsp). This example shows LVGL music demo.

| <div align=center><img src="https://docs.espressif.com/projects/esp-dev-kits/zh_CN/latest/_images/ESP32-S3-LCD-EV-Board_800x480.png" width=400/></div> | <div align=center><img src="https://docs.espressif.com/projects/esp-dev-kits/zh_CN/latest/_images/ESP32-S3-LCD-EV-Board_480x480.png" width=400/></div> |
| :----: | :----: |

## Buy

You can purchase ESP32-S3-LCD-EV-Board from [MOUSER](https://mou.sr/4aFdj07) or [Official shop on AliExpress](https://www.aliexpress.com/item/1005005720726421.html).

## Benchmark

You can find more about performance in [BSP repository](https://github.com/espressif/esp-bsp/blob/master/components/esp_lvgl_port/docs/performance.md).

## Specification

### CPU and Memory
- **MCU:** ESP32-S3
- **RAM:** 512 KB internal SRAM,  8/16 MB external PSRAM
- **Flash:** 2/4/8/16 MB

### Display and Touch
- **Resolution:** 800x480 / 480x480
- **Display Size:** 4.3" / 3.95"
- **Interface:** RGB LCD
- **Color Depth:** 24-bit
- **Touch Pad:** Capacitive (GT1151/FT5x06)

### Connectivity
- Onboard audio codec + audio amplifier
- Onboard dual microphone pickup
- USB type-C interface download and debugging

## Getting started

### Hardware setup
- Connect the display (480x480 or 800x480)
- Connect USB-C (marked as UART) to PC
- [Board User Guide](https://docs.espressif.com/projects/esp-dev-kits/en/latest/esp32s3/esp32-s3-lcd-ev-board/user_guide.html)

### Software setup
- Prepare environment for compiling ESP-IDF - follow this [guide](https://docs.espressif.com/projects/esp-idf/en/latest/esp32/get-started/index.html).

### Run the project
- Clone this repository
- Select screen size in `menuconfig` (default is 800x480):
```
idf.py menuconfig
```
Component config --> Board Support Package --> LCD --> Select Target Sub board

- Compile and flash
```
idf.py -p COMx flash monitor
```

## Contribution and Support

If you find any issues with the development board feel free to open an Issue in this repository. For LVGL related issues (features, bugs, etc) please use the main [lvgl repository](https://github.com/lvgl/lvgl).

If you found a bug and found a solution too please send a Pull request. If you are new to Pull requests refer to [Our Guide](https://docs.lvgl.io/master/CONTRIBUTING.html#pull-request) to learn the basics.

