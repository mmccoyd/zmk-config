Hillside 46 is a split ergonomic keyboard with 3x6+5 choc-spaced keys.
It has the aggressive stagger of the Ferris but a longer thumb arc and a break-off outer pinkie column.
More information is at [github/mmccoyd](https://github.com/mmccoyd/hillside/).

The default keymap is described in
  [QMK](https://github.com/qmk/qmk_firmware/tree/master/keyboards/handwired/hillside/46).
  
For ZMK, the adjust layer has a few differences from the QMK version:

- Extra keys for bluetooth, reset and output.
- No swap Alt GUI keys.
- No RGB controls as RGB eats power.
- Bluetooth clear is deliberately in an inconvenient spot to avoid unpairing.

If used, the following must be manually enabled in hillside46.conf:

- Encoders
- Underglow

If desired, you could hardwire a display to the I2C header,
  which is arranged for a haptic feedback board.