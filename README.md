# Hillside ZMK firmware

![hillside](https://imgur.com/emWDXiT.png)
[![Build](https://github.com/mmccoyd/zmk-config/actions/workflows/build.yml/badge.svg)](https://github.com/mmccoyd/zmk-config/actions/workflows/build.yml)

This is the [ZMK](https://zmk.dev/docs) firmware
 for the [Hillside](https://github.com/mmccoyd/hillside) family of split ergonomic keyboards.

It contains keymap definition files for two boards in [./config](./config):

 - Hillside 52 with 3x6+3+5 keys
 - Hillside 48 with 3x6+1+5 keys

Pushing changes will build both keyboards. Comment out one of the keyboards in [./build.yaml](./build.yaml) if you need only one.

To build the firmware:

- Fork this repo on GitHub
- Clone your fork locally
- Trigger a build:
  - Make a trivial change to ./build.yaml (or any non *.md file)
  - Push that change
- Look in the actions tab for the build triggered by that change
- Wait for the build to finish
- Click on the build link
- Download the artifact file with the firmware
- See [Installing The Firmware](https://zmk.dev/docs/user-setup#installing-the-firmware)
  for more details from there.

*Once* your board works with the default firmware,
  you can modify the keymap.
Your copies of the default Hillside keymaps are in:

- [./config/hillside52.keymap](./config/hillside52.keymap)
- [./config/hillside48.keymap](./config/hillside48.keymap)

Modify those as needed. Pushing the change will trigger a build as above.

If you want to enable features,
  modify the appropriate config file:
 ./config/hillside48.conf or ./config/hillside52.conf.

To add RGB support, uncomment the lines in the ./config/hillside**.conf file
  and add the ```&rgb_ug RGB_TOG``` and other keycodes to the keymap adjust layer.
While RGB is disabled, any RGB control keys
  behave as transparent keys and activate keys on lower layers,
  which can be confusing.

The Hillside 48 and 52 shield definition files *should not* need to be modified and are in ./config/boards/shields.

More information about each keymap is in their readme files.
