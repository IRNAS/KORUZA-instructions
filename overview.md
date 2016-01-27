---
layout: default
---

# Understanding the technical operation of KORUZA
Wireless optical system KORUZA is designed for low-cost gigabit communication over the distance of 100m. See [project website](http://koruza.net) for complete specification and introduction. Wireless optical communication is a good alternative to radio based systems in highly populated ares which likely suffer from radio spectrum congestion.

## Basics of wireless optical communication
Sending data witout the use of wires has shown to be very convenient as laying cables requires time and money. While there is good economic reasoning to do this between larger clusters of buildings ie. cities, running a cable to every single building is a lot of effort. Wireless services that do not require a fixed connection to buildign or users are becoming more and more popular, however wireless radio communications have insuccicient capacity to meet the demand as the devices at close range jam eachother.

Wireless optical communication for connecting buildings is however different. The frequency/wavelength of light allows us to make a very small and directed beam at reasonably large distances, thus enablign us to send information with it directly to the receiver without any spill to the surrounding area.

## Basics of KORUZA optical communication

KORUZA produces an optical beam approximately 3cm in size that does not change in diameter with distance - is collimated. The infrared optical wavelengths used are 1330nm or 1550nm, typically used in wired fiber networks. These are invisible by eye and even with conventional smartphone cameras. The optical power of the transmitter is very low, sub 1mW and thus completely eye-safe. 

Two KORUZA units are used such that they are a matched pair, one transmitting at 1330nm and receiving at 1550nm while the other transmitting at 1550nm and receiving at 1330nm, allowing us to establish a completely bi-directional optical link using a single lens on either unit.

To be able to install the system in real-world aplication as it uses an invisible optical beam, there is a secondary green laser in each unit, which we turn on to see where the invisible infrared beam is pointing. When the units were assembled a calibration procedure is used to make sure they both point in the same direction.

