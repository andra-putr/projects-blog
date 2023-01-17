---
published: true
---
And yet another Raspberry Pi cluster home server. Also includes optimizing home network setup.

(工事中)

# Setup
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

# Current Issues
### PiHole not blocking everything
For some reason though it says it's blocking things, ads still come through

# Future To-Do
- Open port forward through VPN for remote internet access
	- Will need to set firewall rules for security
<!--stackedit_data:
eyJoaXN0b3J5IjpbMTYzNDIyMzMyMl19
-->