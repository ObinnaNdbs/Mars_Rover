# Software Setup Instructions

## Overview
This document guides you through setting up the software necessary for operating the Mars Rover. This includes installing the operating system on the Raspberry Pi and configuring the Navio2 board.

## Steps

### 1. Prepare the Raspberry Pi:
- **Download the Raspbian Image**: Start by downloading the latest version of Raspbian from [Raspberry Pi OS Downloads](https://www.raspberrypi.org/software/).
- **Write the Image to an SD Card**: Use Balena Etcher, which can be downloaded from [Balena Etcher](https://www.balena.io/etcher/), to write the image to your SD card.

### 2. Set Up Navio2:
- **Attach the Navio2 to the Raspberry Pi**: Securely attach the Navio2 board to your Raspberry Pi using the GPIO pins.
- **Install Navio2 Drivers**: Navigate to [Emlid Documentation](https://docs.emlid.com/navio2/) to download and install the necessary drivers and software for the Navio2.

### 3. Network Configuration:
- **Configure Wi-Fi**: Edit the `wpa_supplicant.conf` on the SD card to include your Wi-Fi network details. This file can be accessed by inserting the SD card into a computer and navigating to the boot partition. If use Putty to set up the Raspberry Pi internally later, the labtop and Rasbperry Pi need to be on the same WIFI.
  
  ```plaintext
  network={
      ssid="Your_Network_Name"
      psk="Your_Password"
  }
- **Enable SSH**: To enable SSH access on your Raspberry Pi, place a file named ssh (without any extension) onto the boot partition of the SD card.
### 4. First Boot and SSH Connection:
- **Boot the Raspberry Pi**: Insert the SD card into the Raspberry Pi and power it on.
- **Connect via SSH**: Use an SSH client to connect to the Raspberry Pi. The default hostname is **raspberrypi**, and the default login is **pi** with the password **raspberry**.

### 5. Find the IP address:
- **Connect via SSH**: Using **ifconfig** code to get the Raspberry pi IP address.
  ![Raspberry pi IP_address](https://github.com/ShuoHuang999678/image/blob/main/IP_address.jpg?raw=true)

### 6. View Data
- **Download Winscp**:
For detailed steps and troubleshooting, refer to the full [ROV Avionics Instructions PDF](https://github.com/ObinnaNdbs/Mars_Rover/blob/main/Documents/ROV_Avionics_instructions.pdf).
