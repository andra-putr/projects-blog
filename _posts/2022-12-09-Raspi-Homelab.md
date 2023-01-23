---
published: true
---
And yet another Raspberry Pi cluster home server. Also includes optimizing home network setup.

# Setup

#### PI Cluster
- Raspberry Pi 4
	- Main server
	- Running Docker
		- Portainer docker manager
		- Main pihole server
		- PXE Boot server (future)
- Raspberry Pi Zero WH
	- Secondary server
	- Running docker
		- Portainer docker manager
		- Secondary pihole server
- Raspberry Pi Zero WH
	- Tertiary server
	- Still not set up

#### Network Setup
- Buffalo router
	- Main router directly connected to fiber modem
	- Currently running stock firmware, will install OpenWRT on it so I can set DNS servers to Pihole.
- Elecom router
	- Running OpenWRT
	- Was main router, but delegated to temporary secondary router & WAP
		- Ended up being too weak to serve reliable gigabit speeds
	- Will end up being slave WAP to Buffalo router
- TP-Link gigabit switch
	- Switch for raspberry pi cluster

# Current Issues
### PiHole not blocking everything
For some reason though it says it's blocking things, ads still come through.
The main reason why I wanted to start this project in the first place was so that I can have an ad-free Chromecast experience, and from what I read it's gonna be harder with the Chromecast since apparently it's hard-coded to go through Google's DNS servers for everything.
Will have to find a way to spoof connection to my DNS servers instead in the future.

Update (2023/1/23):
	After some fiddling about and installing OpenWrt on both of my routers, pihole now is able to block *most* ads on the devices on my network. Chromecast however is still a bit of a problem...
	Even after I blocked all outward DNS requests on port 53 and re-route them to my pihole servers, seems like Google still manages to inject ads to my chromecast's YouTube through on way way or another.
	After messing around with it an entire day I decided you know what - there's probably a third party app for YouTube that allows me to watch YouTube ad-free instead of messing about with DNS spoofing and all that. Lo and behold - I found [SmartTubeNext](https://github.com/yuliskov/SmartTubeNext) which surprisingly works PERFECTLY. All I needed to do was re-bind my Chromecast remote's YouTube button to launch that app instead and voila, ad-free YouTube on my chromecast that I actually 

### How to access main router from WAP?
Currently if I connect to main Buffalo router from PC, I can't access my secondary WAP router for some reason. Will have to look into it - probably will be non-issue after I install OpenWRT on Buffalo router.
# Future To-Do
#### Open port forward through VPN for remote internet access
Already bought a static IP thing from Windscribe, will see how I can set up something so that I can access the server from anywhere. 
Will need to set firewall rules for security, so def wanna take my time with this and not rush it just to have my entire network pwned.

This will probably be set up through another Docker container running OpenVPN on the respective Raspi servers.



<!--stackedit_data:
eyJoaXN0b3J5IjpbMTMyNTk2NzA1LDI5MzY1NzMxNSwxNDAxMT
cyNzY3XX0=
-->