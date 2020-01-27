# Clock Nakytec

Welcome to Flutter Clock Nakytec!

This repository is a clean repo from https://github.com/akilinomendez/flutter_clock_nakitec.git submitted for the competion https://flutter.dev/clock

##  The idea

I live in some small islands of Spain, I wanted to represent something of my land, Lanzarote island in the Canary Islands.
A cycle with a photo was the option, The photo was provided by Juan Carlos Reyes (https://www.flickr.com/photos/carlosrobayna/):

![lanzarote](https://github.com/akilinomendez/flutter_clock_nakytec/raw/master/original.png)

The idea was to convert this image to svg and cartoon:

![lanzarote](https://github.com/akilinomendez/flutter_clock_nakytec/raw/master/lanzarote.png)

## The animation 

For the animations of the cycle I needed something powerful, that's where app.rive is strong.
The project is free and visible: https://rive.app/a/aki/files/flare/ciclo-lanzarote

## Programing

- The sunrises at 6:00 and the sunsets at 18:00,  the sun is at the top center of the screen at 12:00, to adjust the times to the second 0 of the animation is subtracted from the current time 6 hours.

- The moon phases were a headache, try a thousand ways,due to the restrictions of the competition I could not use ethernet, but thanks to the following repository (https://github.com/ryanseys/lune), this is a calculation of moon state in javascript, convert all code to dart in https://github.com/akilinomendez/flutter_clock_nakytec/blob/master/nakytec_clock/lib/helpers/moon_phase.dart

- For reasons of time it was not possible for me to do all the animations I would have liked, for now:
    * Raining
    * Cloudy
    * Snowing 
All others are based on these, special mention to snowing, the code was taken from the following repository https://github.com/windwp/flutter-snow-effect


## Use

The app has two options demo and normal, in normal weather changes must come from the api in this case flutter clock helper and  it works like a clock and marks the daily time and position of the moon and sun. In demo the cycle is accelerated and the weather changes are random
