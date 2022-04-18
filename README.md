# MotionEyeOS_APconfig
Motion Eye OS V20200606 Access Point Configuration, Without Internet  

Simply drag the files in the repo into raspberry pi boot folder which contains things like .elf file and kernel.img.  

Default:  
ssid=motioneyessid  
wpa_passphrase=1234567  

Edit the field in hostapd.conf  

# Theory  

* hostapd is what creates the Access Point(AP)
* dnsmasq is a DHCP server which gives out the IPs to PCs/Phones connecting to your motioneyeOS Pi
* static_ip.conf is required for some reason, or else attempt to connect will error "cannot assign IP"
* os.conf tells the OS it doesnt need to be connected to the network since it is the one hosting the network
