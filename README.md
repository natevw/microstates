# Microstates

[forward-looking statements follow]

It should be possible to deploy a new Thing to the Internet Of™ with a $10 bill-of-materials for a "bare server" and less than an hour of REST code customization.

Microstates lets tiny hardware play in the world of Raspberry Pi, letting each  wireless device act as an independent web server using [CoAP](http://tools.ietf.org/html/draft-ietf-core-coap-18) over a reasonably secure tiny data (<32 byte packets) transport layer.

## Hardware platform

Protype with Arduino, deploy using bare AVR chips and nRF24L01+ chips. Keep this flexible.

Assume a "base station" will serve as the gateway to the Internet. Keep chipside code short and sweet.

## Software platform

Arduino — a simple CoAP engine targetting communication over <https://github.com/gcopeland/RF24>

RasPi — start by wrapping <https://github.com/stanleyseow/RF24> in node.js module, write a CoAP transport for <https://github.com/natevw/fermata>

## Use cases

In order of current priority:

1. Aquaponics greenhouse monitoring system
1. -- sekrit [nodebots-tricites](https://tito.io/nodebots-tricities/2013) project --
1. Sous-vide/yogurt-making crockpot (controlled via iPod touch)
1. Wicking bed moisture sensors
1. Household energy usage stats
1. Lawn sprinkler mitigation
1. Solar system monitoring
1. Invisible ©Nest™® (?)

Basically I plan to start by "solving" silly suburban "problems" because that's all I got. If you have more valuable or more important use cases [please get in touch](http://exts.ch/).