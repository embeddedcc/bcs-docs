# BCS Finder

The BCS finder is a small utility which uses a UDP based locator protocol to find BCS devices on the local network.  It will only work if it is run from a computer on the same network as the BCS.

If the finder utility does not locate your BCS, you likely have an underlying networking problem that must be resolved.
  
Examples include:


- The BCS is not physically on the same network segment as your computer.
- Your network router is not supplying DHCP addresses to new clients on your network.
- Your network router is supplying DHCP addresses that are not defined on the same segment as the current settings of your computer.
- You have configured an incompatible static IP address in the BCS via the [Settings](settings.md) page.


## Download

* [BCS Finder for Mac](https://www.dropbox.com/s/7n8nh66sl6pjm9q/BCS%20Finder%20-%20Mac.zip?dl=0)
* [BCS Finder for Windows (MSI Installer)](https://www.dropbox.com/s/7mh5kpm3xabnnp5/BCS%20Finder-1.0-win32.msi?dl=0)
* [BCS Finder for Windows (Zip File)](https://www.dropbox.com/s/5w8teos0x7gg9lo/BCS%20Finder.zip?dl=0)

BCS Finder has been tested on Linux Mint running from the source code.  Please see the README for information on running under Linux.

## Source Code

The source code for BCS Finder is available on [GitHub](https://github.com/lawn-chair/bcs-finder).
