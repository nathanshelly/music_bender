# Music Bender

_Built for Professor Pardo's Digital Luthier @ Northwestern University_

A project for gestural control of audio in real time giving one the opportunity to play with sound and shape their listening experience. There are five controllable parameters - volume, pitch, filter, reverb & chorus. To manipulate audio you first use a gesture to activate a parameter mode (these can be stacked to allow manipulation of multiple at once) then move your hand to adjust the parameter value(s).

## Example

The below video shows a user playing with an example song - [Better Not (feat. Wafia) by Louis The Child](https://www.youtube.com/watch?v=YhZoPauDUg0).

[![Better Not](https://img.youtube.com/vi/0Keh37kdcuI/0.jpg)](https://www.youtube.com/watch?v=0Keh37kdcuI)

## Interface

![Interface](https://raw.githubusercontent.com/nathanshelly/music_bender/assets/images/interface.png "Interface")

## Motivation

This project enables interactive experience of music, more poetically (and aspirationally) playing with music. Music Bender provides an easy way to manipulate high level properties of audio that doesn't require expensive hardware or software. The gestural interface prioritizes simplicity and the intuition of moving to music.

The final interface is intended to be usable by anyone regardless of musical knowledge. Even the effect of musically esoteric parameter values like LFO (ow frequency oscillator) centre can be intuitively understood through experimentation without underlying knowledge of the concept.

## Usage

Load up any audio then trigger (and untrigger) modes by holding out the appropriate number of fingers in your left hand (specified along with the mode name in the interface) and clenching your right hand into a fist. Each mode's parameter's are modified by your right hand's position along one or more of the XYZ axes.

0 fingers bypasses all modes to hear the original audio and simultaneously resets all parameters for a fresh start to manipulation.

## Building

This project was built using Max MSP & a Leap Motion controller. Leap Motion data is fed to Max using a slightly modified version of [Jules Francoise's](https://github.com/JulesFrancoise/) fantastic [Leapmotion For Max](https://github.com/JulesFrancoise/leapmotion-for-max) patch.

## Future

There are a few things I would love to improve on in future iterations. If you have any suggestions please feel free to open an issue or pull request!

1. Add more parameters and gestures - the current set of five allow for broad modification but there exist many more modulatable parameters one might want. Additionally, the number of fingers + clenched fist gesture scheme works the most reliably of those I tried but is inherently limited to 5 fingers. And even though it's the most reliable that doesn't mean it has no flaws. The Leap sometimes fails to recognize changes to the number of fingers or simply miscounts (these errors can even be seen in the demo video above).
2. Make the interface more visual - one can see the values of parameters as raw number but visuals that mapped somehow to the parameter the user is modulating would make the interface both more enjoyable to use and easier to pick up for newcomers.
