# PC Fan Controller for Athena Power Cases

This repository contains the circuit board and firmware for a fan controller which I designed to replace the splitter which ships with the Athena Power RM-1UC138 rackmount computer case.

<img src="https://raw.githubusercontent.com/mike42/fan-controller-athena-power/main/image.jpg" alt="Fan controller" width="600">

Instead of running the bundled 12 V fans at full speed, this controller allows you to install your own PWM fans, and set a fixed speed via a potentiometer, with no involvement from the motherboard.

## Parts list

| Qty. | Description                      | Installed at   | Product ref.                                                                                                 |
|------|----------------------------------|----------------|--------------------------------------------------------------------------------------------------------------|
|    1 | 0.1 µF ceramic capacitor         | C1             | [Adafruit 753](https://www.adafruit.com/product/753)                                                         |
|    1 | PC power "Molex" connector       | J1             | [Sparkfun PRT-15700](https://www.sparkfun.com/products/15700)                                                |
|    4 | 4-pin PC fan header              | M1, M2, M3, M4 | [Molex 47053-1000](https://au.mouser.com/ProductDetail/Molex/47053-1000)                                     |
|    1 | 10 kΩ Potentiometer 0.1" spacing | RV1            | [Core Electronics CE09096](https://core-electronics.com.au/breadboard-compatible-potentiometer-10k-ohm.html) |
|    1 | ATtiny85 microcontroller         | U1             | [ATtiny85-20P](https://au.mouser.com/ProductDetail/Microchip-Technology/ATTINY85-20PU)                       |
|    1 | Optional: DIP-8 socket           | U1             | [TE 1-2199298-2](https://au.mouser.com/ProductDetail/TE-Connectivity/1-2199298-2)                            |

## More info

- [Controlling computer fans with a microcontroller](https://mike42.me/blog/2023-09-controlling-computer-fans-with-a-microcontroller) - which shows the use of a TL-866II+ to program the ATtiny85.

## Licensing 

While you are free to use these files to build this project yourself, you do so at your own risk. No warranty or support is offered.

The code for the ATTINY85 microcontroller is based on "[4-Wire-FAN-Arduino](https://github.com/marceloaqno/4-Wire-FAN-Arduino/blob/master/ATtiny_PWM_Phase_Corret_25kHz.ino)" by Marcelo Aquino, which is licensed under the GNU GPL.

The hardware files in this repository are additionally licensed under the [Creative Commons Attribution 4.0 International License](https://creativecommons.org/licenses/by/4.0/).
