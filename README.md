 Introduction

This is a first attempt at a basic Fedora ARM Image Installer ( Downloader / Creator / Updater ). This script is written in Python (version 2 & 3 compatible) and makes use of the PyQt4 GUI module allowing it to run graphically (on both Linux & Windows). The files written are block device image files containing: [MBR + Partitions + File Systems + Data]. Distributors should make sure to package some sort of first-boot setup-script to customize the operating system as there is no official installer for ARM devices yet. Hopefully this application will be able to create bootable media for almost any generalized Guruplug, Efika, Pandaboard, Trimslice, or Raspberry Pi device type.
Usage

    Select a source file or download option (click the refresh button first)
        A source file must be either a raw image or zip archive
        The download option will prompt you to select a download destination folder first 
    Select the destination (target) device drive where the image should be written
    Click install 

Notes

    Storage devices that are greater than 32 Gigabytes in size are ignored (to temporarily protect users)
    You must have enough space in your temp directories to download or extract any source file
    The Windows version makes use of a pre-packaged dd.exe binary program to help write image files to block devices
        http://www.chrysocome.net/dd 

Known Bugs

    This version currently only works with English languages, I haven't had the chance to make it multi-lingual yet 


for more information and screenshots please go to original source wiki:

www.fedoraproject.org/wiki/Fedora_ARM_Installer
