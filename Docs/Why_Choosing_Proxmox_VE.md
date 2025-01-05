# Introduction to Proxmox_VE

**Proxmox VE** is an open-source, enterprise-grade virtualization platform designed to manage virtual machines (VMs) and containers. It combines the power of **KVM (Kernel-based Virtual Machine)** for full virtualization and **LXC (Linux Containers)** for `lightweight` container-based virtualization. Proxmox VE integrates virtualized computing, networking, and storage into a unified platform with an easy-to-use web interface. It is particularly appreciated for its simplicity and ease of use, making it suitable for both novice and experienced users.

Proxmox VE is based on **`Debian`**, providing a stable foundation for enterprise-level deployments. It operates under the **GNU Affero General Public License (AGPL)**, ensuring that it remains open-source and freely available for everyone. However, Proxmox offers a subscription model for users who seek commercial support and additional features.
# Key Functionality
## KVM-based Virtualization

KVM-based Virtualization lets Proxmox VE run fully isolated virtual machines (VMs), each with its own operating system and apps. Proxmox supports various OS like Linux and Windows. VMs are managed using QEMU and commands like `qm start`, `qm stop`, and `qm migrate`. Proxmox also supports live migration, which allows moving running VMs between servers without interrupting services.
## LCX-based Virtualization

LXC (Linux Containers) provides lightweight virtualization by sharing the host OS kernel, making it more efficient than VMs. Proxmox VE lets you run both containers and VMs on the same host. Containers are managed with the `pct` command (e.g., `pct start`, `pct stop`, `pct enter`). Proxmox ensures isolation between containers using control groups (cgroups) and namespaces, even though they share the same kernel.
## Storage Management

Proxmox VE offers different storage options for VMs and containers, including local, network, and distributed storage. It uses LVM for flexible storage management, allowing resizing and thin provisioning. Proxmox also supports Ceph for high availability and scalability, and ZFS for advanced features like data checks, snapshots, and replication. Additionally, it supports network storage protocols like NFS, iSCSI, and CIFS for easy integration with other storage systems.
## Network Management

Proxmox VE provides a great network management for VMs and containers. It supports **Bridged Networking**, **VLANs**, and **Bonding** for high availability and failover. **Software-defined Networking (SDN)** allows for the creation of virtual networks to isolate and connect VMs and containers efficiently. Proxmox VE also has a built-in firewall, which can be configured at the node, VM, or container level for granular security control.
## Security

Proxmox VE integrates with **LDAP**, **Active Directory**, and **two-factor authentication (2FA)** to enhance security. Role-based access control (RBAC) is available, allowing administrators to assign specific permissions to users or groups based on their roles.
## Backup and Restore

Proxmox VE supports **backup** and **restore** for both VMs and containers. Backups can be scheduled and performed live without interrupting the services. Proxmox supports full and incremental backups. **Restore** operations allow recovering the exact state of a VM or container.

**Proxmox VE also provides CLI-Tools and Web-UI for managing all the services it provides.**

[Goto Main](../README.md)
