# zhol/backup_plan/beta

![zhol/backup_plan/beta](https://i.imgur.com/BNG3y6t.png)

A prototype version of a drop-in replacement for the Matrix 1.2OG.

* Keyboard Maintainer: [zhol](https://github.com/zhol0777)
* Hardware Supported: APM32F072
* Hardware Availability: [Github](https://github.com/zhol0777/1.2og_pcb_clone)

Make example for this keyboard (after setting up your build environment):

    make zhol/backup_plan:default

Flashing example for this keyboard:

    make zhol/backup_plan:default:flash

See the [build environment setup](https://docs.qmk.fm/#/getting_started_build_tools) and the [make instructions](https://docs.qmk.fm/#/getting_started_make_guide) for more information. Brand new to QMK? Start with our [Complete Newbs Guide](https://docs.qmk.fm/#/newbs).

## Bootloader

Enter the bootloader in 3 ways:

* **Bootmagic reset**: Hold down the key at (0,0) in the matrix (usually the top left key or Escape) and plug in the keyboard
* **Physical reset button**: Press and hold the reset button on the rear of the pcb (or short the reset jumper beside the spacebar key) for at least 3 seconds.
* **Keycode in layout**: Press the key mapped to `QK_BOOT` if it is available
