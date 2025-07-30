# 💡 MicroPython LED Blinker

This is a simple MicroPython script that blinks the onboard LED of a microcontroller, such as the Raspberry Pi Pico. It toggles the LED on and off every 0.5 seconds.

## 🧰 What It Does

- Turns the onboard LED **on** for 0.5 seconds
- Turns it **off** for 0.5 seconds
- Repeats the cycle forever

This is a classic "Hello World" project for microcontrollers and is great for testing your board setup.

## 🛠️ Requirements

- A MicroPython-compatible board (e.g., Raspberry Pi Pico)
- MicroPython firmware flashed to the board
- A USB cable and serial terminal (e.g., Thonny, PuTTY)

## 📦 File Overview

- `main.py` — Main script to blink the LED
- `README.md` — This documentation

## 🧪 Code

```python
from machine import Pin
import utime

led = Pin(25, Pin.OUT)

while True:
    led.value(1)
    utime.sleep(0.5)
    led.value(0)
    utime.sleep(0.5)
