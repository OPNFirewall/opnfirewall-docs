# OPNFirewall
## Scope of the Project

- [ ] UI That doesn't look like 1869
- [ ] Responsive UI that is usable on a mobile device
- [ ] A modern Router Operating System for HomeLab use based on modern tooling

## Parts of the Project

### opnfirewall-web

- Bootstrap Webapplication
- Static (Loads really fast)

## opnfirewall-api-service

- NodeJS Express application that edits and generates config files for the different services used by the opnfirewall project
- Provides 
  - An publicly accessible api for reading and writing configuration
  - An internal accessible api for the webinterface

### opnfirewall-os
- A Arch Linux based linux distribution that bundles all opnfirewall-web, opnfirewall-api-service together with the following tools
  - dhcpd (https://wiki.archlinux.org/title/dhcpd): A versitile dhcp server
  - bind (https://wiki.archlinux.org/title/BIND): An industry standard dns server
  - Iptables (https://wiki.archlinux.org/title/Iptables): An industry standard firewall application
  - ntpd (https://wiki.archlinux.org/title/Network_Time_Protocol_daemon): A simple ntp Network time Daemon
  - wireguard (https://www.wireguard.com/): A modern approach to remote-access vpn
