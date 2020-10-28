
# The-Little_Foot-Keyboard-rev2.3-PCB Gerbers

![Little_Foot](https://i.imgur.com/GC1st7U.png)
===

**PCB Dimensions:** `190.5mm x 95.3mm`
===

## Required Parts for PCB & PCB Assembly:

+ **x40-44** - 1N4148 Diodes (PCB Supports both/either SMD and THT Diodes)
  
   - LCSC SMD Diodes: [C2099](https://lcsc.com/product-detail/Switching-Diode_Changjiang-Electronics-Tech-CJ-1N4148W_C2099.html)

   OR*

   - LCSC Through-Hole Diodes: [C14516](https://lcsc.com/product-detail/Switching-Diode_1N4148_C14516.html)

.

.

.

+ **x1** - SMD Flat Tactile Switch (Reset)

   - LCSC Reset Switch: [C92584](https://lcsc.com/product-detail/Tactile-Switches_Korean-Hroparts-Elec-K2-1187SQ-A4SW-06_C92584.html)

   OR*

   - Reset Switch [MSLPT5252AG2TR](https://www.mouser.com/ProductDetail/506-MSLPT5252AG2TR)

.

.

.

+ **x1** - Elite-C (USB_C) or Pro-Micro Variant (Micro_USB)

   - Pro Micro [Clone from Amazon](https://www.amazon.com/KeeYees-ATmega32U4-Development-Microcontroller-Bootloader/dp/B07FXCTVQP/ref=sr_1_3?dchild=1&keywords=pro+micro&qid=1589765488&sr=8-3)

+ **x2** - 12P-2.54mm Header-Pin Connectors (Most controllers already come with these)

+ **x41 or x44** - Cherry MX compatible key switches

   - Cherry MX Switches [Cherry MX Clear](https://www.mouser.com/ProductDetail/540-MX1A-C1NW) 

## Optional Parts:

+ **x10-x20** WS2812b RGB LEDs (Strip) 

   - [Kingly-Keys RGB Strips](https://kingly-keys.xyz/collections/parts-and-pieces/products/ws2812b-leds-strip)
   
.

.

.

+ **x2** - 2u Stabilizers (GMK Brand *screw-in* Preffered)

OR*

+ **x1** - 7u Stabilizer (GMK Brand *screw-in* Preffered)

   - [Novelkeys Stabilizers](https://novelkeys.xyz/collections/miscellaneous/products/cherry-stabilizers?variant=3747938893864)
   


## Build Guide
0. Orient yourself with the board. You're looking at the **top**  of the PCB when the Little Foot emblem is visible on the **right side** of the board.

1. Solder in diodes, making sure to orient them according to the silk screen on the board. You should solder them on to the bottom of the board (with leads coming out of the top of the board) because there are 2 diodes which will interfere with switches if soldered to the top.

2. Take the pin headers that came with your Pro Micro and push LONG ends through the BACK of the PCB, so that the black plastic spacers are on the back side of the PCB. Solder to the pins poking through the FRONT of the board. I like to use a small piece of tape to hold the pins in place while I solder, otherwise the headers might fall out of the holes when the board is flipped over to solder.

 When the build is finished, the Pro Micro will sit on top of the black plastic spacers now on the back of the PCB.  

3. Solder in pin headers or pin sockets for an RGB strip if you're using one. The pins/sockets should be mounted on the bottom off the board, so that you can plug in your RGB strip there.

4. Install stabilizers (either 2x 2U or 1x 7U depending on your spacebar configuration). Ensure they are mounted on the **top** of the board.

5. Solder on the reset switch. I find it's easiest to do this by applying a tiny (tiny!) blob of solder to the pads first, then using tweezers to hold the switch and solder the pins to the solder blob on the board.

6. If you're building this with a plate, now is the time to put all your switches in the plate, and then use that to align all the switch pins with their holes on the board. 

 If you're building this without a plate, you can mount all the switches in their holes and use a piece of flat cardboard or plastic to help you flip the PCB over without any of the switches coming out of the holes.

 Solder the switches in place.

7. Put the pin headers coming from the PCB through the holes on the microcontroller. The components and socket on the microcontroller should be facing away from the PCB, with the USB port facing towards the top of the PCB. You can double check that everything is facing the correct direction by making sure the TX and RAW labels on the PCB line up with the corresponding holes on the microcontroller. The microcontroller should rest on the black pin spacers placing it just above the PCB, with enough space for the diode and switch leads under it.

8. Flash micro controller firmware if not already done. In my experience with these Pro Micro clones it helps to hold the reset button, then run the programmer command, then release the reset button. The programmer should recognize the board and flash it. I use the following command on my Ubuntu 16.04 system: 

 ```
sudo avrdude -F -p atmega32u4 -P /dev/ttyACM0 -c avr109 -U flash:w:kingly_keys_little_foot_default.hex
```

9. Header over to [Keyboard Tester](https://keyboardtester.com) and ensure that all the keys are registering. If some of the switches are not registering, check to ensure that you do not have any incomplete or cold solder joins on your switch pins. Additionally, check to make sure the keymap in your firmware matches the switch layout that you installed.

 At this point your PCB is fully assembled, and you can install it in a case of your choice. 