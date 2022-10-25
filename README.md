# Adafruit Neotrellis M4 8x8 MIDI Controller using CircuitPython

MIDI controller with [Adafruit NeoTrellis M4 (8x8)](https://www.adafruit.com/product/1929)

Required modules (copy to lib folder):
 - adafruit_midi
 - adafruit_neotrellis
 - adafruit_bus_device
 - adafruit_seesaw

These can be downloaded [here](https://circuitpython.org/libraries) 

## Additional Setup

Edit `code.py` to set address info for tiling. See <https://learn.adafruit.com/adafruit-neotrellis/tiling> for more info.

 - (default)             0x2E
 - A0 (+1)               0x2F
 - A1 (+2)               0x30
 - A2 (+4)               0x32
 - A3 (+8)               0x36
 - A4 (+16)              0x3E
 - A0+A1 (+3)            0x31

With a standard build, orientation places the USB connector on bottom edge, on the left side. Set the addressing as follows: 

 - Top Left, Top Right
 - Bottom Left, Bottom Right
 
## Button Colors and Modes

Edit `buttons.py` to set colors and button modes, using `colors.py` for color constants. If desired, set _OFF_BRIGHTNESS_DIVISOR_ to adjust default brightness of button.