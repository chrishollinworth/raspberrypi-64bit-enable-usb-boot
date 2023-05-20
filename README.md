1/ update eeprom with SD card with Raspberry PI OS and:
sudo apt update
sudo apt full-upgrade
reboot
sudo rpi-update
sudo rpi-eeprom-update
sudo rpi-eeprom-update -d -a


2/ change the boot order
With The last Rasberry Pi imager (version >= 1.6.2). Select misc Utility images>bootloader> USB Boot
boot RPI with this SD, green screen = update done

3/ Boot from Ubuntu on SSD (no more SD card in the port)


