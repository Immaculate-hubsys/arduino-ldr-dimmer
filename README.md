# LDR Auto-Dimmer

Automatically adjusts LED brightness based on ambient 
light level using an LDR module and PWM on Arduino Uno.

## Components
- Arduino Uno
- LDR Module (4-pin)
- 1x LED
- 1x 220Ω Resistor

## Concepts Covered
- analogRead() — reading sensor values (0-1023)
- analogWrite() — PWM LED brightness control (0-255)
- map() — converting sensor range to brightness range
- millis() — non-blocking Serial Monitor updates
- Sensor calibration

## How It Works
LDR reads ambient light level. The value is mapped 
from 0-1023 to 0-255 and written to the LED via PWM.
Bright light = dim LED. Dark room = bright LED.
Sensor calibrated from 8-1023 (real hardware minimum).

## Simulation
[Run on Wokwi](https://wokwi.com/projects/466303027387358209)
