Once you have your sd card with raspbian, open the sd card in the file explorer and add a file called 'wpa_supplicant.conf'. Copy and paste the following into it.
```
country=US
ctrl_interface=DIR=/var/run/wpa_supplicant GROUP=netdev
update_config=1
network={
	ssid="MyWiFiNetwork"
	psk="aVeryStrongPassword"
	key_mgmt=WPA-PSK
}
```

Additionally, create a blank file called 'ssh' (with no file extension) so that you can access the device remotely and without a keyboard and monitor.


Then, if you are on Windows install PuTTY. It allows you to talk to Unix/Linux computers. Once that is installed, you should be able to ssh into the hostname 'raspberry pi' using port '22' and the ssh protocol. The command is:

```
ssh pi@raspberrypi
```
Once you login with the default password of 'raspberry,' run

```
sudo raspi-config
```

This command runs a utility for configuring raspberry pis. The sudo part means you want to do it as administrator. On Linux, the administrator account is called 'root' or 'superuser'. ```sudo``` means 'do as superuser' or 'SuperUserDO'. First, change your root password. Then, change your hostname. In the advanced configuration menu, set the memory allocation to 256, expand the filesystem, and change the resolution to 1024 * 768.  

Reboot.

Once you've connected again, we're going to install some software. Here we'll use aptitude to install software. On Linux, there are a variety of ways to install software. This is the most reliable way for raspbian, the flavor of linux that our raspberry pi runs. The command is

```
sudo apt-get install git
```


