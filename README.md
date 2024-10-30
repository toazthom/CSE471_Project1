# CSE471_Project1
Title: Accordion Synthesis
Group Members: Thomas Toaz - Solo Project

### Score
The score format used for the score files in this project are nearly identical to those used in the Synthie program of Step5. Here is a simple example score file:
```
<?xml version="1.0" encoding="utf-8"?>
<score bpm="120" beatspermeasure="2">
  <instrument instrument="WavetableInstrument" effect1="NoiseGate">
	  <note measure="1" beat="1" duration="0.5" note="C1"/>
  </instrument>

</score>
```
Score files begin with a declaration of xml information followed by a score tag with attributes determining the beats per minute and beats per measure of the score, then end with an ending score tag at the end of the file. To add instruments to your score simply put a starting and ending instrument tag between the score tags. The instrument starting tag will contain an instrument attribute with the name of the instrument you would like to be playing the notes between it's tag (which can be: WavetableInstrument or ToneInstrument for this project). The instrument tag can also have up to three effect attributes: effect1, effect2, and/or effect3, which can have values of: NoiseGate, RingMod, or Compressor. To declare a note for the instrument to play, put a note tag as shown above within the instrument tag that will be playing the note. The notes follow the exact same structure as those in Step5 with measure, beat, duration, and note attributes.

Here is the [Score](Song.score) used to generate my 1-1.5 minute long piece that shows off all the components I created for this project. The background base is the accordian instrument I made for the Wavetable synthesizer, with not additional effects. The counter tones at the beggining are the accrodian featuring the compressor and noise gate effects, with the melody being the same. There is a measure toward the end that features the accordian with all three effects (compressor, noise gate, and ring modulator) that serves as a source of dissonance (primarily from the ring modulator) to help keep the listener on their toes. 

Please click this link to view descriptions of the [Effects Component](effects.md) and this one for details on the [Synthesis Component](synthesis.md)

