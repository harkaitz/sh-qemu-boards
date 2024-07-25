QEMU BOARD EMULATION SCRIPTS
============================

Scripts to launch images in emulated boards.

## Help

iso-raspberry

    Usage: iso-raspberry ...
    
    Download images to ${DDIR:-${TEMP:-/tmp}}.
    
    ... raspios/rpi{3,4}     : Download "img.xz". (user: pi, pass: raspberry)
    ... debian/12/rpi{2,3,4} : Download Debian 12 for RPI{2,3,4} (User:root)
    ... openbsd/7.4/rpi4     : Download OpenBSD 7.4 for RPI4.

lomount

    Usage: lomount [-v][-n NUM][-o OPTIONS] DRIVE [DIRECTORY]
    
    Mount the NUM'th partition in DRIVE image in DIRECTORY (by default /mnt).
    
    Dependencies: sudo(1), fdisk(1), mount(1).

qemu-h-rpi3

    Usage: qemu-h-rpi3 IMAGE QEMU-ARGS...
    
    Launch qemu emulating a Raspberry PI 3b+. This program uses lomount(1)
    to extract the kernel and the dtb file from the image.
    
    Known dtbs    : bcm2710-rpi-3-b-plus.dtb (raspios)
    Known kernels : kernel8.img
    SSH localhost port : 2222

## Collaborating

For making bug reports, feature requests and donations visit
one of the following links:

1. [gemini://harkadev.com/oss/](gemini://harkadev.com/oss/)
2. [https://harkadev.com/oss/](https://harkadev.com/oss/)
