# Azure-Secure-Hub-Spoke-Infrastructure

## Overview

A practice lab where I designed and deployed a secure, multi-region Hub-and-Spoke network architecture on Microsoft Azure and accessed resources through a private zero-trust setup.

## What I did

* Created Azure resource groups, virtual networks, and virtual machines across two regions (South Africa North and Sweden Central).
* Bypassed a 4 vCPU regional quota limit by connecting the two networks using Global VNet Peering.
* Connected to the Ubuntu VMs securely using Azure Bastion (eliminating the need for public IPs).
* Locked down Azure Blob Storage and Azure Key Vault from the public internet using Private Endpoints.
* Configured access control using Azure Role-Based Access Control (RBAC) and a shared user-assigned managed identity.
* Practised network troubleshooting and private DNS validation using the Linux terminal.

## Linux commands practised

* `ping` — test private network connectivity between the Hub and Spoke VMs across the peering tunnel.
* `nslookup` — verify that the Blob Storage and Key Vault FQDNs resolve to private 10.x.x.x IP addresses.
* `ls` — list files and folders.
* `sudo` — execute commands with administrative privileges.

## Tools used

Microsoft Azure, Ubuntu Linux, Azure Bastion, Global VNet Peering, Private Endpoints, RBAC, SSH.

## What I learned

I practised bypassing regional subscription limits, securing cloud architectures by removing public internet access, and managing private DNS resolution through the Linux terminal.
