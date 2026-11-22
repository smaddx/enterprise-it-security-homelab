# Windows Server Installation

## Project

Sentinel Defense Technologies — Enterprise IT & Security Homelab

## Objective

Deploy a Windows Server virtual machine to serve as the foundation for an enterprise Active Directory environment.

## Environments

- Hypervisor: Microsoft Hyper-V
- Operating System: Windows Server 2025 Standard Evaluation (Desktop Experience)
- VM Name: SDT-DC01
- RAM: 4 GB
- Virtual Processors: 2
- Virtual Disk: 80 GB VHDX
- Virtual Network: Sentinel-Internal

## Installation Summary

Successfully installed Windows Server 2025 inside a Hyper-V virtual machine. The VM is isolated from the physical network using an internal virtual switch.

## Purpose

This server will eventually provide:

- Active Directory Domain Services (AD DS)
- DNS
- Centralized user and computer authentication
- Group Policy management

## Evidence

See `../screenshots/server-installation.png`.

## Security Considerations

- This is a simulated enterprise environment.
- No real company data or credentials are used.
- Administrative credentials are kept private.

