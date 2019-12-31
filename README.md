# openwrt_router

* Starting 

Plug a network cable
```bash
dhclient -r <interface>
dhclient -v <interface>
``` 

* To reset conf and password

- poweroff , poweron,  click in the reset button then wait for dmz led become green

```bash
telnet 192.168.1.1
mount_root
# To reset password
passwd

# To reset configuration
fistboot

reboot -f
``` 

To connect in ssh

```bash
ssh root@192.168.1.1
```

* Go to web interface
http://192.168.1.1


* To configure for the freebox
IP static: 192.168.0.145, mask: 255.255.255.0, gateway:192.168.0.254, broadcast: 192.168.0.255, Custom DNS: 8.8.8.8

* To configure  the wifi 
Network -> Wifi -> Set your <ssid> and Wireless security, attach it to the network interface which have internet lan, the enable the wifi
