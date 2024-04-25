# Raspberry Pi Common Commands
## Overview
This document introduces the relevant instructions in the Raspberry Pi. We can add or delete some files or codes to realize the multi-functionality of Raspberry Pi.
### Defult Command Prompt:
**"pi@raspberrypi:~$"**: It indicates that teh current host is **raspberrypi*, the user is **pi*, and the user is in the home directory of the "pi" user(/home/pi).
### Sudo:
**"sudo"** is to increase user permissions. Adding sudo in front of the command line is equivalent to running this command as the root user.
### View CPU information:
**"cat/proc/cpuinfo"**
### Check the motherboard version:
**"cat/proc/cpuinfo"**
### Shutdown:
**"sudo halt"**: Shut down immediately(close all processes, exit the kernel, and do not shut down the system power).
**"sudo poweroff"**: Shut down immediately(close all processes, exit the kernel, and turn off the system power).
**"sudo shutdown -h 5"**: Timed shutdown, here it is set to shut down after 5 minutes.
### Restart:
**"sudo reboot"**: restart immediately.
**"sudo shutdown -r now"**: restart immediately.
### Check the remaining space on the SD card:
**"df-h"**
### Go to any directory
**"cd/folder1/folder2"**: Go to the directory /folder1/folder2.
### Creating and Deleting Directories:
**"mkdir folder1"**:Creat a new directory (folder) folder1 in the curren directory.
**"rmdir folder1"**:Delete the directory (folder) folder1 under the current directory.
**"rm -rf/home/pi/temp2"**:Delete temp2 and all its contents.
### Search files 
**"sudo find/-name file.txt"**: Find files named file.txt.
**"sudo find/-name somedir -type d"**: Search for files named file.txt, only search directories.

