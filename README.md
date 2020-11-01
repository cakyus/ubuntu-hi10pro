# Ubuntu 20.04 on Chuwi Hi10Pro

## Features

| Feature | Status | Notes |
|-|-|-|
| Booting | Working | Out of the box. Automatically boot to ubuntu, no need to select device to boot. |
| Keyboard | Working | Out of the box. |
| Touchpad | Working | Out of the box. |
| Wifi | Working | Out of the box. |
| Graphics | Working | Out of the box. |

### Miscellaneous

#### TODO

 1. Rotate on boot

## Hardware

| Part | Model | Notes |
|-|-|-|
| CPU | - | - |
| Memory | - | - |
| Disk | - | - |

## Installation

 1. Download [Ubuntu 20.04.1 LTS](https://releases.ubuntu.com/20.04.1/ubuntu-20.04.1-desktop-amd64.iso)
 2. Write to USB. Assuming your usb device on /dev/sde `dd if=ubuntu-20.04.1-desktop-amd64.iso of=/dev/sde`.
 3. Insert the USB Device into a USB port on Chuwi.
 4. Press power button.
 5. Press `F7` repeatly until you see "Select device to boot shown"
 6. Choose your USB Device.
 7. Choose minimal installation.
 8. Continue until Ubuntu installation is complete.
