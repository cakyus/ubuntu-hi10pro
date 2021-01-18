# Ubuntu 20.04 on Chuwi Hi10Pro

## Features

| Feature | Status | Notes |
|-|-|-|
| Boot | Working | Out of the box. Automatically boot to ubuntu, no need to select device to boot. |
| Keyboard | Working | Out of the box. |
| Touchpad | Working | Out of the box. |
| Wifi | Working | Out of the box. |
| Graphics | Working | Out of the box. |
| Audio | Working | Out of the box. |
| Touchscreen | Not Working | |
| Accelerometer | Not Working | |

### Things To Do After Ubuntu Installation

 1. Rotate to landscape on boot. Settings > Displays > Orientation : Portait Left. This is useful as a quick temporary solution after installing ubuntu before you successfully configure accelerometer and screen rotation.
 2. Disable automatic screen lock. Settings > Screen Lock > Automatically  Screen Lock : Off.
 3. Large text. Settings > Universal Access > Large Text : On.

## Hardware

| Part | Model | Notes |
|-|-|-|
| CPU | Intel(R) Atom(TM) x5-Z8350 @1.44GHz | `/proc/cpuinfo` |
| Memory | 3.857 MB | `free -m` |
| Disk | 61.9 GB | `parted -l` |

## TODO

 1. Battery indicator is discharging when power cable is connected.
 2. Accelerometer `bmc150_accel_i2c i2c-BOSC0200:00: Invalid chip 3`.

## Installation

These are my installation steps.

 1. Download [Ubuntu 20.04.1 LTS](https://releases.ubuntu.com/20.04.1/ubuntu-20.04.1-desktop-amd64.iso)
 2. Write to USB. Assuming your usb device on /dev/sde `dd if=ubuntu-20.04.1-desktop-amd64.iso of=/dev/sde`.
 3. Insert the USB Device into a USB port on Chuwi.
 4. Press power button.
 5. Press `F7` repeatly until you see "Select device to boot".
 6. Choose your USB Device.
 7. Choose minimal installation.
 8. Choose erase disk and install ubuntu. WARNING: This will delete all files in disk.
 9. Continue until Ubuntu installation is complete.

## References

 1. https://github.com/danielotero/linux-on-hi10
 2. https://github.com/willyneutron/lubuntu_in_chuwi_Hi10Pro
 3. https://github.com/pk-personal/I1D6-C109S-Hi10Pro

