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
### How to access main router from WAP?
Currently if I connect to main Buffalo router from PC, I can't access my secondary WAP router for some reason. Will have to look into it - probably will be non-issue after I install OpenWRT on Buffalo router.
# Future To-Do
#### Open port forward through VPN for remote internet access
Already bought a static IP thing from Windscribe, will see how I can set up something so that I can access the server from anywhere. 
Will need to set firewall rules for security, so def wanna take my time with this and not rush it just to have my entire network pwned.
<!--stackedit_data:
eyJoaXN0b3J5IjpbMTE0ODgyOTEwNV19
-->