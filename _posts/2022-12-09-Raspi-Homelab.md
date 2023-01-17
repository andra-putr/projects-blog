---
published: true
---
And yet another Raspberry Pi cluster home server. Also includes optimizing home network setup.

(工事中)

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
	- Currently running stock firmware, will install OpenWRT on it so I can set DNS servers to Pihole
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
The main reason why I wanted to start this project in t
### How to access main router from WAP?

# Future To-Do
- Open port forward through VPN for remote internet access
	- Will need to set firewall rules for security
<!--stackedit_data:
eyJoaXN0b3J5IjpbMTAwMDA5NzgwMl19
-->