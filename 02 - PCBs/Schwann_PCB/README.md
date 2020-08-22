# The Schwann PCB

![Schwann](https://cdn.discordapp.com/attachments/642426539824119849/690722239531974706/image0.jpg)

An ortholinear "HHKB" style PCB.  Specifically designed for use in the [Neuron 40% Keyboard](https://geekhack.org/index.php?topic=102681.0) by Walletburner of Geekhack. 

While not proprietary, the Schwann PCB has cut-off bottom corners and may not be compatible with many, current, after-market cases.  A Custom Designed case will most likely be the correct route. Acrylic is always a solid option.

## **Specs/Features**
- Powered By QMK Firmware (*Soon to be in QMK Configurator)
- Compatible and Designed for use with the Neuron Keyboard Case
- USB Type-C Connection
- x8 Optional WS2812B RGB LEDs
- No In-Switch LED Support
- Expansive Ortholinear Bottom Row Options
- and (IMO) A Beautiful PCB Aesthetically

## [**Non-Official QMK Firmware Documentation Can Be Found Here**](https://github.com/TheRoyalSweatshirt/The_Royal_QMK_Firmware_Vault/tree/master/In-Development_Boards/schwann)


## **Layout Options**
![Schwann_Layouts](https://i.imgur.com/H78IrGM.png)

## **Building**
This Repo was realeased to the public so that you can order some of these for yourself and skip the chain! Just upload the gerbers from the latest release section and send them to your favorite PCB Production facility ([JLCPCB](https://jlcpcb.com/) is a fantastic and Cheap Facility), Order the Components Listed below (My Personal Choice is [LCSC](https://lcsc.com/)), and solder up! 

*Thin Liquid Flux, Thin (.6mm Min Diameter) Solder, A Decent Soldering Iron/Station are required for a well function PCB and an intact sanity.

I am not responsible for anything DIY assembly you man do yourself.  This information is public so it is  between you and the PCB to decide who will be the victor.  Assemble safely and assemble confidently my friends!

## **Bill of materials (BOM)**
Amount is for a **SINGLE SCHWANN PCB**.

Multiply as needed for higher quantities.

| LCSC part # | Description   | Value   | Package  | Amount |
| ----------- | ------------- | ------- | -------- | ------:|
| C128353     | Capacitor     | 0.1uF   | 0805     | 3      |
| C215803     | Capacitor     | 1uF     | 0805     | 1      |
| C2099       | Diode         |         | SOD-123  | 48     |
| C20799      | Fuse          |         | 1206     | 1      |
| C165948     | USB Connector |         | SMD/THT  | 1      |
| C103904     | Resistor      | 10K     | 0805     | 2      |
| C147798     | Resistor      | 5.1K    | 0805     | 2      |
| C325772     | Resistor      | 22      | 0805     | 2      |
| C45874      | MCU           | 32U4-AU | QFN-44   | 1      |
| C32180      | Crystal       | 16MHz   | SMD-3213 | 1      |
| C127478     | RST_Switch    |         | SMD      | 1      |

***Optional/Other:**
| LCSC part # | Description   | Value   | Package  | Amount |
| ----------- | ------------- | ------- | -------- | ------:|
| C114585     | WS2812B       | RGB     | 5050     | 8      |

### **Note On Viewing PCB Documentation:*
The latest KiCAD version will be needed to view the PCB Docs.  As well as correct project file path configurations.