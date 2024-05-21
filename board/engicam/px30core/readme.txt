Libre Computer Board ROC-RK3399-PC
===================================

Build:

  $ make engicam_px30_core_defconfig
  $ make

Files created in output directory
=================================

output/images

├── bl31.elf
├── idbloader.img
├── Image
├── px30-engicam-px30-core-ctouch2-of10.dtb
├── rootfs.ext2
├── rootfs.ext4 -> rootfs.ext2
├── rootfs.tar
├── sdcard.img
├── u-boot.bin
└── u-boot.itb

Creating bootable SD card:
==========================

Simply invoke (as root)

sudo dd if=output/images/sdcard.img of=/dev/sdX && sync

Where X is your SD card device

Serial console
--------------

Baudrate for this board is 115200

Wiki link:
https://wiki.amarulasolutions.com/bsp/rockchip/px30/px30.html
