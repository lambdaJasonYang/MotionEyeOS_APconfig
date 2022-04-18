# MotionEyeOS_APconfig
Motion Eye OS V20200606 Access Point Configuration, Without Internet for the Raspberry Pi

Simply drag the files in the repo into raspberry pi boot folder which contains things like .elf file and kernel.img.  

Default:  
ssid=motioneyessid  
wpa_passphrase=12345678

Edit the field in hostapd.conf for custom ssid name and password  

Go to browser and enter 192.168.27.1 into the URL bar to access MotionEyeOS web interface after connecting to the Access Point.

# Theory  

* hostapd is what creates the Access Point(AP)
* dnsmasq is a DHCP server which gives out the IPs to PCs/Phones connecting to your motioneyeOS Pi
* static_ip.conf is required for some reason, or else attempt to connect will error "cannot assign IP"
* os.conf tells the OS it doesnt need to be connected to the network since it is the one hosting the network
