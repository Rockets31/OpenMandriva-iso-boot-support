# OpenMandriva iso-boot support
Directly boot & install OpenMandriva from Official OpenMandriva Installation Media using grub2 without burning to usb-drive.

# Features
- Filesystems: exfat, ext4
- Provide boot menu
- Supported ISOs: Openmandriva Live Media Rock-6.0 & Rome20260927.4765 releases.

# Usage
Load provided 'om-rock6.img' or 'om-rome2609.img' file along with the main 'initrd' of the installation media via grub loopback module.
If you are using 'https://github.com/Mexit/MultiOS-USB', it is just a few steps:

0. Use MultiOS-USB partition on 'exfat' or 'ext4' filesystem.
1. Copy your OpenMandriva-iso files to 'ISOs' directory.
2. Create a directory for 'grub.cfg' files: '/MultiOS-USB/config_priv/openmandriva-sc'
3. Copy 'om-rock6.img', 'om-rome2609.img', 'openmandriva-Rock6-live.cfg' & 'openmandriva-Rome2609-live.cfg' over there.
4. Reboot into 'MultiOS-USB' and start e.g. 'openmandriva-6.0-plasma6-x11.x86_64.iso [scandev]' entry.
6. Installer will start same way as from a usb-stick.
