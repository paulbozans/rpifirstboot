# rpifirstboot - Raspberry Pi Image Filesystem Expansion

This is the Raspberry Pi Image Filesystem Expansion project! This project focuses on enhancing the flexibility and usability of Raspberry Pi images by introducing an improved method for filesystem expansion, utilizing the new `raspberrypi-sys-mods/firstboot` option.

## Overview

The Raspberry Pi is a versatile and widely-used mini-computer that requires an operating system (OS) to be installed on an SD card. Often, these OS images are sized smaller than the SD card capacity. The new `raspberrypi-sys-mods/firstboot` option enables automatic expansion of the filesystem to utilize the full capacity of the SD card on the first boot. This feature is particularly useful for users who create custom Raspberry Pi images or deploy multiple Raspberry Pis with the same image.

## Key Features

- **Automated Filesystem Expansion:** On the first boot of the Raspberry Pi, the filesystem automatically expands, making full use of the SD card's available space.
- **Seamless Integration:** The `raspberrypi-sys-mods/firstboot` script integrates seamlessly into the boot process, requiring no manual intervention.
- **Customization and Flexibility:** This method offers greater control over the filesystem setup, allowing for custom partition layouts and configurations.
- **Improved User Experience:** New users or those deploying Raspberry Pis in volume will find this automated process reduces setup time and complexity.

## Getting Started

To use this feature, include the `raspberrypi-sys-mods/firstboot` script in your Raspberry Pi image. On the initial boot-up, the script will execute and automatically resize the filesystem. Detailed instructions on how to integrate and use this feature are provided in the subsequent sections.

## How to enable ?

```bash
cd ~ && rm -rf rpifirstboot && git clone https://github.com/paulbozans/rpifirstboot && sudo bash rpifirstboot/enable_firstboot

sudo halt
```

Obtain the image (Win32DiskImager for Windows) and transfer it onto a new SD card that has a larger capacity than the original source.
