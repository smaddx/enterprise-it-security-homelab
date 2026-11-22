# Network Configuration

## Project
Sentinel Defense Technologies – Enterprise IT & Security Homelab

## Virtualization Platform
Microsoft Hyper-V on Windows 11 Pro.

## Virtual Network

| Setting | Configuration |
|---|---|
| Switch Name | Sentinel-Internal |
| Switch Type | Internal |
| Host Connectivity | Enabled |
| VM-to-VM Connectivity | Enabled |
| Direct Physical Network Access | Not provided by this switch |

## Purpose

The internal virtual switch provides an isolated networking environment for the simulated enterprise infrastructure.

It will allow virtual machines to communicate with each other and the host operating system without directly connecting the lab network to the physical LAN.

## Future Configuration

- Configure an internal IPv4 subnet.
- Deploy Windows Server.
- Configure DNS and Active Directory.
- Connect Windows client machines.
- Implement network security controls.

## Security Considerations

This is a personal training environment. No company data, credentials, or Controlled Unclassified Information (CUI) will be stored in this lab.
