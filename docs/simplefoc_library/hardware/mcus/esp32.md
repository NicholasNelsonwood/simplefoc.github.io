---
layout: default
title: ESP boards
nav_order: 3
description: "Arduino Simple Field Oriented Control (FOC) library ."
permalink: /esp_mcu
parent: Microcontrollers
grand_parent: Supported Hardware
grand_grand_parent: Arduino <span class="simple">Simple<span class="foc">FOC</span>library</span>
---

# ESP32 boards support

MCU | 2 PWM mode | 4PWM mode | 3 PWM mode | 6 PWM mode | pwm frequency config 
--- | --- |--- |--- |--- |--- 
esp32 | ✔️ | ✔️ | ✔️ | ❌ | ✔️ 

Esp32 devices have full coagulability using the <span class="simple">Simple<span class="foc">FOC</span>library</span> and will work with all driver types.

 Board | Name | Specifications | Link | Price
---- | --- | --- | --- | --- | ---
[<img src="extras/Images/esp32.jpg" class="imgtable150">](https://www.ebay.com/itm/Espressif-ESP32-WLAN-Dev-Kit-Board-Development-Bluetooth-Wifi-v1-WROOM32-NodeMCU/253059783728?hash=item3aeb89dc30:g:5-8AAOSwAThb3MaZ) | ESP32 | (ex. NodeMCU)<br>- 3,3V / 5V logic<br> - 16 PWMs <br>- all pins interrupts <br>- 240MHz <br> - Wifi + Bluetooth | [Ebay](https://www.ebay.com/itm/Espressif-ESP32-WLAN-Dev-Kit-Board-Development-Bluetooth-Wifi-v1-WROOM32-NodeMCU/253059783728?hash=item3aeb89dc30:g:5-8AAOSwAThb3MaZ) | 10€
[<img src="extras/Images/d1_r32.jpg" class="imgtable150">](https://www.amazon.com/Arduino-Wireless-Bluetooth-Development-Memory/dp/B07W1K56LN/ref=sr_1_2?dchild=1&keywords=d1+r32&qid=1614849959&sr=8-2) | ESP32 R32 D1 board | - 3,3V / 5V logic<br> - 16 PWMs <br>- all pins interrupts <br>- 240MHz <br> - Wifi + Bluetooth <br> - Arduino headers | [Amazon](https://www.amazon.com/Arduino-Wireless-Bluetooth-Development-Memory/dp/B07W1K56LN/ref=sr_1_2?dchild=1&keywords=d1+r32&qid=1614849959&sr=8-2)  <br> [Ebay](https://www.ebay.com/itm/USB-B-ESP32-WiFi-Bluetooth-UNO-WeMos-D1-R32-4MB-Flash-CH340-Board-for-Arduino/264084379226?hash=item3d7ca7d65a:g:f0wAAOSwIs1cEF8l) | 10€

## Arduino IDE support package

ESP32 boards are supported using [arduino-esp32](https://github.com/espressif/arduino-esp32) package, it is open source software provided by the espressif. You can download the support package through the `Arduino Board Manager` by searching for `esp32` or follow the instruction of their webpage [package installation](https://github.com/espressif/arduino-esp32#installation-instructions).

# ESP8266 boards support

MCU | 2 PWM mode | 4PWM mode | 3 PWM mode | 6 PWM mode | pwm frequency config 
--- | --- |--- |--- |--- |--- 
esp8266 | ✔️ | ✔️ | ✔️ | ❌ | ✔️ 

Esp8266 devices are still in the initial support phase in the <span class="simple">Simple<span class="foc">FOC</span>library</span> and have been tested with a set of different drivers. These boards have only 4 pwm pins so the 6PWM motor control cannot be implemented, as well as having only one analog input, the foc current control is not possible. 

 Board | Name | Specifications | Link | Price
---- | --- | --- | --- | --- | ---
[<img src="extras/Images/ESP8266-NodeMCU.jpg" class="imgtable150">](https://www.make-it.ca/nodemcu-arduino/nodemcu-details-specifications/) | NodeMCU ESP8266 | - 3,3V logic<br> - 4 PWMs <br>- all pins interrupts <br>- 80-160MHz <br> - Wifi | [Aliexpress](https://fr.aliexpress.com/item/4000160133215.html?spm=a2g0o.productlist.0.0.14227d91b2rMrV&algo_pvid=3643ec64-8668-484e-9d0e-b38be7b8c375&algo_exp_id=3643ec64-8668-484e-9d0e-b38be7b8c375-1&pdp_ext_f=%7B%22sku_id%22%3A%2210000000516093098%22%7D) | 2-10€
[<img src="extras/Images/esp8266_uno.png" class="imgtable150">](https://www.amazon.com/WOWOONE-Arduino-ESP8266-Development-Compatible/dp/B0899N647N?th=1) | ESP8266 ESP-12E D1 board | - 3,3V logic<br> - 4 PWMs <br>- all pins interrupts <br>- 80-160MHz <br> - Wifi <br> - Arduino UNO R3 headers | [Amazon](https://www.amazon.com/WOWOONE-Arduino-ESP8266-Development-Compatible/dp/B0899N647N?th=1)  <br> [Aliexpress](https://fr.aliexpress.com/item/32822012864.html?spm=a2g0o.productlist.0.0.21175f67HylnCb&algo_pvid=5b656b45-d8e5-416d-b5bb-25587a13ac55&algo_exp_id=5b656b45-d8e5-416d-b5bb-25587a13ac55-3&pdp_ext_f) | 3-10€


## Arduino IDE support package

ESP8266 boards are supported using [arduino-esp8266](https://github.com/esp8266/Arduino) package, it is open source software provided by the espressif. You can download the support package through the `Arduino Board Manager` by searching for `esp8266` or follow the instruction of their webpage [package installation](https://arduino-esp8266.readthedocs.io/en/latest/installing.html).
