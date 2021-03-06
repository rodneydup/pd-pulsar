# pulsar~

An implementation of Pulsar Synthesis<sup>1</sup> in Pure Data.

Abstracting pulsar synthesis into an object in pure data expands the possibilities for controlling and experimenting with single or multiple simultaneous pulsar generators. It can be integrated into a complex Pure Data patch with potentially several pulsar~ objects. See the help patch for examples.

![](Pulsar~.png "This is what it looks like")

## Features:

- A GUI on the object itself as well as the ability to control various parameters through the control inlets.<sup>2</sup>
- 5 basic waveforms included for the <i>pulsaret</i> in addition to the ability to import any arbitrary .wav file as the pulsaret.
- 4 common envelopes with a "Slope" variable that adjusts the width of the Gauss envelope and the exponential curve of the Expodec.
- Draw a custom envelope shape or custom pulsaret shape on screen.
- Visual displays of the shapes of the pulsaret, envelope, and overall pulsar.
- "Sync" input that accepts a bang and resets the phase of the pulsar, allowing the ability to synchronize multiple pulsar objects.
- "Mask" input that accepts a list of numbers between 0 and 1, playing pulsars with those amplitude values sequentially.<sup>3</sup>

## Installation
No installation required, but you must have [Pure Data](https://puredata.info/) installed. 
<br><br>
[Download](https://github.com/rodneydup/pd-pulsar/archive/master.zip) this repository and put "pulsar~.pd" and "pulsar~-help.pd" in a folder where Pure Data looks for its objects. Help on this can be found here: https://puredata.info/docs/faq/how-do-i-install-externals-and-help-files

Once the pulsar~ files are in the right directory, you will be able to create a pulsar~ object in any Pure Data patch by creating an object and typing pulsar~ in it. 


<br><br><br>

<sub>
[1]: Pulsar Synthesis described by Curtis Roads (2000) here: https://archive.org/details/soundcompwithpulsars/page/n1/mode/2up
<br><br>
[2]:Having a complex interface on the object itself is not very "Pure Data" in philosophy, but the goal was to make the object very user friendly even to beginners in Pure Data. There are not very many implementations of Pulsar Synthesis on the market at the moment of writing this and my hope is that this object can be an easy way for anyone to experiment with its potential.
<br><br>
[3]: This effectively turns the pulsar generator into an audio rate sequencer.
</sub>
