# 1.2og repro pcb

unfinished attempt to re-create pcb and lightbar for matrix 1.2og.

pcb edge cuts are provided courtesy of astro of matrixlab [here](https://geekhack.org/index.php?topic=106122.msg2901076#msg2901076). it has 19.02mm spacing (mostly) based off those edge cuts. stm32f072 schematic is courtesy of xphoenixd. schematic for ws2812c-2020 rgb chain is courtesy of zykrah's [fuyu](https://github.com/zykrah/fuyu). voltage stepdown thing for lightbar is lifted from dededecline and olivia's [sst60](https://github.com/dededecline/SST60).

indicator LEDs on scroll lock and caps lock. JST is s3b ph 3 pin, since that's what it looks like from watching youtube build videos. split backspace and split right shift are included in spite of default plate not including those positions. iso is not included in spite of default plate including those positions. usb port placement is mostly based off guesswork and eyeballing it. there's also a nice little reset jumper beneath the space bar. also included is a little pad to ground on the back, in case you think you can add conductive foam to case to route esd shorts to ground. maybe you can solder some wire to a mounting screw or something, i don't know. this thing costs like over a hundred bucks to proto at jlcpcb and i don't have that kinda cash yet. the routing is extremely messy.

lightbar mounting holes on PCB are slightly off-spec, and are plated m3 (edge cuts seem to imply the hole is a bit wider).

i don't know if i'm allowed to license this, given the pcb edge cuts this is based off of were released without a license.

this is completely untested.

## todo

1. fill out BOM?
1a. measure and source standoffs that are good enough and ultra low profile screws
2. split main pcb and lightbar pcb separately so jlcpcb production files don't keep bothering each other
3. adjust placement of diodes
4. consider alternative to ws2812 2020
5. consider pico ezmate or something instead of jst-ph + directly soldered cable
6. prototype PCB and lightbar
7. firmware (come on, this is basically automated at this point)
8. verify this works with original lightbar

