# Sequencer Specifications

- I previously thought sequencing was just for Instrument Clip types but now I'm changing my tune.
- The sequencer in the Deluge produces an output by "processing the current playhead position" - for audio clips that means rendering the audio sample it contains and then processing that through the global clip modulation settings at that same position (e.g. sample + filter).
- For instrument clips, for the sequencer to generate sound, you must first place note (event) triggers across the timeline. The triggers create sound. Where modulation happens in the sound generation path varies depending on the type of modulation (e.g. it could at a voice level, or applied globally after). But modulation is also sequenced because it takes the modulation values at the same position as the note trigger.
- For kit clips we go even further by having sound generated at the kit row level and then additional modulation at the clip level (affect entire parameters).
- All this to say, while an audio clip is not traditionally what we think of as a sequencer, technically it is still sequencer with the audio sample having a single trigger at the start of the clip.

An example of high level workflow on setting up a sequence

**- Insert picture from manual**

## Playing a Sequence

Playing the sequence is a simple process using the mode group transport controls. The default direction is forwards, but reverse and ping-pong are also available as selectable options.

1. Press [CLIP] to select clip view. This is indicated by the clip button illuminated blue.

1. Press [PLAY] to start playback. Button is lit green. Press [PLAY] again to stop the sequence. Button is off.

1. Press (SCROLL◄►) + Press [PLAY] to start playback from the beginning of the grid / zoom position that is in focus instead of from the sequence start position.

**- Insert picture from manual**

## Setting the Sequencer Play Direction

1. Press [CLIP] to select clip view. This is indicated by the clip button illuminated blue. For a KIT clip*, select the row, press [AUDITION].
   
1. Press [SHIFT] + [DIRECTION] to open the setup menu options. The button will flash and the display will indicate the current play direction. The default is Forward.
   
1. Turn (SELECT) to choose the desired direction from the three available
options.

    - FORWARD. Will play the sequencer from the start - left to right. This is the normally expected playback behaviour.
    
    - REVERSE. Will play the sequencer in reverse where the start will be the end of the sequence - right to left.
    
    - PING-PONG. Will play the sequencer firstly from the start - left to right, then at the end will reverse back right to left.
    
    - NONE. Only available for KIT rows* when AFFECT ENTIRE is OFF. This sets the current row direction to operate based on the global kit clip direction setting.

1. Once the direction is selected, press [PLAY] to start playback. Button is lit green. Press [PLAY] again to stop the sequence. Button is off.

**- Insert picture from manual**

*Note: Kit rows can be set to have independent direction control settings. Independent direction for rows are set in a KIT and when [AFFECT ENTIRE] is set to OFF. To set the global direction for all rows in a kit clip, set the direction setting while the [AFFECT ENTIRE] option is set to ON. This will therefore apply the direction to all rows.

**- Insert picture from manual**
