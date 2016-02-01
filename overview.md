---
layout: default
title: "Koruza Overview"
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

##System assembly

The design exploits the bi-directional optical path via a single plano-convex lens, as SFP Bi-Di modules inherently have coaxial receiving and transmitting optical axes for aiming the collimated beam at a distant complementary pair, that places the focal point of the received beam sufficiently in the SFP module focal point. The infra-red collimated beam is experimentally aligned with manual theta-phi stage to be parallel with the green auxiliary laser beam, that is used as a visual aid for initial coarse manual alignment. By exploiting the SFP module digital monitoring mode, the received IR optical power is monitored by the control system, establishing the IR beam lock-in condition after initial manual aiming using the green aiming laser. Based on the real-time received optical power, the units are precisely aligned with motorized X and Y micrometer stages to maximize the optical power.

Mechanical construction of the system is designed to be fully 3D printable to enable easy modification and experimentation, as well as to decrease the system cost. An innovative approach combining precision screws and low-cost stepper motors enables micrometer precision alignment in X and Y axis translating to angular displacement of the inner movable arm with pivot mounting in front. F axis linear translation of the SFP module inside the inner structure adjusts the collimation of the laser beam. The outer enclosure is designed to be cut from stock aluminium elements and acts as a manual coarse alignment stage, to align the units within the motorized movement range.

Control electronics system connects to the SFP module via the digital diagnostic interface collecting temperature, Transmitter/Reciever (TX/RX) power measurement, interfacing stepper modules as well as a range of sensors for environmental sensing.

Environmental sensor range is deployed to observe and measure a number of parameters that could potentially affect system performance and are particularly useful for debugging and research purposes. This includes sensors for detecting mechanical disturbances and movement as well as meteorological sensors for observing the micro-climate.

A Wi-Fi router running an open source OpenWRT firmware is used to collect and store the measurements, generate traffic for packer error rate monitoring and send data real-time to a monitoring system.
