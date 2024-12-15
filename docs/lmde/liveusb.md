# Live USB

Although most operating systems are available in .iso format, it is now common to write them to USB sticks, for speed and convenience and because many computers no longer have a CDROM drive.

There are many programs that can create live USB sticks from an .iso image. Follow the instructions on their pages to create them.

!!! danger
    The following steps include **formating** your USB stick, and **will** delete the files inside it. Please make sure to **backup** any important files in it before you continue.

## Ventoy

[ventoy](https://ventoy.net) is one of the best options and supports Windows and Linux. It has the advantage that once you create a USB stick, you can then add or remove .iso files by placing them in a subfolder without having to reload the stick.(:material-youtube: [related tutorial for](https://youtu.be/CuonyS3xdwg?t=125&si=_qxSIHNg0bgk9V9n))

## Windows

The following software runs on Windows and can create live USB sticks for any operating system:

- [Rufus](https://rufus.ie/) (:material-youtube: [related tutorial for
  lmde-6-cinnamon.iso](https://www.youtube.com/watch?v=UsJ6z3RMic8))
- [Easy2boot](https://www.easy2boot.com/)

## Linux
!!! note
    This will work with any distribution.

The following software runs on Linux and can create live USB sticks for any operating system:

- [Startup disk creator](https://linuxmint-installation-guide.readthedocs.io/en/latest/burn.html)
- [Unetbootin](https://fossbytes.com/create-bootable-usb-media-from-iso-ubuntu/)
- [dd](https://fossbytes.com/create-bootable-usb-media-from-iso-ubuntu/)

## LiveUSB

!!! warning
    This is really outdated, and not recommended to use.
<https://github.com/alkisg/liveusb> predates ventoy and also supports adding .iso by copy/paste. But it has no graphical interface and is not recommended to use it except in a few cases where the other methods don't work, for example if we want to boot.
[lmde-6-cinnamon-64bit.iso](https://repo.greeklug.gr/data/pub/linux/mint/iso/debian/lmde-6-cinnamon-64bit.iso) on a computer with UEFI.