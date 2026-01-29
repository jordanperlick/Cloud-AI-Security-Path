# Day 03 — Ubuntu Golden Image + Snapshot

## Objective
Create the Ubuntu base VM (Golden Image), update it, install core tools, and take a clean snapshot.

## VM Settings (VMware)
- VM Name: Ubuntu-Lab
- ISO used: ubuntu-24.04.3-desktop-amd64.iso
- CPU: 2 cores
- RAM: 4 GB (or 6 GB if applicable)
- Disk: 50 GB (split into multiple files)
- Network: NAT
- VM Location: C:\LAB\VMs\Ubuntu-Lab\

## Install Notes
- Installation type: Erase disk and install Ubuntu (virtual disk only)
- Username: <your_user>
- Desktop reached successfully after install/reboot

## Post-install Commands (Terminal)
```bash
sudo apt update && sudo apt -y upgrade
sudo apt install -y git curl unzip build-essential python3-pip net-tools
sudo apt install -y open-vm-tools open-vm-tools-desktop
sudo reboot

