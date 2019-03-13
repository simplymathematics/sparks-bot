# Getting Started

## Example

## Feather Line

## Esp8266 Docs

## Digital Logic

## Analog Logic

## Databases and Data Storage

### SQL

### MQTT

### JSON

## Networking

# Robot Control Software

Adafruit has a variety of boards with the 'Feather' name. These are boards that play nice with each other by easily sharing data, power, and control pins where appropriate. In many cases, these board stack on top of each other. There are also cheap adapters  that connect these boards side-by-side, supporting up to 3 boards. However, you will have to do a power budget to ensure that you have enough current (measured in mA) to power everything you want to do. If you're very clever, you can power your sensors on at different times and conserve power. 

## esp8266-robot

This is the software to build a web-controlled robot using the esp8266. It supports the current configuration of the esp-8266 board driving the Feather DC motor board

## mqtt_esp8266

MQTT is a protocol for exchanging data between a bunch of clients (the esp_8266) and your central server (the raspberry pi). 

## interface

This folder contains the html, css, and javascript code that makes a website in a browser that can control your robot. It currently supports, up, down, left, and right, buttons that then send json requests to the hard-coded ip address in the script.js document. Currently, it is set to 192.168.50.221. This can be run on any computer that is connected to the same network as the robot. Style.css is the stylesheet, and demo.html is the webpage that you open in the browser. Either double-click that file or open it in firefox using the command line
```
firefox demo.html &
```
where the ```&``` allows you to continue to use that terminal even though it has an open, running process (Firefox). 


# Data Server Software

## MQTT Broker

## VLC

## MySQL

## Anaconda Server

## Multi-Threading


