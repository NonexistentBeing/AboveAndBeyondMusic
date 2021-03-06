# The magic of sound

## Sound

Probably the best way to begin is by defining sound itself.

What is sound? Sound is a signal - a value that changes over the course of time. In fact it's a bipolar signal, meaning its values can be both positive and negative.
The easiest way to put, it is the strength of pressure, most often air pressure, which our ears then proceed to catch and process it accordingly.

In real world, we deal with two kinds of signals, a periodic signal, which repeats over and over again, and random signal, more commonly referred to as noise.
Most often sound is an intricate combination of these two.

What do we measure in sound? There is a copious number of units we can look at, however there are three fundamental which we will look at.
First off, we measure the immediate sound pressure in decibels (dB).
The second property we will look at is the amplitude, which is the absolute peak value of the signal.
Last but not least we can measure is exclusively in periodic signals frequency, which is how many times the signal repeats over a certain time period. We call this unit one hertz (Hz).

## Oscillators

So how do we make sound? We use oscillators, circuits that produce continuous and repeating wave.
There are 4 well established wave shapes that oscillators commonly generate.

-   Sine - the fundamental building block of sound, every sound can be rebuilt with purely sine waves
-   Saw - sound wave which contains every harmonic overtone, they are usually used to fill the audible frequency spectrum, they are commonly referred to as "full"
-   Square - waveshape whose value is constantly at the amplitude, it's a harmonic series which consist of odd harmonics
-   Triangle - very similar to square, except it has way fewer harmonics

## Hamonic overtones and the fundamental

As mentioned, a saw wave is constructed using a sine wave and its harmonics, so what are they?
First we need a little bit of backtracing, every periodic signal has a frequency at which the values begin to repeat.
We call this the fundamental frequency, and if we have a sine wave playing at this frequency, we call it the fundamental.
So what happens if we were to add a sine wave at a frequency multiplied by an integer greater than one?
(we will call this integer n)

Firstly, we can notice that it will fit n times into each iteration of the original signal,
additionally, the combined sound doesn't feel as two playing simultaneously, it feels much more cohesive.

So now back to saw wave - if we have a fundamental frequency at 100Hz, then a saw wave would be the infinite sum of harmonics at fractional amplitudes.

Optimization note: Technically, a sound can have infinitely many harmonics, but for performance sake, we usually render around 500 when we render them individually
