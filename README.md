# mister-rtl8188-wifi
Wifi driver for RTL8188 for MiSTer 

Grab a fresh Ubuntu installation, it may be easier to create a VM using Virtualbox. 

`apt-get install gcc-arm-linux-gnueabihf build-essential bison flex libssl-dev`

```
make ARCH=arm mrproper && \
make ARCH=arm MiSTer_defconfig && \
make ARCH=arm CROSS_COMPILE=arm-linux-gnueabihf- EXTRAVERSION=-socfpga-r1 modules_prepare
```
