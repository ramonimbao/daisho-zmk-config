# zmk-config for RMI-KB

This is a repository for RMI-KB keyboards that use ZMK.

## Andrea

1) Edit the `andrea.keymap` file to change your keymap.

- https://zmkfirmware.dev/docs/behaviors/key-press
- https://zmkfirmware.dev/docs/behaviors/layers
- and pretty much everything in the "Behaviors" section, plus
- https://zmkfirmware.dev/docs/codes/

2) Head over to the Actions tab at the top of the repository.

3) Click on the latest workflow run.

- If you did your keymap correctly, there should be a green checkmark to the left.

4) Check the back of your PCB for the date on the lower left corner for the date marking.

- Currently either 31 Mar 2021, or 14 Apr 2021.

5) Click on the relevant firmware file to download. Unzip it somewhere too.

6) Plug the USB connector in, and double press the reset button twice quickly (Has to be <500 ms apart).

- The reset button is located underneath the right spacebar.

7) Drag and drop the UF2 file you unzipped to the mass storage device that appeared.

- I think it's named `NRF52BOOT` or something?
- Whatever the name, there should be a UF2 file inside. Don't delete or anything, just drag and drop the new Andrea firmware file to the mass storage device.