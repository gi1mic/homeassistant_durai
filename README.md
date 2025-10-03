# homeassistant_durai
Homeassistant integration for Duracell/CYD Skyline/Midnite AIO Inverters using esphome 



Esphome config to connect a Duracell Durai Inverter into homeassistant
Should also work with similar CYG Skyline based inverters such as the MidNite AIO 

The register maps where taken from https://github.com/iPeel/HA-Skyline/tree/main
and my thanks goes out to iPeel who created the above project.

This project requires an ESP32 and a low cost RS232 to RS485 adapter
 
A Liligo LILYGO T-CAN485 or a Waveshare ESP32-S3-RS485-CAN should work but may need the UART pins changed
