---
title: Building My Homelab
published: true
excerpt:I'm always seeking new learning opportunities whenever available so that I can continue to grow my skills within the IT and cybersecurity industry. That is how...
description: Patrick Cannon. University of Central Florida. Information Technology Major. Secure Computing and Networking Minor...
---

<br>

## Planning Phase

I'm always seeking new learning opportunities whenever available so that I can continue to grow my skills within the IT and cybersecurity industry. That is how I stumbled upon homelabs. Homelabs are essentially personal learning environments where individuals are able to run their own experiments with hardware or software, troubleshoot new technologies, or just gain confidence with technologies before utilizing them professionally. 

After realizing I could build my own server environment within the comfort of my own home, I immediately began planning what first piece of hardware would be suitable to kick off the homelab as well as what experiments I would be able to run on said hardware. A common trend I noticed was to convert old computer hardware into home servers, so I opted to do just that, and planned to convert an old desktop into a homelab vm server where I could create and run as many virtual machines as I would like. 

<br>

# Hardware and Software

Now that I had a general plan in mind, the next steps of this project were to find suitable hardware that supported my initial goals. These goals mainly consisted of having a setup that could reliable run a minimum of 3-4 virtual machines at all times without any major performance issues. After researching potential candidates, I ended up opting for a refurbished Dell OptiPlex that had all the hardware specifications I would need for any projects I intended on running. 

As for the software, after doing some more thorough research, I decided to utilize Proxmox VE for the server’s hypervisor. Proxmox stood out to me especially as it offers solid performance for running multiple virtual machines and also allows for them to be easily created, managed, and scaled efficiently. 

<br> 

## Server Setup

The current setup I have dedicated on this server is to have three virtual machines be created and running constantly with each machine dedicated to a certain task.

Host OS: Proxmox VE
Running Virtual Machines:
- Pfsense:
  For my first virtual machine, I’ve deployed pfSense to serve as the primary firewall and router for the homelab. This setup allows me to gain hands-on experience with core network security concepts such as network     segmentation, firewall rule configuration, and VPN setup. I’ve dedicated this VM exclusively to pfSense to ensure that all other virtual machines in the environment operate behind a consistently available and          properly managed firewall.

- Splunk:
  Splunk is an essential tool for log analysis and security event monitoring. I’ve deployed it on this VM in order to build practical experience with SIEM (Security Information and Event Management) workflows.

- (To be determined...):
  Currently, I am still planning what software will go on future VMs but some possible candidates could be either Security Onion or Wazuh. 

