<picture>
  <source media="(prefers-color-scheme: dark)" srcset="/docs/images/TOTEM_logo_dark.svg">
  <source media="(prefers-color-scheme: light)" srcset="/docs/images/TOTEM_logo_bright.svg">
  <img alt="TOTEM logo font" src="/docs/images/TOTEM_logo_bright.svg">
</picture>

# ZMK CONFIG FOR THE TOTEM SPLIT KEYBOARD

[Here](https://github.com/GEIGEIGEIST/totem) you can find the hardware files and build guide.\
[Here](https://github.com/GEIGEIGEIST/qmk-config-totem) you can find the QMK config for the TOTEM.

TOTEM is a 38 key column-staggered split keyboard running [ZMK](https://zmk.dev/) or [QMK](https://docs.qmk.fm/). It's meant to be used with a SEEED XIAO BLE or RP2040.


![TOTEM layout](/docs/images/TOTEM_layout.svg)



## HOW TO USE

- fork this repo
- `git clone` your repo, to create a local copy on your PC (you can use the [command line](https://www.atlassian.com/git/tutorials) or [github desktop](https://desktop.github.com/))
- adjust the totem.keymap file (find all the keycodes on [the zmk docs pages](https://zmk.dev/docs/codes/))
- `git push` your repo to your fork
- on the GitHub page of your fork navigate to "Actions"
- scroll down and unzip the `firmware.zip` archive that contains the latest firmware
- connect the left half of the TOTEM to your PC, press reset twice
- the keyboard should now appear as a mass storage device
- drag'n'drop the `totem_left-seeeduino_xiao_ble-zmk.uf2` file from the archive onto the storage device
- repeat this process with the right half and the dongle

Dongle Code from:
https://github.com/BertPlasschaert/zmk-config-totem-dongle

## USE WITH DONGLE
(from https://www.reddit.com/r/ErgoMechKeyboards/comments/1evno9r/wireless_totem_first_build_dongle_question/?tl=de&utm_source=share&utm_medium=web3x&utm_name=web3xcss&utm_term=1&utm_content=share_button)

1. Flash Dongle w/ settings reset
2. Flash Left w/ settings reset (power On)
3. Flash Right w/ settings reset (power On)
4. Flash Right with firmware
5. Press Right Reset Button
6. Wait 20 seconds
7. Flash Left with firmware
8. Press Left Reset Button
9. Wait 20 seconds
10. Flash Dongle with Firmware

## Nice!View Screen
This Version supports a Nice!View screen for the dongle. With the support of [mctechnology17s repo](https://github.com/mctechnology17/zmk-dongle-display-view).
The wiring is shown below.

