# GroveEncoder Library

A project to enable the Grove Encoder v1.2 hardware to work simply on Arduino. You can find information about the [Grove Encoder here](http://wiki.seeed.cc/Grove-Encoder/).  The library included by the manufacturer didn't run on my Arduino101, so I wrote this new one from scratch.

# Hardware requirements

- Arduino101/Genuino101
- Grove Shield and a cable
- Grove Rotary Encoder v1.2

## Recommended hardware setup

1. Put the Grove Kit Shield in the Arduino101
2. Plug one side of the cable into the D7 port on the Grove Shield
3. Plug the other side of the cable into the Grove Rotary Encoder v1.2
4. You're done!  Power it on and start programming.

# Installation

Download the ZIP and install using the Arduino IDE.  Alternative 
installation instructions may be found [here](https://www.arduino.cc/en/Guide/Libraries).

# Usage

You can use this library via polling, or attach an interrupt handler if you're an advanced user.

Please see the examples directory.

## Polling

Simply create a GroveEncoder object and pass NULL as the second parameter.

## Interrupts

Create a GroveEncoder object and pass it a pin as well as a callback.

# Limitations

- Currently you can only use one GroveEncoder per platform.
- This has only been tested on Arduino101.  However, I haven't done anything 
  specifically to prevent this from working on other Arduino versions.

# License

See LICENSE.
