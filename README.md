# CSE471_Project1
Title: Accordian Synthesis
Group Members: Thomas Toaz

### Score
The score format used for the socre files in this project are nearly identical to those used in the Sunthie program of Step5. Here is a simple example score file:
```
<?xml version="1.0" encoding="utf-8"?>
<score bpm="120" beatspermeasure="2">
  <instrument instrument="WavetableInstrument" effect1="NoiseGate">
	  <note measure="1" beat="1" duration="0.5" note="C1"/>
  </instrument>

</score>
```
Score files begin with a declaration of xml information followed by a score tag with attributes determining the beats per minute and beats per measure of the score, then end with an ending score tag at the end of the file. To add instruments to your score simply put a starting and ending instrument tag between the score tags. The instrument starting tag will contain an instrument attribute with the name of the instrument you would like to be playing the notes between it's tag (which can be: WavetableInstrument or ToneInstrument for this project). The instrument tag can also have up to three effect attributes: effect1, effect2, and/or effect3, which can have values of: NoiseGate, RingMod, or Compressor.


