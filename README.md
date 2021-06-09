# fiberhomesuperadmin

By default the PLDT HOME FIBR AN5506-04-FA RP2627 comes only with limited settings.

The following walkthrough consists of opening the device and enabling the advanced settings using the device serial console to enable access to the admin account on the web interface.

## Disclaimer

This will void your device ISP warranty. Any modification done to your device comes with no guarantee.

We have no responsibility to any damage that can happen to any of your devices. **Mod at your own risk**.

## Walkthrough

Guides on accessing the router's advanced settings

[PLDT Home Fiber router hacking](https://kleo.github.io/pldt-home-fiber-router-hacking)<br>
[PLDT Home Fiber router console access](https://kleo.github.io/pldt-home-fiber-router-console-access)<br>
[PLDT Home Fiber router firmware and files](https://kleo.github.io/pldt-home-fiber-router-firmware-and-files)<br>
[PLDT Home Fiber router web interface admin access](https://kleo.github.io/pldt-home-fiber-web-interface-admin-access)

## Frequently Asked Questions

### How to activate LAN PORTS 2-4 / Remove ethernet isolation?

1. Gain admin access

Guide: https://kleo.github.io/pldt-home-fiber-web-interface-admin-access

2. On the web interface, Network > BroadBand Settings > Internet Settings

Check all the boxes on: LAN Binding, 2.4G SSID Binding and 5G SSID Binding

Reference: https://kleo.github.io/img/2018-09-09/01.png

### Origin

Gist: https://gist.github.com/kleo/de3b1610b1879f8e92966ba106f83f97

### Discord

Backspace https://discord.gg/C43625u

### Hidden URLs

The URLs were usable from version RP2616 and lower but as of firmware RP2627 update the URLs below are now restricted and will redirect back to the login page. [Reference](https://kleo.github.io/pldt-home-fiber-router-hacking)

<details>
    <summary>AN5506-04-FA RP2616</summary>

    Hidden from the web interface are the rest of the router's capabilities and advanced settings.

    We just need to enter the right url for the settings you're looking for.

    We need to be logged in before we can do anything else, use your defined password if you already set the admin password.

    Note that you have to log in again if you're idle for a few minutes on the web interface.


        username: admin
        password: 1234

        http://192.168.1.1/application/ddns.asp		            # Configure DDNS
        http://192.168.1.1/application/dlna.asp                         # Enable or disable DLNA service
        http://192.168.1.1/application/dmz.asp			    # Set host IP to DMZ
        http://192.168.1.1/application/multi_nat.asp                    # Configure Multi NAT
        http://192.168.1.1/application/samba.asp                        # Enable or disable samba service
        http://192.168.1.1/application/ping_diagnosis.asp	            # Network diagnosis. Ping and Traceroute
        http://192.168.1.1/application/port_forwarding.asp              # Configure port forwarding
        http://192.168.1.1/application/port_trigger.asp                 # Configure port trigger
        http://192.168.1.1/application/redirect.asp		            # blank
        http://192.168.1.1/application/upnp.asp			    # Configure UPnP enable/disable

        http://192.168.1.1/help/

        http://192.168.1.1/internet/dhcp_macband.asp                    # blank
        http://192.168.1.1/internet/dhcp_portband.asp                   # blank
        http://192.168.1.1/internet/dhcp_service.asp		    # Enable/disable DHCP functions, configure parameters
        http://192.168.1.1/internet/dhcpv6_portband.asp                 # blank
        http://192.168.1.1/internet/dhcp_userlist.asp		    # Display information about DHCP client, include IP address, MAC address and lease
        http://192.168.1.1/internet/ipv6_static_route.asp               # Configure IPv6 static route
        http://192.168.1.1/internet/lan.asp			            # Setup router IP address and subnet mask
        http://192.168.1.1/internet/pppoe_accout.asp                    # Modify PPPoE account
        http://192.168.1.1/internet/qos.asp                             # blank
        http://192.168.1.1/internet/wan_romania.asp                     # Choose different connection type suitable for your environment.
        http://192.168.1.1/internet/wan_sfu.asp                         # Choose different connection type suitable for your environment.
        http://192.168.1.1/internet/wan_user.asp		            # blank

        http://192.168.1.1/log/log.asp			            # View router logs

        http://192.168.1.1/management/account_admin.asp                 # Configure admin account
        http://192.168.1.1/management/account_self_admin.asp	    # Configure admin account
        http://192.168.1.1/management/account_self_admin_toacs.asp
        http://192.168.1.1/management/down_cfgfile.asp                  # Backup several config files from device to PC as you wish after opening the ftp tool
        http://192.168.1.1/management/ftp_server.asp                    # Configure FTP server
        http://192.168.1.1/management/ntpchecktime.asp                  # Configure time
        http://192.168.1.1/management/reboot.asp	                    # Reboot
        http://192.168.1.1/management/restore.asp             	    # Restore device configuration (!)
        http://192.168.1.1/management/update.asp	                    # Upgrade firmware (!)

        http://192.168.1.1/menu/

        http://192.168.1.1/ont_auth/sncfg.asp                           # Modify the ONU authentication-related parameters to authenticate the OLT
        http://192.168.1.1/security/acl.asp                             # Configure ACL enable/disable, and enabled rules
        http://192.168.1.1/security/ddos.asp		            # Enable/disable DDOS
        http://192.168.1.1/security/dhcp_filter.asp                     # Blocking the MAC address to get the DHCP
        http://192.168.1.1/security/firewall_enable.asp		    # Configure firewall enable/disable
        http://192.168.1.1/security/https_enable.asp		    # Enable/disable Https
        http://192.168.1.1/security/ip_filter.asp		            # Filter ipv4 if firewall is enabled
        http://192.168.1.1/security/ipv6_filter.asp		            # Filter ipv6 if firewall is enabled
        http://192.168.1.1/security/macaddr_filter.asp		    # Filter mac addresses if firewall is enabled
        http://192.168.1.1/security/macaddr_v6_filter.asp               # Filter mac addresses if firewall is enabled
        http://192.168.1.1/security/parental_control.asp	            # Parental Control
        http://192.168.1.1/security/port_scan.asp		            # Configure Anti Port Scan enable/disable
        http://192.168.1.1/security/qos_enable.asp                      # Enable/disable Route QOS
        http://192.168.1.1/security/remote_control.asp		    # Access the web interface through WAN (!)
        http://192.168.1.1/security/route_qos.asp                       # Configure Route QOS
        http://192.168.1.1/security/url_filter.asp		            # Filter urls if firewall is enabled
        http://192.168.1.1/security/wan_acl.asp                         # Configure network access control based on internet WAN port
        http://192.168.1.1/security/wps.asp                             # Configure WPS

        http://192.168.1.1/state/deviceInfor.asp		            # Device information
        http://192.168.1.1/state/lan_state.asp			    # LAN state
        http://192.168.1.1/state/lan_state_count.asp                    # Query the state of LAN port
        http://192.168.1.1/state/opt_power.asp			    # Optical power state
        http://192.168.1.1/state/pon_info.asp                           # Query information of PON interface
        http://192.168.1.1/state/voip_auth_status.asp		    # VoIP state
        http://192.168.1.1/state/wan_state.asp			    # WAN interface state
        http://192.168.1.1/state/wan_state_user.asp                     # WAN interface state
        http://192.168.1.1/state/wireless_state.asp		            # Wireless state
        http://192.168.1.1/state/wireless_state_5g.asp	       	    # Wireless 5GHz state

        http://192.168.1.1/tr069/tr069.asp                              # Configure the url, username, password, connectionRequestUsername, connectionRequestPassword of TR069 basic settings (!)

        http://192.168.1.1/voip/

        http://192.168.1.1/wireless/basic.asp			    # Configure wireless settings
        http://192.168.1.1/wireless/basic_5g.asp		            # Configure wireless 5GHz settings
        http://192.168.1.1/wireless/security_romania.asp      	    # Configure wireless password and encryption
        http://192.168.1.1/wireless/security.asp		            # Configure wireless password and encryption
        http://192.168.1.1/wireless/security_5g.asp		            # Configure wireless 5GHz password and encryption
        http://192.168.1.1/wireless/wifimaclist.asp		            # WIFI clients list
        http://192.168.1.1/wireless/wifipowerctrl.asp		    # Set WIFI power and the number of WIFI access here
        http://192.168.1.1/wireless/wifipowerctrl_5g.asp                # Set WIFI power and the number of WIFI access here

        # Resource files

        http://192.168.1.1/js/utils.js
        http://192.168.1.1/js/checkValue.js
        http://192.168.1.1/js/versionControl.js
        http://192.168.1.1/js/jquery.js
        http://192.168.1.1/js/menu_tips.js
        http://192.168.1.1/js/frame_romania.js
        http://192.168.1.1/js/menuparse.js
        http://192.168.1.1/js/ajaxupload.3.2.js
        http://192.168.1.1/js/frame_3bb.js
        http://192.168.1.1/js/wan.js
        http://192.168.1.1/js/wifibasic.js

        http://192.168.1.1/lang/b28n.js
        http://192.168.1.1/lang/en/account.xml
        http://192.168.1.1/lang/en/firewall.xml
        http://192.168.1.1/lang/en/internet.xml
        http://192.168.1.1/lang/en/log.xml
        http://192.168.1.1/lang/en/menu.xml
        http://192.168.1.1/lang/en/restore.xml
        http://192.168.1.1/lang/en/state.xml
        http://192.168.1.1/lang/en/wireless.xml
        http://192.168.1.1/lang/en/errorpage.xml

        http://192.168.1.1/menu/sfu/ph_pldt/hisi5116/voip_dualwifi/sip/1.xml
        http://192.168.1.1/menu/hgu/ecuador/voipwifi/sip/1.xml
        http://192.168.1.1/menu/hgu/romania/voipwifi/sip/1.xml

        http://192.168.1.1/style/frame_pldt.css
        http://192.168.1.1/style/style.css
        http://192.168.1.1/style/frame_romania.css


</details>
