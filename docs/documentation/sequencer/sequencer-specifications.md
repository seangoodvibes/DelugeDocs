# Sequencer Specifications

- I previously thought sequencing was just for Instrument Clip types but now I'm changing my tune.
- The sequencer in the Deluge produces an output by "processing the current playhead position" - for audio clips that means rendering the audio sample it contains and then processing that through the global clip modulation settings at that same position (e.g. sample + filter).
- For instrument clips, for the sequencer to generate sound, you must first place note (event) triggers across the timeline. The triggers create sound. Where modulation happens in the sound generation path varies depending on the type of modulation (e.g. it could at a voice level, or applied globally after). But modulation is also sequenced because it takes the modulation values at the same position as the note trigger.
- For kit clips we go even further by having sound generated at the kit row level and then additional modulation at the clip level (affect entire parameters).
- All this to say, while an audio clip is not traditionally what we think of as a sequencer, technically it is still sequencer with the audio sample having a single trigger at the start of the clip.
