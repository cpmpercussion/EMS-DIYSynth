---
title: DIY Synthesiser Workshop 
author: Charles Martin
...

This workshop is a crash-course in creating sound-making electronics!
We're going to use some inexpensive parts to make some insane, noisy
synthesisers and think about some ways to use them in performances.

The key parts we're using are two integrated circuits (ICs) which are
(big versions of) some of the building blocks of computers. In digital
electronics, signals are either on ("high" or connected to positive
voltage) or off ("low" or connected to ground or 0 volts). One IC
contains inverters or NOT-gates that output the opposite of their
input (so high becomes low). The other contains NAND-gates which have
two inputs and are only high if both inputs are low. Both of these
elements can be easily used to make circuits that oscillate (go from
high to low and back) at audio frequencies. Connect the oscillating
signal to a speaker and BAM you've got a synthesiser.

The cool part is that with one chip we can make not one but SIX
inverter synth voices and the other can make four voices of NAND
oscillators. By mixing the voices together or using them to control
each other we can make some very interesting sonic results.

Each kit contains a project box, battery and some parts. We'll do a
few experiments together to figure out the possibilities of these
parts but at the end of the workshop, you'll have a hackable
synthesiser built into the project box ready for your next
experimental music session.

## Parts in your DIY Synth Kit

- breadboard
- 9V battery
- 9V battery lead
- strip of header pins
- 40106 - hex inverter IC (one little chip)
- CD4093 - quad nand gate IC (other little chip)
- Potentiometers: 10KOhm, 100KOhm, 1MOhm (knobs)
- Light Dependent Resistors (LDR)
- Enclosure box

### Other Parts available to take

- bunch of resistors (esp. 1K, 10K, 100K)
- bunch of diodes
- extra LDRs 
- extra potentiometers
- jumper leads
- alligator clips
- breadboard wire (thin solid core wire for making breadboard
  connections)

### Tools available

- soldering irons
- pliers
- wire cutters
- mini speakers

## Parts we need

### Battery

We're all familiar with batteries - they store electrical power and
when you connect the + terminal to the - terminal electrical current
will flow between the two terminals until the power in the battery is
consumed. 9V batteries are convenient because they're small and have a
lot of volts (useful for powering complicated circuits) - but they
don't have a high capacity so they can't supply a high current for a
long time.

(In contrast, AA batteries have much higher capacities, but can only
supply 1.5V each, so devices typically use more than one.)

### Resistors

Resistors slow down the flow of electrical current. If you connect
the + and - terminals of a 9V battery you might find that the wire
will quickly get too hot to touch - too much current is flowing, which
causes the metal to heat up, and the battery to run down quickly.

Resistors are used for slowing down electrical current in circuits.
Some reasons to do this are: so that other components aren't damaged
by excessive current, so we don't run down batteries too quickly!

Two resistors can also form a simple circuit called a voltage divider
that converts from a high to lower voltage. And we can also use
resistors to create a simple mixer! They're all around good guys.

Resistance is measured in Ohms and you can find out the value of a
resistor by decoding the coloured bands or by measuring it with a
multimeter. 1Ohm is a very small amount of resistance, so we usually
use resistors with values between a few hundred and a few hundred
thousand Ohms. For making our synthesisers it usually doesn't matter
_exactly_ what value the resistors are, so I've got a huge number of
1kOhm, 10kOhm and 100kOhm resistors to use!

### Capacitors

Capacitors are like little rechargeable batteries. They've got lots of
uses in electronics, but they're a key component in the synthesisers
we're going to make. Capacitors are measured by how much charge they
can contain, a value in Farads. 1F is a huge amount, so we usually see
caps that contain between 0.1uF and 220uF that is millionths of a
Farad!

Higher valued capacitors have a + and - terminal and need to go in the
right way. These ones are usually little tubes and have a big arrow on
the side with minus signs. Little caps sometimes look like little
yellow discs or blobs and it doesn't matter which way you put them in.
The tube caps usually have a marked value, while the little ones use a
code. "104" is a common type, which means 0.1uF.

### Potentiometers, LDRs

Potentiometers and LDRs (Light Dependent Resistor) are both resistors
that change their value. Potentiometers change when you turn the knob
and LDRs change when they are exposed to more or less light.

LDRs are easy to deal with because they have two leads - just like a
regular resistor. Potentiometers can be confusing because they have
three leads. Inside the potentiometer there's a long windy trace of
resistive material connected to each of the outer leads, and the inner
lead is connected to a bit of metal that brushes over this trace as
you turn the potentiometer. So as you turn, the connection between one
of the outer and the middle leads increase resistance, while the other
decreases.

### Integrated Circuits

Little black caterpillers with 14 legs. These guys will do the work in
our synthesisers! These devices are electronic swiches with inputs and
outputs. On the "inverter" if the input is on, the output is off and
vice versa. On the NAND gate, there are two inputs and one output, the
output is only on if both inputs are off. Both of the chips actually
contains several of these switches, there are six inverters and four
NAND gates on each.

ICs always need to be powered before they can be used. On both of
these pin 1 (marked with a dot) is connected to +ve and pin 14
(diagonally opposite) is connected to -ve.

## Project 0 - set up the breadboard

The breadboard has lots of little holes to plug in components. They're
connected in a fairly simple pattern (see below). The long connections
at the top and bottom are designed for the + and - connections of the
battery (you would normally connect these to several places in a
circuit). The slot in the middle is for ICs to sit.

As a first step, lets connect the battery snap to one side of the
breadboard and then use some jumper wires to connect the power rails
on both sides togther.

## Project 1 - making one inverter-oscillator

Let's get started by making one sound. We'll use the 40106
hex-inverter. Put it in the middle of the breadboard and use a jumper
to connect pin 1 to the + rail and pin 14 to the - rail.

Grab a resistor and a capacitor and connect like so:

Now, get some alligator clips and connect them to a speaker, and we
can probe around to find the sound. Connect the ground to ground and
the speaker input to the leg of the IC connected to the resistor.
Loud!

This little circuit relies on how long it takes to charge the
capacitor for the frequency of the sound. Larger valued caps will
charge more slowly (lower sound), and smaller valued resistors will allow more
current through, charging them more quickly (higher sound). Try out
some different capacitors and resistors!


## Project 2 - controlling the volume

## Project 3 - controlling the pitch

## Project 4 - mixing synths together

## Project 5 - a NAND synth

## Project 6 - oscillators that control oscillators

## Project 7 - getting it all into a project box

