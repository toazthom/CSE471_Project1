# Synthesis Component: Wavetable Synthesizer
All of this component was created by Thomas Toaz as a group of one.

I chose to create a Wavetable Synthesizer for my synthesis component for this project. It works by opening up an accordion audio snippet contained within the project files and parcing out each frame into its own vector table of frames.
This is done in the CAccordion class, which acts as the source for the CWavetableInstrument class much as the SineWave class does for the ToneInstrument class form project 5, allowing the WavetableIntrument class to parse xml notes in exacly the same way. 
Just like the ToneInstrument, the WavetableIntrument class also as a m_ar member variable of the class AR from project 5. This member variable is assigned the Accordion class as a source, creating attacks and releases at the starts and ends
of notes just like it did for the sine tone in Step5, meeting the 20 - Envelope generation requirement. The Accordion class uses a sample audio clip of a C2 to fill its table/frames. In it's generate function, it checks the frequency value
of the note it is currently assigned to be generating, and changes the C2 pitch frames to the proper frequency by multiplying the C2 frame by the base frequency (the C2 frequency) / the assigned note frequency. In this way the 
Wavetable Sythesizer changes the pitch of the sample/table sounds, meeting the 30 - Pitch requirement, and generates those pitches through xml parcing and a Generate function exactly like in the ToneInstrument of Step5 on demand of the sequencer, meeting
the 10 - Wave playback on demand from the sequencer requirement, making it so that the 30/50 required by solo projects is met. Here is a [Score](Accordian.score) and downloadable [Audio](Accordion.wav) of the WavetableInstrument being used 
to play the C scale.

[Back To Main Page](README.md)
