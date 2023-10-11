# Lama Quartet for FL Studio 21 Patcher
## Overview
Lama Quartet is a Patcher preset designed to replicate the dissonant, wide vibrato of the choir in Kenji Kawai's legendary "Making of a Cyborg" from the Ghost in the Shell OVA with vocal synthesizers. 
## Requirements
Lama Quartet requires FL Studio 21 and the Delay Lama vocal synthesis plugin by AudioNerdz.
## Instructions
To control the notes played by the four Lamas, reference the VFX Color Mapper instance on the map screen. The keyboard is divided (rather crudely) into four sections, each controlling a Lama within a similar octave to the others. Automate the controls on the control surface to control the Lamas' parameters in unison (or staggered unison in the case of the vibrato).
## FAQ
*Why did you make this?*
For my upcoming Ritual Horror-themed Music Pack (Coming soon to itch.io and others) I wanted to recreate the Shinto ritual bell sound from "Making of a Cyborg" (I have no idea what the bell is actually called, but I heard a very similar one during a blessing at a Shinto shrine). Making the bell sound was relatively straightforward; I took a concert sleigh bells sample from a free orchestra VST, added some reverb, and then rolled off the lows and mids until it sounded pretty close. Since I don't have the budget to use an actual choir, I wondered if I might be able to synthesize the choir or at least replicate their technique in some other context. 

*Why are there so many LFO Controllers?*
Aside from the ones used for Lama pitch modulation, the LFO controllers are used to control relatively-static parameters because of a bug in Delay Lama's MIDI implementation in my environment. For me, Delay Lama's parameters will reset to default values after a few minutes of being set at a static value. As a workaround, I use LFO controllers to feed in very subtle changes to these values in the hope that they will not reset unexpectedly. This workaround is usually successful, but double check your values when you load a project or if you haven't adjusted them in a while. With a different vocal synthesizer, the static parameter LFOs would become vestigial.

*What's with the PEQ2 instances?*
I used the EQs in a crude attempt to tame some of the harsh harmonic resonances that can occur when Delay Lamas are played in unison. If you modify this plugin, it would probably make more sense to use some type of compressor instead. Hopefully, your favorite vocal synth won't create any such harsh resonances. 

