# NodeMCU WiFi Relay Control using SinricPro
This project demonstrates how to control relays connected to an ESP8266 microcontroller(NodeMCU) over WiFi using the SinricPro library. It enables you to remotely switch relays on and off using the SinricPro cloud platform.

Features

Control relays connected to ESP8266 microcontroller over WiFi.
Use SinricPro cloud platform to remotely switch relays on and off.
Supports multiple devices with individual control.
Hardware Requirements

ESP8266 microcontroller board (NodeMCU)
Relay module(s)
Tactile switches or toggle switches (optional, depending on configuration)
LEDs (optional, for status indication)
Installation

Clone or download this repository.
Open the Arduino IDE.
Install the required libraries:
ESP8266WiFi
SinricPro
Update the following parameters in the sketch:
WiFi SSID and password (WIFI_SSID and WIFI_PASS)
SinricPro API key and secret (APP_KEY and APP_SECRET)
Device IDs (device_ID_1, device_ID_2, etc.)
GPIO pins connected to relays and switches (RelayPin1, SwitchPin1, etc.)
Upload the sketch to your ESP8266 board.
Usage

Connect your ESP8266 board to power and ensure it's connected to your WiFi network.
Use the SinricPro mobile app or web dashboard to discover and control the devices.
Optionally, use tactile switches or toggle switches connected to the GPIO pins to manually control the relays.
Configuration

The devices map in the sketch defines the device IDs and GPIO pins connected to relays and switches. Update this map according to your hardware setup.
Uncomment #define TACTILE_BUTTON if you're using tactile switches instead of toggle switches.
Dependencies

ESP8266WiFi: Library for connecting ESP8266 to WiFi.
SinricPro: Library for interfacing with the SinricPro cloud platform.
