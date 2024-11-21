Repository to store all code pertaining to the final project of EE456 - Digital Communications Laboratory, Cal Poly SLO.
This project contains code for a three-way link using raspberry Pi's, LoRa/GPS modules. 

   RPI 1:       |       RPI 2:        |     RPI 3:      
  LoRa TX       |      LoRa RX        |   TCP/IP Server
  GPS Module    |    TCP/IP Client    |

The first raspberry PI will have both a LoRa and GPS module. This rpi takes the GPS data from the GPS module
and transmits the GPS data across LoRa.

The second rpi has a LoRa module and an internet connection. This rpi will receive the GPS data sent by the
first rpi and send that data over TCP/IP internet connection. This rpi will be configured as a client.

The third and final rpi will just have an internet connection. This rpi will be configured as a server,
to collect the GPS data sent by the second rpi over internet.

In total, the GPS data is collected by the first rpi, sent to the second over LoRa, which then sends
the data to the third over an internet connection.

This project was created by Sammy Brunton, Alejandro Cosper, Colin Lucio, and Mont Murad.
