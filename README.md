# TechFlash-Tool
AutoFlasher is an automated tool designed to streamline the firmware flashing process. It features a user-friendly interface, supports automatic retries on failures, and ensures secure software updates for various devices, enhancing operational efficiency.

Here's a guide to set up the necessary libraries to run the flasher device on Ubuntu.


To set up a 3.5 inch LCD screen on a Raspberry Pi running Ubuntu, you need to install the appropriate driver. Here's how to do it:

Installing the Driver for the 3.5 Inch LCD Screen
### 1. Prepare Your Raspberry Pi:
Make sure your Raspberry Pi is up to date with the following commands:
```
sudo apt-get update
sudo apt-get upgrade
```

### 2. Clone the Driver Repository:
Drivers for LCD screens are often available on GitHub. You can use the goodtft repository to obtain the necessary drivers. Clone the repository with:
```
git clone https://github.com/goodtft/LCD-show.git
```

### 3. Install the Driver:
Change directories to access the driver folder, then run the installation script:
```
cd LCD-show/
sudo ./LCD35-show
```
This script will reconfigure your Raspberry Pi to use the LCD screen as the default output. After running it, the system will automatically reboot with the display on the LCD screen.















Prerequisites
This device utilizes Python and Kivy for the user interface, along with system tools for USB management and device flashing. Here are the steps to set up your Ubuntu environment:

Install Python
Ubuntu usually comes with Python pre-installed, but you can ensure you have the latest version of Python 3 and pip (Python's package manager):

bash

```
sudo apt update
sudo apt install python3 python3-pip
```

Install Kivy
Kivy is a framework for developing multitouch applications. Install it along with necessary features support:

bash
```
# Install dependencies for Kivy
sudo apt-get install -y python3-kivy
```

Pyudev for USB Event Handling
pyudev is a pure Python binding to udev allowing for dynamic device management under Linux. Install it via pip:
bash
```
pip3 install pyudev
```

SDL2 Environment Setup
Kivy uses SDL2 for window and graphics management. Install the necessary dependencies:
bash
```
sudo apt-get install -y libsdl2-dev libsdl2-image-dev libsdl2-mixer-dev libsdl2-ttf-dev
```

These instructions will help you set up the environment to run the flasher device on an Ubuntu system effectively.
