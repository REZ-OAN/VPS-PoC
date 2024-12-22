# Building Your Own VPS
# Table of Contents
- [Introduction](#introduction)
- [Fundamental Requirements](#fundamental-requirements)
- [My Findings](#my-findings) 
- [Steps To Follow](#steps-to-follow)
# Introduction
In this repository I will guide you to a whole process how and why I came with an idea to building a VPS from scratch. The documents are provided here are part of my learnings and understandings throughout the process of building a VPS. I will update this repository as per my learnings and towards making a VPS. 
# Fundamental Requirements
- A `PC`or `RaspberryPI` (I am using my old pc ASUS k556UR)
				<details>
					<summary>
						Configuration of my PC
					 </summary>
					 CPU -> Corei7 7th gen
					 RAM -> 12GB
					 HDD -> 1TB
					 SSD  -> 250GB 
				 </details>
- Setup any of the linux distribution as per your need.
	<details>
			 <summary>
				I've Used
			 </summary>
			 Linux Distribution -> Ubuntu 22.04 LTS
			 Because I want to use Type-2 Hypervisor, I only need to understand the VPS working. If you're concern about performance overhead you can setup any Type-1 Hypervisor.
	</details>

# My Findings
- [Security, Reliability, Flexibility](./Docs/Security_Reliability_Flexibility.md)
- [Hosting Types](./Docs/Hosting_Types.md)
- [VPS-POC towards DevOps and Cloud Engineering](./Docs/VPS-POC_towards_DevOps_and_Cloud_Engineering.md)
- [Why Choosing Proxmox VE](./Docs/Why_Choosing_Proxmox_VE.md)
- [ProxmoxVE Architechture](./Docs/ProxmoxVE_Architechture.md)
- [Hypervisor Types](./Docs/Hypervisor%20Types.md)
- [SSH Working](./Docs/SSH_Working.md)
- [Logical Volume Management](./Docs/logical_volume_manager.md)
# Steps To Follow
- [Setup Host Machine](./Docs/Setup%20Linux%20Distribution%20On%20Host%20Machine.md)
- [Network Architechture of My Setup](./Docs/network_diagram.md)
- [Setup Remote Access](./Docs/Setup%20Remote%20Access%20Using%20OpenSSH.md)
- [LVM Hands on](./Docs/lvm_commands.md)
- [Reduce LV's size using LVM](./Docs/reduce_size_of_lv.md)
