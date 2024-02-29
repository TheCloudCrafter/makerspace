# Build notes

# Shortcomings

## Fan speed controller

Attempted to use a PWM fan controller to manage fan speed.  
PWM Fan controllers require fans that have 4pin and not 3pins.  
3 pin fans are missing the speed controller chip required for the PWM Fan controller.

Switched to a standard DC motor controller.  
Shortcomings are PC fans don't start spinning until ~1.5 volts which is about 10%~15% on the controller knob.  
Good enough.

## Wiring

Instead of purchasing spools of wire to run the system. This is a low voltage solution and I have ethernet spools from a previous career. Cat6 ethernet cable is rated for PoE. 60 W of power per pair.

https://en.wikipedia.org/wiki/Power_over_Ethernet#Single-pair_Ethernet

    Single-pair Ethernet

    The IEEE 802.3bu-2016[13] amendment introduced single-pair Power over Data Lines (PoDL) for the single-pair Ethernet standards 100BASE-T1 and 1000BASE-T1 intended for automotive and industrial applications.[14] On the two-pair or four-pair standards, the same power voltage is applied to each conductor of the pair, so that within each pair there is no differential voltage other than that representing the transmitted data. With single-pair Ethernet, power is transmitted in parallel to the data. PoDL initially defined ten power classes, ranging from 0.5 to 50 W (at PD).

    Subsequently, PoDL was added to the single-pair variants 10BASE-T1,[15] 2.5GBASE-T1, 5GBASE-T1, and 10GBASE-T1[16] and as of 2021 includes a total of 15 power classes with additional intermediate voltage and power levels.[15]

https://www.eenewseurope.com/en/new-automotive-power-over-ethernet-standard-extends-wattage-range/

    Single pair Ethernet was initially developed to support automotive manufacturer’s increasing demand for Ethernet connectivity in vehicles, and IEEE 802.3bu-2016 defines specifications and parameters for adding up to 60 W of power to that cabling.

## Power source

SmoTecQ 12V 2A Power Supply AC Adapter, AC 100-240V to DC 12 Volt Transformers, 2.1mm X 5.5mm Wall Plug (12 Volt - 2amp - 2pack)  
https://a.co/d/dJlWppt  
![](https://m.media-amazon.com/images/I/61vPmtoGlQL._AC_SL1200_.jpg)

# Lessons learned

Calculate total system load in watts to avoid issues.

