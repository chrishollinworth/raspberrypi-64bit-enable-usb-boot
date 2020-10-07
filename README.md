# raspberrypi-64bit-enable-usb-boot

0. Download 64bit image (lite image) https://downloads.raspberrypi.org/raspios_lite_arm64/images/raspios_lite_arm64-2020-08-24/

1. Use balenaEtcher to put image onto sd card

2. Install SD card in pi 4

3. Check Existing firmware version
```
vcgencmd bootloader_version
Mar 19 2020 14:27:25
version 940f978d13e45be9baef77f3f4a13b76a832f7b4 (release)
timestamp 1584628045
```
4. Update to get new firmware (rpi-eeprom)
```
 sudo apt update
 sudo apt-get dist-upgrade -y
```
5. Check Firmware
```
vcgencmd bootloader_version
Mar 19 2020 14:27:25
version 940f978d13e45be9baef77f3f4a13b76a832f7b4 (release)
timestamp 1584628045
```
6. Reboot to install new firmware
```
shutdown now -r 
```
7. Confirm new firmware version
```
vcgencmd bootloader_version
Sep  3 2020 13:11:43
version c305221a6d7e532693cc7ff57fddfc8649def167 (release)
timestamp 1599135103
```
8. Turn off pi
```
shutdown now
```
9. Unplug sdcard
10. Use balenaEtcher to put image onto USB SSD/HDD
11. Plug in ssd/hdd with raspbian image and boot!



