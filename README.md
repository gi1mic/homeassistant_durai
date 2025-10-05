# Homeassistant/ESPhome integration for Duracell Durai Solar Inverters

ESPhome configuration for monitoring and control of Duracell/Senergy/CYD Skyline/Midnite AIO inverters in Home Assistant. 

The register maps were taken from https://github.com/iPeel/HA-Skyline/tree/main
and my thanks to iPeel who created the above project.



# Known issues
* This is a work in progress, the data may not be correct!!!!!


# Requirements

*    ESP32 (But should work on any supported ESPhome device)
*    TTL To RS485 Module with automatic flow control

![alt text](https://github.com/gi1mic/homeassistant_durai/blob/main/images/rs485%20connection.jpg "RS485 Wiring")

RX and TX pins are connected to the ESP32 pins 16 and 17 or a Liligo LILYGO T-CAN485 or a Waveshare ESP32-S3-RS485-CAN should work but may need the UART pins changed
I have ordered the Waveshare device and will update the code in due course for it.

![alt text](https://github.com/gi1mic/homeassistant_durai/blob/main/images/ESP32-S3-RS485-CAN.avif "Waveshare ESP32-S3-RS485-CAN")
![alt text](https://github.com/gi1mic/homeassistant_durai/blob/main/images/LILYGO%20T-CAN485%20ESP32%20CAN%20RS-485.avif "Lilygo")


# Installation

*    Create your esp32 in esphome in home assistant using the yaml file (make sure you have your wifi ssid&password in the secrets and set the API and OTA passwords in the yaml file)
*    Upload the the compiled code via. usb to the ESP32
*    Test wireless upload
*    Edit the sensor names in the config if you like
*    Re-upload via wireless and test
