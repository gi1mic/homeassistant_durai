# Homeassistant/ESPhome integration for Duracell/Senergy/CYD Skyline/Midnite AIO inverters

ESPhome configuration for monitoring and control of Duracell/Senergy/CYD Skyline/Midnite AIO inverters in Home Assistant. 

The register maps were taken from https://github.com/iPeel/HA-Skyline/tree/main plus information found on the net. 
I thank iPeel who created the above project as I would never have got far without his code.



# Known issues
* This is a work in progress, but the basic info most people will need is available


# Requirements

*    Waveshare ESP32-S3-RS485 module but any ESP32 with a TTL To RS485 Module should work

![alt text](https://github.com/gi1mic/homeassistant_durai/blob/main/images/ESP32-S3-RS485-CAN.avif "Waveshare ESP32-S3-RS485-CAN")



You can use an ESP32 and a RS485 module with automatic flow control using the following diagram

![alt text](https://github.com/gi1mic/homeassistant_durai/blob/main/images/rs485%20connection.jpg "RS485 Wiring")

RX and TX pins are connected to the ESP32 pins 16 and 17.

A Liligo LILYGO T-CAN485 should work but may need the UART pins changed.


# Waveshare ESP32-S3-RS485 Installation

*    Create a blank yaml file (device) using esphome and select edit the new file.
*    Cut and paste the contents of the waveshare-esp32-s3-rs485.yaml file into your new device
*    Make sure you have your wifi ssid&password in the homeassistant secrets file and set the API and OTA as required in the yaml file
*    Select install and upload the the compiled code to your waveshare device
*    The install will pull the latest yaml file from github every time you reinstall. If you do not want to do that you will need to create your own YAML config
