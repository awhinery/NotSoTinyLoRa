Having modified this lib continually, I made a fork to hold the modifications. 

Ada's version as of this fork, has a non-TTN-compatible set of data rates defined. One mod I will make is to make the available data rates match the TTN channel plan. 

Another is to make a define "diagnostics" so that one can sweep a gateway to collect a complete list of channels and data rates it receives on. 

Another is optimizing the LoRa transceiver mote as an I2C slave, so that a master can control several slaves, provide timing and GPS position to several slaves, and monitor whether packets get sent. This is because the problem with such survey tools as TTNMapper is that they don't show failed attempts.

As the University Of Hawaii explores providing LoRaWAN coverage to the community and researchers, we will develop one or more other Gits to store as-tested code and hardware specs. 

Alan Whinery - 09-27-19, (with no code mods completed). 

# Adafruit TinyLoRa Library [![Build Status](https://travis-ci.com/adafruit/TinyLoRa.svg?branch=master)](https://travis-ci.com/adafruit/TinyLoRa)


Library for communicating with [The Things Network](https://www.thethingsnetwork.org/) using a Hope RF RFM95/96/97/98(W) LoRa Transceiver Module.

## Documentation/Links

The Doxygen documentation is automatically generated from the source files
in this repository, and documents the API exposed by this driver. For
practical details on how to connect and use this sensor, consult the Learning
Guide.

- [Adafruit Learning Guide](https://learn.adafruit.com/the-things-network-for-feather)
  (Installation details for Feather 32u4/Feather M0.)
- [API Documentation](https://adafruit.github.io/TinyLoRa/) (automatically generated via doxygen from source)
- [Adafruit Feather 32u4 RFM95 LoRa Radio](https://www.adafruit.com/product/3078)
- [Adafruit Feather M0 with RFM95 LoRa Radio](https://www.adafruit.com/product/3178)

## License

This library was written by [ClemensRiederer](https://github.com/ClemensRiederer/TinyLoRa-BME280). We've modified it to support channel/datarate selections and made small changes so it works with the Adafruit Feather 32u4 LoRa and the Adafruit Feather M0 LoRa. We've added examples for using this library to transmit sensor data over a single channel or multiple channels to The Things Network.

This open source code is licensed under the LGPL license (see [LICENSE](LICENSE)
for details).
