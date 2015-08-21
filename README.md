//This repo has been forked from the original to accomodate changes in GUI and possible changes to reolution
The below is a 63Hz PWM signal with the current arduinoscope version.  Goal would be to allow the user to zoom in to better see the signal.

![PWM](http://s24.postimg.org/7yux62xv9/oscope.png)

Credits go to https://github.com/konsumer/arduinoscope for the original arduinoscope

# Arduinoscope

This is the current version of my Arduino-powered, low-resolution, multi-channel oscilliscope. I made 2 frontends, that both speak [firmata](http://firmata.org), so you will need to install the Firmata firmware on your Arduino (File -> Open -> Examples > Library-Firmata > StandardFirmata, in latest Arduino IDE.)

It used to run over a simple serial protocol, but I have decided to standardize on Firmata, so I can keep the pin-reading code in the client, and make installation more standardized.

The basic idea with both front-ends is to connect your Arduino running Firmata, and start the front-end.

## Standalone

If you don't care about developing the front-end, or don't want to install any dependencies, or do anything other than just have a working oscilliscope, choose the correct "standalone" zip file for your plaform from [here](https://github.com/konsumer/arduinoscope/releases/).


## Processing

This is a up-to-date port of my original oscilliscope. It is also the current source for the stand-alone apps.

If you want to modify the processing front-end, see [instructions](https://github.com/konsumer/arduinoscope/tree/master/processing).


## Node

This is my new and favorite GUI for Arduinoscope.  You will need to install [node.js & npm](http://nodejs.org/download/) and follow the [instructions](https://github.com/konsumer/arduinoscope/tree/master/arduinoscope.nw/) for that frontend.

## Modification

This is by no means the most efficient or best osciloscope you can build. It's meant to be simple & easy to modify, so you can do whatever you want with it. Checkout [this wiki article](https://github.com/konsumer/arduinoscope/wiki/Modification) to see how to easily read a different voltage range, for example.


