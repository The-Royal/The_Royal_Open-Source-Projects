
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
1. Solder in diodes, making sure to orient them according to the silk screen on the board. You could solder them to the top or bottom of the PCB according to your preference.
2. Install stabilizers (either 2x 2U or 1x 7U depending on your spacebar configuration). Ensure they are mounted on the **top** of the board.
3. Solder in the 2x Cherry MX compatible switches which overlap the footprint of the micro controller.
4. Solder in the micro controller, or micro controller socket if you choose to use one. Note that using a socket will increase the height of the micro controller on the board and may not be compatible with the pre-designed cases in this repository.
5. Solder on the reset switch.
6. Flash micro controller firmware if not already done.
7. Now is a good time to go to [Keyboard Tester](https://keyboardtester.com) and ensure that all your keys are registering. You can do this by shorting together the switch pins with tweezers or a piece of wire.
8. Solder in remaining Cherry MX compatible switches.
9. Header over to [Keyboard Tester](https://keyboardtester.com) and ensure that all your keys are registering, if you didn't do it in an earlier step. 
