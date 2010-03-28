# mySDR Baseband Software Defined Radio Modem

mySDR is a new project to create a fully open source baseband modem for software defined radio.
The plan is to provide a range of performance options to pick and choose from such that the radio,
can be somewhat customized for the best "bang for your buck".

The project will target [GNU Radio](http://gnuradio.org "GNU Radio") compatibility as well as
being a drop-in replacement for the USRP.

## Specifications
* [Analog Devices](http://www.analog.com/en/analog-to-digital-converters/ad-converters/ad9251/products/product.html "AD9251") Dual Channel 14-bit Analog to Digital Converter
    * Full 700MHz Analog Input Bandwidth
    * Family compatible for 20/40/65/80 MHz sampling options
* [Analog Devices](http://www.analog.com/en/digital-to-analog-converters/da-converters/ad9717/products/product.html "AD9717") Dual Channel 125MHz Digital to Analog Converter
    * Family compatible for 8-/10-/12-/14-bit options
* [Altera Cyclone III](http://www.altera.com/products/devices/cyclone3/overview/cy3-overview.html "Altera Cyclone III") FPGA
    * Up to 1,134 kbits of internal BRAM
    * Up to 126 18x18 multipliers
    * Up to 39,600 total logic elements
* Flexible Clocking Solutions
    * [FOX924B](http://www.foxonline.com/pdfs/fox924.pdf "FOX924B PDF") 25MHz TCXO standard
    * [FOX801BHCLF](http://www.foxonline.com/pdfs/FOX801BHCLF.pdf "FOX801BHCLF PDF") 25MHz low phase-noise &plusmn;2.5ppm VCTCXO option
    * [Si5338](http://www.silabs.com/products/clocksoscillators/anyrategeneratorsandbuffers/Pages/default.aspx "Si3558") Clock buffer/generator for flexible RX/TX sample rates
* [Vitesse](http://www.vitesse.com/products/product.php?number=VSC8601 "VSC8601") 10/100/1000 Ethernet PHY
* [Atmel SAM3U](http://www.atmel.com/products/AT91/sam3landing.asp "Atmel SAM3U") USB 2.0 High-speed ARM Cortex-M3 microcontroller
* Compatible with [Ettus Research](http://www.ettus.com "Ettus Research") RF daughterboards

## Required Software
* [TinyCAD](http://tinycad.sourceforge.net/ "TinyCAD") for schematic capture
* [FreePCB](http://www.freepcb.com/ "FreePCB") for PCB layout
* Atmel SAM3U GNU GCC Software Package (not available yet)
* [Quartus II](http://www.altera.com/products/software/quartus-ii/web-edition/qts-we-index.html "Quartus II") for FPGA programming

## To Do
* Hardware
    * <strike>Parts selection</strike>
    * Schematic
        * <strike>Symbol creation</strike>
        * Connections
        * BOM
    * PCB
        * Footprint creation
        * Routing
* Software
    * Microcontroller
        * Diagnostic UART
        * microSD Driver
        * FPGA Bootloader
        * USB Driver
    * FPGA
        * RX Signal Chain
        * TX Signal Chain
        * 10/100/1000 MAC
    * GNU Radio
        * USRP-like compatible host drivers
        * Integration
        * Testing
* Documentation
    * Detailed Design