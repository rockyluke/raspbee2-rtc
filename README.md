# raspbee2-rtc
RTC kernel module builder for RaspBee II

This repository provides a Makefile which downloads, builds and installs the RTC kernel module needed for the RaspBee II Zigbee shield on Raspberry Pi.

## Install

1. install dependencies
\
  <code> sudo apt install i2c-tools build-essential raspberrypi-kernel-headers </code>
2. clone or download this repository
3. <code>cd raspbee2-rtc</code>
4. <code>make</code>
5. <code>sudo make install</code>
6. Reboot

## Troubelshooting
If something went wrong during install please consider following error sources:

- install dependencies
- execute make without sudo
- execute make install with sudo
- if behind a proxy make sure it is correctly configured
 
 ## Use the RTC
 Set RTC time to system time:
 \
   <code>sudo hwclock --systohc</code>

 Read the RTC time:
 \
   <code>sudo hwclock</code>
\

 For more information see: https://linux.die.net/man/8/hwclock
   
## Dependecies
Hardware: \
RPI1 (Revision 2 or greater), RPI2, RPI3, RPI4 \
RaspBee II Zigbee shield
