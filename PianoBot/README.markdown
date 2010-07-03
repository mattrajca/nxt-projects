PianoBot
========

A simple NXT robot that can play a given tune on a piano keyboard. Watch a [video]() of it in action!

Building Instructions
---------------------

1. PianoBot uses a 4x4 chassis as its base. Instructions for building one can be found on the NXT Programs [website](http://www.nxtprograms.com/4x4_chassis/steps.html).
2. Follow steps 10-11 found [here](http://www.nxtprograms.com/4x4_joystick/steps.html) to mount the NXT brick on the chassis.
3. Up-close pictures of the robot's "finger" can be found on my [Flickr page](http://www.flickr.com/photos/mattrajca/sets/72157624362797274/). The motor powering the "finger" should be connected to port A.
4. The source of the NXC program can be found in this git repository under the PianoBot subfolder.

Usage
-----

Before playing any song, make sure the robot's "finger" is lined up with the middle-C.

Song Files
----------

Songs themselves are stored in separate 'sng' files. Each line in a song file consists of a note value (> 1, see pianobot.nxc) and a duration (in milliseconds). These are separated by a space. Each line is terminated by a space as well, and the file is terminated with an empty line. To include a "rest", use a note value of 0.

Limitations
-----------

Motor rotations can be imprecise as the motors tend to overshoot the actual angle given. I made an effort to make playback as accurate as possible, but if anyone has any ideas on improving this furthermore, please drop me an email.
