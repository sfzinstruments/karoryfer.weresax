Weresax is a sample library for Plogue Sforzando version 1.845 or newer. It contains samples of an alto saxophone.

To register, drag the Weresax.bank.xml file onto the Sforzando interface. Once registered, Weresax will be available in the Sforzando loading menu and the GUI will work.

Weresax contains three instruments based on the same samples but with different mappings and controls: sax, saxcordion (fake accordion using saxophone sounds), and sxnth (polyphonic subtractive synthesizer). The provided presets are labeled "New Moon" for sax presets, "Half Moon" for saxcordion, and "Full Moon" for sxnth.

The vibrato of the sax instrument is fairly complex, with nine controls. You can get decent results by just using the sax style vibrato and speed and leaving the rest of the controls alone.

The sax style vibrato only goes below the main pitch of the note, so when it kicks in it will make the note go slightly flat, which makes it sound "bluesy". The violin style vibrato goes both below and above the main pitch, and is better at staying in tune with synths, classical orchestras etc. There's no reason to not use both at once - leaving the synth vibrato at a fairly low setting and automating the sax vibrato and speed for expression seems to work pretty well.

The tremolo, brightness and wind noise controls don't affect the pitch, but instead affect the volume and tone color. If you only use them and keep the sax style and violin style controls at zero, you can emulate what sax players call diaphragm vibrato (which is in theory not really vibrato at all, as the pitch never changes). Or use them all together. The wind noise vibrato control has no effect if the wind noise volume control is turned all the way down.

The humanize controls make the pitch and vibrato speed unsteady. At the minimum change rate, the values will be randomized once per note (unless you hold a note for many seconds). At high change rates, they will be randomized many times per second.

Finally, two warnings about the controls:

The vibrato humanization affects each voice independently, so if you have the mic blend set to some intermediate position and are humanizing the pitch and/or vibrato rate, it can end up sounding like two separate saxes, or a sax with a weird chorus.

The resonance in the sxnth instrument have huge resonant peaks at high settings, so if turning them up, we recommend turning down the volume in Sforzando, or using a limiter to avoid clipping.

MIDI CC control assignments for the sax:

7: master volume
10: master pan
100: volume envelope attack
101: volume envelope hold
102: volume envelope decay
103: volume envelope sustain
104: volume envelope release
110: degree to which breath noise is affected by vibrato
111: sax-style vibrato depth (goes only below the main pitch)
112: vibrato speed
113: tremolo (degree to which volume is affected by vibrato)
114: violin-style vibrato depth (goes both below and above the main pitch)
115: degree to which mid-boost is affected by vibrato
116: delay of vibrato onset
117: vibrato humanization rate (how often the next two parameters are randomly changed)
118: pitch humanization
119: vibrato rate humanization
120: mic blend between clean condenser and overdriven dynamic
121: turning this up will cut midrange frequencies at low velocities and boost them at high velocities
122: breath noise volume

MIDI CC control assignments for the saxcordion:

1: power (combination of volume and filter cutoff)
7: master volume
10: master pan
100: volume envelope attack
104: volume envelope release
106: amount od detune between the voices
107: stereo width of the voices
112: tremolo speed
113: tremolo depth
114: vibrato speed
115: vibrato depth
120: brightness (amount by which CC1 affects filter cutoff)

MIDI CC control assignments for the sxnth:

7: master volume
10: master pan
100: volume envelope attack
101: volume envelope hold
102: volume envelope decay
103: volume envelope sustain
104: volume envelope release
105: volume of unison voices (first two additional voices, then two more)
106: amount of detune between the voices
107: stereo width of the voices
111: vibrato depth
112: vibrato speed
113: delay of vibrato onset
114: vibrato fade-in time
115: low-pass filter cutoff
116: low-pass filter resonance
119: low-pass filter envelope depth
120: low-pass filter envelope attack time
121: low-pass filter envelope decay time
122: low-pass filter LFO depth
123: low-pass filter LFO speed
124: low-pass filter LFO onset delay time
125: low-pass filter LFO onset fade-in time
126: high-pass filter cutoff
127: high-pass filter resonance

This sample library is royalty-free for all commercial and non-commercial use. It is also open-source, and we especially encourage adaptation, reuse and further improvement of the sax vibrato configuration.
Copyright 2015, 2018 Karoryfer Lecolds.