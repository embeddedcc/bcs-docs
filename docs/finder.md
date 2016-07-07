# BCS Finder

The BCS finder is a small utility which uses a UDP based locator protocol to find BCS devices on the local network.  It will only work if it is run from a computer on the same network as the BCS.

If the finder utility does not locate your BCS, you likely have an underlying networking problem that must be resolved.
  
Examples include:


- The BCS is not physically on the same network segment as your computer.
- Your network router is not supplying DHCP addresses to new clients on your network.
- Your network router is supplying DHCP addresses that are not defined on the same segment as the current settings of your computer.
- You have configured an incompatible static IP address in the BCS via the [Settings](settings.md) page.


## Download

* [BCS Finder for Mac](http://www.embeddedcc.com/finder/BCS%20Finder%20-%20Mac.zip)
* [BCS Finder for Windows (MSI Installer)](http://www.embeddedcc.com/finder/BCS%20Finder-1.0-win32.msi)
* [BCS Finder for Windows (Zip File)](http://www.embeddedcc.com/finder/BCS%20Finder.zip)

BCS Finder has been tested on Linux Mint running from the source code.  Please see the README for information on running under Linux.

## Source Code

The source code for BCS Finder is available on [GitHub](https://github.com/lawn-chair/bcs-finder).
