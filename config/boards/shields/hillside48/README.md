Hillside48 is a split ergonomic keyboard with 3x6+4+2 choc-spaced keys.
It has the aggressive stagger of the Ferris but a longer thumb arc and a break-off outer pinkie column.
More information is at [github/mmccoyd](https://github.com/mmccoyd/hillside/).

The default keymap is described in
  [QMK](https://github.com/qmk/qmk_firmware/tree/master/keyboards/handwired/hillside/).
  
For ZMK, the adjust layer has a few differences from the QMK version:

- Extra keys for bluetooth, reset and output.
- No swap alt gui keys.
- No RGB controls as RGB eats power.
- Blue tooth clear is deliberately in an inconvient spot to avoid unpairing.

If used, the following must be manually enabled in hillside48.conf:

- Encoders
- Underglow

If desired, you could hardwire a display to the I2C header,
  which is arranged for a haptic feedback board.
