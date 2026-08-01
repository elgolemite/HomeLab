# HomeLab Setup

This repository documents my cybersecurity homelab environment.

## Virtualization Platform

- VMware Workstation Pro 17

## Machines

| Machine | Version | Hostname | IP Address | Description |
|---|---|---|---|---|
| Windows Server | Windows Server 2025 | DC01 | 192.168.10.10 | Domain controller used to manage users, groups, DNS, and Group Policy |
| Windows Client | Windows 11 | CLIENT01 | 192.168.10.20 | Client machine joined to the Active Directory domain |
| pfSense | Community Edition 2.8.1 | pfSense | 192.168.10.1 | Firewall, DHCP server, default gateway, and router |
