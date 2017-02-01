# BCS Documentation

Welcome to the user guide for the BCS series brewery controllers. Use the navigation menu on the left to find the topic in which you are interested. This page contains some basic setup information and links to some helpful resources.

The BCS documentation is basically setup to correspond to the screens available in the BCS web interface. Those screens are:


-  [Main Control](main_control.md)
-  [Data Log](data_log.md)
-  [Process Editor](process_editor.md)
-  [Temp Adjust](temp_adjust.md)
-  [Ladder Logic](ladder_logic.md)
-  [Settings](settings.md)

In addition, there are pages to help you better understand the [User Interface](ui.md), the [BCS Finder](finder.md) application, and the  [Online Utilities](utilities.md).

## Setup

The BCS should be connected via Ethernet cable to your network.  It is configured by default to obtain an IP address via [DHCP](http://en.wikipedia.org/wiki/Dynamic_Host_Configuration_Protocol) from your router.  The [BCS Finder](finder.md) will help locate the BCS on your network. Depending on your router, you may also be able to locate the IP address given to your BCS in your router interface. It may be helpful the know the MAC address of your BCS which is printed on the BCS case.

It is highly recommended to create a DHCP reservation on your router so the BCS will always have the same IP address.  This setup is specific to each individual router, please check the manual for your router to learn how to set up a DHCP reservation. If the BCS is unable to lease a DHCP address, it will default to the 169.254.0.63 IP address. 

Another option is to assign your BCS an IP address that is outside of your router's DHCP address pool. For more information on configuring a static IP address on your BCS, see [Settings](settings.md).

## Accessing the BCS

The BCS has no physical display and is normally accessed through the web interface. Once you discover the IP address of your BCS, you can just enter the BCS IP address in your favorite web browser to access the [BCS Interface](ui.md).

### Accessing the BCS Remotely

Entering the local IP address of the BCS in your browser only works for accessing the BCS interface when you are on the same local area network as the BCS. If you want to access the BCS from a remote location, some additional configuration is required. 
#### Port Forwarding
One option for accessing the BCS is to use [port forwarding](https://en.wikipedia.org/wiki/Port_forwarding). See your router documentation on how to configure port forwarding. Basically, port forwarding allows you to access your BCS using your public IP address on the WAN port of your router. This IP address is assigned by your ISP and is subject to change periodically. The router will translate the request coming in from the Internet to a host on the inside of your network, your BCS in this case. You can locate your public IP address by looking at your router configuration or by using an web site such as [What is My IP Address](http://whatismyipaddress.com/). Use port forwarding with caution since it does open a hole in your firewall/router and your BCS could easily be compromised by a denial of service attack resulting in unpredictable behavior.

For more information on setting your BCS IP address and port number, please see [Settings](settings.md).

#### Dynamic DNS
Since your public IP address is usually not static, this can cause frustration when trying to access your BCS remotely. A possible solution to this problem is to use a dynamic DNS service. This service provides you with a URL that never changes and that URL automatically goes to your public IP address, even if it changes. Embedded Control Concepts does support or endorse any dynamic DNS service, but one example is [DynDNS](http://dyn.com/remote-access/).