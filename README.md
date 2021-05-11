# ZMK Config for GW01 boards

This is the repository for GW01 boards (main and macro pad).

First, fork the repository by clicking on the `Fork` button on the upper right, then proceed to make any changes you need.

## Main Board

[](images/gw01-main-keymap.png)

1) Edit the `config/boards/arm/gw01_main/gw01_main.keymap` file to change your keymap.

- https://zmkfirmware.dev/docs/behaviors/key-press
- https://zmkfirmware.dev/docs/behaviors/layers
- and pretty much everything in the "Behaviors" section, plus
- https://zmkfirmware.dev/docs/codes/

2) Head over to the Actions tab at the top of the repository.

3) Click on the latest workflow run.

- If you did your keymap correctly, there should be a green checkmark to the left.

5) Click on the relevant firmware file to download. Unzip it somewhere too.

6) Plug the USB connector in, and double press the reset button twice quickly (Has to be <500 ms apart).

- The reset button is located underneath the right spacebar.

7) Drag and drop the UF2 file you unzipped to the mass storage device that appeared.

- I think it's named `NRF52BOOT` or something?
- Whatever the name, there should be a UF2 file inside. Don't delete or anything, just drag and drop the new firmware file to the mass storage device.

## Macro Board

[](images/gw01-macro-keymap.png)

- Yes, there's only one layer by default. I didn't really know what to put.

- Basically the same as above, except edit the file `config/boards/arm/gw01_main/gw01_macro.keymap`.

- Change the behavior of the rotary encoder by changing the line `sensor-bindings = <&inc_dec_kp XXXX YYYY>;`

- If the encoder behavior is inverted, just switch the `XXXX` and `YYYY`. Uses the same keycodes as the ones linked above.