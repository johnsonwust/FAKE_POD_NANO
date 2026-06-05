# FAKE_POD_NANO

# FAKE POD NANO Lossless Audio Player

**FAKE POD NANO** is a compact, open-source hardware audio player built around the **ESP32-S3** platform and a square **AMOLED display**. The project is inspired by the look and feel of the iPod Nano, while focusing on DIY-friendly hardware, portable playback, and support for high-resolution local audio files.

The player supports **MP3** and **FLAC** playback, with audio specifications listed by the original project as up to **96 kHz sampling rate** and **24-bit bit depth**.

## Project Highlights

* **ESP32-S3-based design** for embedded audio playback and user-interface control
* **Square AMOLED display** for a compact, modern visual interface
* **iPod Nano-inspired enclosure and appearance**
* **MP3 and FLAC playback support**
* **High-resolution audio support** up to 96 kHz / 24-bit, according to the original project description
* **Two firmware hardware targets** are provided: CS43131 and PCM5102 versions
* **TF card content package** is provided for preparing the storage card
* **3D-printable enclosure files** are included for the main body and side cover
* **Estimated reproduction cost:** approximately ¥140, as listed on the original OSHWHub page

## Hardware Overview

The project is intended as a small standalone music player. The publicly listed project information identifies the main platform as **ESP32-S3** and the display as a square **AMOLED** screen. The available firmware packages indicate support for builds targeting **CS43131** and **PCM5102** audio-output configurations.

Because the OSHWHub page currently does not provide a full BOM preview, builders should refer to the included component-purchase spreadsheet and verify all parts before fabrication or assembly.

## Available Project Resources

The OSHWHub project page provides several downloadable resources, including:

| Category                     | File / Resource                                | Purpose                                                                                 |
| ---------------------------- | ---------------------------------------------- | --------------------------------------------------------------------------------------- |
| Component reference          | `部分零件购买链接.xlsx`                                | Reference links for purchasing selected parts                                           |
| Source / development package | `ESP32S3-IDF_AMOLED_LVGL-V8.zip`               | ESP32-S3 firmware/project package based on ESP-IDF, AMOLED display support, and LVGL V8 |
| 3D enclosure                 | `右侧盖板.stl`                                     | Right-side cover model                                                                  |
| 3D enclosure                 | `本体卡得紧的版本.stl`                                 | Main body model with a tighter fit                                                      |
| 3D enclosure                 | `本体容易安装版.stl`                                  | Main body model designed for easier installation                                        |
| Media tool                   | `MJPEG转换工具.zip`                                | MJPEG conversion utility                                                                |
| Flashing tool                | `NIGHT7_FLASH_TOOL.zip`                        | Firmware flashing tool package                                                          |
| Firmware                     | `固件_CS43131版_V1.0.0.zip`                       | Firmware package for the CS43131 version                                                |
| Firmware                     | `固件_PCM5102版_v1.0.0.zip`                       | Firmware package for the PCM5102 version                                                |
| TF card package              | `TF卡内容_j解压后拷贝到TF卡根目录.zip`                      | Files to extract and copy to the TF card root directory                                 |
| Firmware                     | `固件cs43131_1.1.2_播放器版_单文件.zip`                 | Single-file player firmware for CS43131 version                                         |
| Firmware                     | `固件pcm5102_1.1.2_播放器版_单文件.zip`                 | Single-file player firmware for PCM5102 version                                         |
| UAC firmware                 | `固件CS43131_UAC单功能版_0x10000_可用蓝牙OTA更新此文件.bin`   | CS43131 UAC-focused firmware binary, marked as usable for Bluetooth OTA update          |
| UAC firmware                 | `固件PCM5102_UAC单功能版_0x10000_可用蓝牙OTA更新此文件.bin`   | PCM5102 UAC-focused firmware binary, marked as usable for Bluetooth OTA update          |
| OTA firmware                 | `PROJECT_N7_IDF_PCM5102_1.3.2_0x10000_ota.bin` | OTA firmware binary for the PCM5102 version                                             |
| OTA firmware                 | `PROJECT_N7_IDF_CS43131_1.3.2_0x10000_ota.bin` | OTA firmware binary for the CS43131 version                                             |

## Getting Started

1. **Open or clone the project** from the OSHWHub project page.
2. **Review the hardware files** and the component-purchase spreadsheet before ordering parts.
3. **Manufacture the PCB** using the provided design files from the OSHWHub project.
4. **Print the enclosure** using the provided STL files. Choose either the tighter-fit body or the easier-installation body depending on your assembly preference.
5. **Assemble the hardware**, including the ESP32-S3 board, AMOLED display, audio-output circuit, controls, storage, and enclosure parts.
6. **Flash the matching firmware** for your hardware version:

   * Use the CS43131 firmware if your build uses the CS43131 audio configuration.
   * Use the PCM5102 firmware if your build uses the PCM5102 audio configuration.
7. **Prepare the TF card** by extracting the provided TF-card package and copying its contents to the root directory of the card.
8. **Test playback** with MP3 and FLAC files before final enclosure assembly.

## Firmware Notes

The available downloads suggest multiple firmware paths:

* Standard player firmware packages for both **CS43131** and **PCM5102** versions
* Single-file player firmware builds
* UAC-focused firmware binaries
* OTA update binaries for newer project builds

Before flashing, confirm that the firmware file matches your exact hardware version. Flashing the wrong firmware may cause the device to fail to boot or behave incorrectly.

## License

This project is released under the **CC BY-NC-SA 3.0** license as listed on the original OSHWHub page.

That means the project may be shared and adapted with attribution, but it is restricted to non-commercial use and derivative works must be shared under compatible terms. Always refer to the original license text for the complete legal terms.

## Reproduction Notice

The original platform page states that this is an open-source hardware project intended for learning, communication, and research. It is not intended for commercial sale or other profit-making use. Builders should independently verify the circuit, parts, firmware, and mechanical files before reproducing the project.

## Credits

* Original project: **FAKE_POD_NANO 无损音频播放器**
* Project author/member listed on OSHWHub: **萨纳兰的黄昏**
* Source platform: **OSHWHub / 立创开源硬件平台**
