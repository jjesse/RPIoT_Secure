# RPIoT_Secure

Raspberry Pi as a router for a secure IoT Network

## Overview

This project runs a script to configure a Raspberry PI to function as a router and seperate Internet of Things (IoT) devcies from the main network.

A script creates a 2 Virtual LANs (VLANs) one for Users with an IP Address range of 192.168.2.0/24 and the second for IoT devices with an IP Address range of 192.168.3.0/24.

## Getting Started

## Needed for this project

The following is needed:

- Raspberry PI

- SD Card for the OS on the PI

- Ability to connect to the Raspberry PI on your network

## Steps

This guide assumes one knows how to install an Operating System (OS) on a Raspberry PI, guides on the Internet exist on how to do this.

- Connect the Raspbery PI wired connection to the Internet Modem (Cable Modem, Router, etc.)

- Configure the iotdevices.csv file to include the devices and exceptions for the firewall

  - The csv follows the format (protocol, port, name, allow/deny, description)

  - The items included are samples to understand how the file works.

- Copy the script RPIoT_Secure.sh to the Raspberry PI

- Exeucte the script (sudo RPIoT_Secure.sh)

- Restart the Raspberry PI

