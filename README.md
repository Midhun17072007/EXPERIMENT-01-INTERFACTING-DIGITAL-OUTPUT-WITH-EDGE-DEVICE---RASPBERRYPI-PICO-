# EXPERIMENT-01-INTERFACTING-DIGITAL-OUTPUT-WITH-EDGE-DEVICE---RASPBERRYPI-PICO-
## NAME MIDHUN S
## DEPARTMENT: AIDS
## ROLL NO:212224230158
## DATE OF EXPERIMENT: 24/02/2025

### AIM
To interface a digital output device (LED) with the Raspberry Pi Pico and control it using MicroPython.

APPARATUS REQUIRED
Raspberry Pi Pico
LED (Light Emitting Diode)
330Ω Resistor
Breadboard
Jumper Wires
USB Cable
Computer with Thonny IDE
## THEORY
Raspberry Pi Pico is a microcontroller board based on the RP2040 chip. It supports MicroPython, making it suitable for IoT and embedded applications.

Digital Output refers to controlling external devices like LEDs, buzzers, or relays using GPIO (General Purpose Input Output) pins. A GPIO pin can be set to HIGH (3.3V) or LOW (0V) to turn the device ON or OFF.

## Working Principle:

The LED is connected to one of the GPIO pins of the Pico.
The MicroPython script sets the GPIO pin HIGH to turn the LED ON and LOW to turn it OFF.
CIRCUIT DIAGRAM
Connect the anode (longer leg) of the LED to GP15 via a 330Ω resistor.
Connect the cathode (shorter leg) of the LED to GND (ground).


## PROGRAM (MicroPython)
```
from machine import Pin
from utime import sleep
led1 = Pin(0, Pin.OUT)
led2 = Pin(4, Pin.OUT)
led = Pin(11, Pin.OUT)

while True:
    led1.toggle()
    sleep(0.5)
```
from machine import Pin
from utime import sleep
led1 = Pin(0, Pin.OUT)
led2 = Pin(4, Pin.OUT)
led = Pin(11, Pin.OUT)

while True:
    led1.toggle()
    sleep(0.5)
    led2.toggle()
    sleep(0.5)
    led.toggle()
    sleep(0.5)
```
from machine import Pin
from utime import sleep
led1 = Pin(0, Pin.OUT)
led2 = Pin(4, Pin.OUT)
led = Pin(11, Pin.OUT)
buzz=Pin(6, Pin.OUT)

while True:
    led1.toggle()
    sleep(0.5)
    buzz.toggle()
    sleep(0.5)
    led2.toggle()
    sleep(0.5)
    buzz.toggle()
    sleep(0.5)
    led.toggle()
    sleep(0.5)
    buzz.toggle()
    sleep(0.5)
```
## OUPUT
![Screenshot 2025-02-24 113539](https://github.com/user-attachments/assets/64c29d22-3066-47fe-add3-4461c57afa24)

![Screenshot 2025-02-24 112909](https://github.com/user-attachments/assets/8ed072e9-30b3-4f89-9b87-eae81c78f64d)
 
 ![Screenshot 2025-02-03 151338](https://github.com/user-attachments/assets/9d676038-2408-4b4c-9a7a-3f95fdf21e5b)

## RESULTS
The LED connected to the Raspberry Pi Pico successfully turns ON and OFF at 1-second intervals, confirming the proper interfacing of a digital output.
