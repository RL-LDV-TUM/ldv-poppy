# Ethernet

Poppy is configured to obtain a IP adress via DHCP when he is connected to the lrz network with an ethernet cable.
The DNS Service [poppy.clients.ldv.ei.tum.de](http://poppy.clients.ldv.ei.tum.de) is configured only for Wifi connections to the LDV-CPP network bridge.

# Wifi
Poppy automatically connects to the Wifi SSID: **LDV-CPP**

The LDV-CPP accesspoints work in bridge-mode so Poppy can be reached by: [poppy.clients.ldv.ei.tum.de](http://poppy.clients.ldv.ei.tum.de) 
This only works when the accesspoint is connected to the lrz network. 

    # interfaces(5) file used by ifup(8) and ifdown(8)
    # Include files from /etc/network/interfaces.d:
    source-directory /etc/network/interfaces.d
    
    auto eth2
    iface eth2 inet dhcp
    
    iface default inet dhcp
    
    auto lo
    iface lo inet loopback
    
    auto wlan2
    iface wlan2 inet dhcp
            wpa-ssid "LDV-CPP"
            wpa-psk "*******"
    
    allow-hotplug wlan2 eth2
