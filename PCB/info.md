# Ratless65

## Nice Info

* [QMK docs for split keyboards](https://docs.qmk.fm/#/feature_split_keyboard)

* A pro_micro with the [rp2040](https://www.google.com/search?client=firefox-b-d&q=rp2040) chip could be best with [full duplex communication](https://docs.qmk.fm/#/serial_driver?id=usart-full-duplex) between the two side would be best.

* [Firmware config](https://docs.qmk.fm/#/feature_split_keyboard?id=firmware-configuration)

* [handedness by pin](https://docs.qmk.fm/#/feature_split_keyboard?id=handedness-by-pin), if high it is assumed to be the left side, therefore the left side must be high while the right side must be low.

### Key Differences Between Pull up and Pull down

- **Default State:**
  - **Pull-Up Resistor:** Ensures the input defaults to high (logic 1).
  - **Pull-Down Resistor:** Ensures the input defaults to low (logic 0).
  
- **Use Cases:**
  - **Pull-Up Resistor:** Common in open-collector or open-drain configurations, switches, and buttons.
  - **Pull-Down Resistor:** Less common but used in situations where a default low state is desired.


### Pull Up:
5V -> Pin -> R

output --> 1023, 4.7v


### Pull Down:
GND -> R -> Pin

output --> 0, 0v
