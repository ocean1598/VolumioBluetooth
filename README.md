# VolumioBluetooth

A simple, light weight Bluetooth audio receiver.

## Features

Devices like phones, tablets and computers can play audio to the volumio Raspberry Pi.

## Requirements

- Raspberry Pi with Bluetooth support (tested wth Raspberry Pi 3)
- Volumio 2

## Installation

The installation script asks whether to install each component.

    wget -q https://github.com/myichimoku/VolumioBluetooth/archive/master.zip
    sudo apt-get install unzip
    unzip master.zip
    rm master.zip

    cd VolumioBluetooth-master
    ./install.sh

### Bluetooth

Sets up Bluetooth, adds a simple agent that accepts every connection, and enables audio playback through [BlueALSA](https://github.com/Arkq/bluez-alsa). A udev script is installed that disables discoverability while connected.

## Disclaimer

These scripts are tested and work on a current (as of April 2020) Volumio 2 setup on Raspberry Pi. Depending on your setup (board, configuration, sound module, Bluetooth adapter) and your preferences, you might need to adjust the scripts. They are held as simple as possible and can be used as a starting point for additional adjustments.

## References
https://github.com/nicokaiser/rpi-audio-receiver
https://forum.volumio.org/volumio-bluetooth-receiver-t8937.html

