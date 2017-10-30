### PLDT HOME FIBR AN5506-04-FA RP2616 Advanced Settings

By default the PLDT HOME FIBR AN5506-04-FA RP2616 comes only with limited settings.

Hidden from the web interface are the rest of the router's capabilities and advanced settings.

We just need to enter the right url for the settings you're looking for.

We need to be logged in before we can do anything else, use your defined password if you already set the admin password.

Note that you have to log in again if you're idle for a few minutes on the web interface.

```
username: admin
password: 1234
```

```
http://192.168.1.1/application/ddns.asp			# Configure DDNS
http://192.168.1.1/application/dmz.asp			# Set host IP to DMZ
http://192.168.1.1/application/ping_diagnosis.asp	# Network diagnosis. Ping and Traceroute
http://192.168.1.1/application/port_forwarding.asp      # Configure port forwarding
http://192.168.1.1/application/redirect.asp		# blank
http://192.168.1.1/application/upnp.asp			# Configure UPnP enable/disable

http://192.168.1.1/internet/dhcp_service.asp		# Enable/disable DHCP functions, configure parameters
http://192.168.1.1/internet/dhcp_userlist.asp		# Display information about DHCP client, include IP address, MAC address and lease
http://192.168.1.1/internet/lan.asp			# Setup router IP address and subnet mask
http://192.168.1.1/internet/wan_user.asp		# blank

http://192.168.1.1/log/log.asp			        # View router logs

http://192.168.1.1/management/account_self_admin.asp	# Configure admin account
http://192.168.1.1/management/reboot.asp	        # Reboot
http://192.168.1.1/management/restore.asp       	# Restore device configuration (!)
http://192.168.1.1/management/update.asp	        # Upgrade firmware (!)

http://192.168.1.1/security/ddos.asp		        # Enable/disable DDOS
http://192.168.1.1/security/firewall_enable.asp		# Configure firewall enable/disable
http://192.168.1.1/security/https_enable.asp		# Enable/disable Https
http://192.168.1.1/security/ip_filter.asp		# Filter ipv4 if firewall is enabled
http://192.168.1.1/security/ipv6_filter.asp		# Filter ipv6 if firewall is enabled
http://192.168.1.1/security/macaddr_filter.asp		# Filter mac addresses if firewall is enabled
http://192.168.1.1/security/parental_control.asp	# Parental Control
http://192.168.1.1/security/port_scan.asp		# Configure Anti Port Scan enable/disable
http://192.168.1.1/security/remote_control.asp		# Access the web interface through WAN (!)
http://192.168.1.1/security/url_filter.asp		# Filter urls if firewall is enabled

http://192.168.1.1/state/deviceInfor.asp		# Device information
http://192.168.1.1/state/lan_state.asp			# LAN state
http://192.168.1.1/state/opt_power.asp			# Optical power state
http://192.168.1.1/state/voip_auth_status.asp		# VoIP state
http://192.168.1.1/state/wan_state.asp			# WAN interface state
http://192.168.1.1/state/wireless_state.asp		# Wireless state
http://192.168.1.1/state/wireless_state_5g.asp		# Wireless 5GHz state

http://192.168.1.1/wireless/basic.asp			# Configure wireless settings
http://192.168.1.1/wireless/basic_5g.asp		# Configure wireless 5GHz settings
http://192.168.1.1/wireless/security.asp		# Configure wireless password and encryption
http://192.168.1.1/wireless/security_5g.asp		# Configure wireless 5GHz password and encryption
http://192.168.1.1/wireless/wifimaclist.asp		# WIFI clients list
http://192.168.1.1/wireless/wifipowerctrl.asp		# Set WIFI power and the number of WIFI access here
http://192.168.1.1/wireless/wps.asp			# Configure WPS

# Resource files

http://192.168.1.1/images/login_pldt.jpg
http://192.168.1.1/images/pldt_fibr.png

http://192.168.1.1/js/utils.js
http://192.168.1.1/js/checkValue.js
http://192.168.1.1/js/versionControl.js
http://192.168.1.1/js/jquery.js
http://192.168.1.1/js/menu_tips.js
http://192.168.1.1/js/frame_romania.js
http://192.168.1.1/js/menuparse.js

http://192.168.1.1/lang/b28n.js

http://192.168.1.1/menu/hgu/romania/voipwifi/sip/1.xml

http://192.168.1.1/style/frame_pldt.css
http://192.168.1.1/style/style.css
http://192.168.1.1/style/frame_romania.css
```