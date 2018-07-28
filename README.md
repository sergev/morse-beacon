# Morse CW Beacon

Here you can find the sources of a simple CW beacon, for ESP32 board with LoRa and OLED display.
The beacon sends a predefined message as Morse code on a fixed frequency, like 433.575 MHz.
The signal can be received using any UHF handheld.

## Hardware Requirements

 * ESP32 board with LoRa SX1278 transceiver and OLED SSD1306 display

Two boards are supported:

![](https://raw.githubusercontent.com/wiki/sergev/morse-beacon/img/wifi-lora32.jpg)

![](https://raw.githubusercontent.com/wiki/sergev/morse-beacon/img/ttgo-lora32.jpg)

## Software Requirements

 * Arduino IDE `>= 1.8.5`
 * Arduino support for ESP32 platform
 * Adafruit GFX Library

## Build

1. Get the sources: `git clone https://github.com/sergev/morse-beacon.git`

2. Modify the message at end of `morse-beacon.ino` file. Replace the callsign and add any information you may find useful (QTH etc).

3. Make sure pin definitions match your ESP32 board (LORA_RST, OLED_SDA, OLED_SCL, LED).

4. Change the frequency to the desired value (FREQ_HZ).

5. Compile and upload the program to the board.

## Credits

*morse-beacon* was created by Serge Vakulenko, KK6ABQ.
