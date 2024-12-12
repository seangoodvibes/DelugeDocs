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

### Setting the Sequencer Play Direction

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

## Recording Pattern Sequences

The recording of note events can be performed manually using the step sequencer or live recording using the audition pads.

### Step Recording a Basic Synth / MIDI / CV Pattern

1. Press [CLIP] to select clip view. Clip button illuminated blue.

1. Select SYNTH by pressing [SYNTH] if not already selected. The synth button illuminates red. Also applies to MIDI & CV.

1. Select a preset for a synth or channel for MIDI & CV by turning the (SELECT) rotary. Auditioning the synth selections is available with the [AUDITION] pads which plays the scale.

1. Program a pattern on the grid by pressing one or more [PAD] buttons. The arrangement is made across columns for the time line from left to right. The note pitch is dependant on the row selected.

1. To extend the note length hold the first [PAD] + press end [PAD] which will extend the note between the two pads. The first pad is lit with the additional pads of the note dimly lit. Repeat to deselect.

1. The grid by default is in 1/16th Note intervals across 1 bar of the physical horizontal grid. The [PAD] buttons lit will trigger the synth when the sequence is playing. The actual grid environment can be bigger than just the physical 16 x 8 pads and therefore may be out of view.

1. Press [PLAY] to play out the synth sequence and observe the white cursor bar scrolling left to right and cycling across the grid.

1. Patterns can be edited during playback.
   - Press an unlit [PAD] to select it and press a lit [PAD] to deselect it.
   - Press [BACK / UNDO] to undo a note step placement action and [SHIFT] + [BACK / UNDO] to restore, redo the note step action
   - Use the mute / launch column to mute (yellow) or unmute (green) a selected row’s notes from the pattern.
   - Saving synth presets in clip view will only save the synth settings. Patterns are stored with songs not in synth presets.
   - The lit audition / section pad indicates the root note by the lit button or buttons if a full octave is in view.
   - The colours will change dependant upon the pitch by row
  
### Step Recording a Basic Kit Pattern

1. Press [CLIP] to select clip view. This is indicated by the clip button illuminated blue.

1. Selected kit by pressing [KIT] if not already selected. The kit button illuminates red.

1. Select a preset by turning the (SELECT) rotary and auditioning the individual sound selections available with the [AUDITION] Pads.

1. Program a pattern on the grid by pressing one or more [PAD] buttons. The arrangement is made across columns for the time line from left to right. The individual sounds i.e. drum hits are dependant on the rows selected.

1. The grid by default is in 1/16th intervals across 1 bar of the physical horizontal grid. The [PAD] buttons lit will trigger the kit sounds when the sequence is playing. The actual grid can be bigger than just the 16 x 8 pads and therefore may be out of view.

1. Press [PLAY] to play out the kit sequence and observe the white cursor bar scrolling left to right and cycling across the grid.

1. Patterns can be edited during playback.
   - Press an unlit [PAD] to select it and press a lit [PAD] to deselect it from the pattern.
   - Press [BACK / UNDO] to undo a kit step placement action and [SHIFT] + [BACK / UNDO] to restore, redo the kit step action.
   - Use the mute / launch column to mute (yellow) or unmute (green) a selected row’s notes from the pattern.
   - Saving kit presets in clip view will only save the kit settings. Patterns are not stored in kit presets, they are stored with songs.
   - The lit audition / section pad indicates the selected row and hence the selected kit sound.
   - Colours are assigned to the unique kit sound on each row.
  
### Live Recording a Basic Pattern using Audition Pads

1. Press [CLIP] to select clip view. This is indicated by the clip button illuminated blue.

1. Selected SYNTH or KIT by pressing [SYNTH] or [KIT] if not already selected. The synth or kit button illuminates red.

1. Press [RECORD] to put the sequencer into armed record mode ready for play. Record button is lit red.

1. Press [PLAY] to start the sequencer playing. Play is lit green.
   - Fixed length mode. If notes exist in the clip a white cursor will play. The notes are recorded for the length set, eg: 1 bar.
   - Auto extend mode: If the clip is fully empty, no notes or sounds on the grid, the cursor will play red. Notes will be recorded as the sequencer records with an ‘unlimited’ length.

1. Play the notes, chords, melody in real time using the eight [AUDITION] pads. The pattern will be recorded as played including a predefined velocity, timing, length and note. Notes are displayed for each of the audition pads when played.

1. Press [PLAY] to stop playing the sequencer. Press [RECORD] to deselect record mode.

1. Overdubs can be created by repeating step 3 - 6.

1. Patterns can be edited during playback.
   - Default quantization for recording live is 32nd notes. Quantization sets how accurately the notes are placed onto the grid
   - Press an unlit [PAD] to select it and press a lit [PAD] to deselect it.
   - Press [BACK / UNDO] to undo phases of the recording and [SHIFT] + [BACK / UNDO] to restore, redo the recording.
   - Use the mute / launch column to mute (yellow) or unmute (green) a selected row’s notes from the pattern.
   - The lit audition / section pad indicates the root note by the lit button or buttons if a full octave is in view for synths. Lit pad for kits indicates a selected row.
   - The colours will change dependant upon the pitch by row.

### Live Recording a Basic Synth Pattern using Keyboard

1. Press [CLIP] to select clip view. This is indicated by the clip button illuminated blue.

1. Select SYNTH by pressing [SYNTH] if not already selected. The synth button illuminates red. Keyboard view is not available for kits.

1. Press [KEYBOARD] to select keyboard view. Pads illuminate to represent keyboard scale to be played. Semitones horizontally and rows represent 4th intervals per row. This is similar to a guitar fret-board.

1. Press [RECORD] to ‘arm’ the sequencer in record mode ready for a play request. Record button is lit red.

1. Press [PLAY] to start the sequencer playing. Play is lit green and the red grid cursor steps through the sequence on the top row.
   - Fixed length mode. If notes exist in the clip a white cursor will play. The notes are recorded for the length set, example 1 bar.
   - Auto extend mode: If the clip is fully empty, no notes or sounds on the grid, the cursor will play red. Notes will be recorded as the sequencer records with an ‘unlimited’ length.

1. Play the grid keyboard [PAD] lit notes, chords, melody in real time. The pattern will be recorded as played including predefined velocity, timing, length and note. Notes are displayed for each of the keyboard pads when played.

1. Press [PLAY] to stop playing the sequencer. Press [RECORD] to deselect record mode.

1. Overdubs can be created by repeating step 4 - 7

1. Patterns can be edited during playback.
   - Default quantization for recording live is 32nd notes. Quantization sets how accurately the notes are placed onto the grid- Scale for the keyboard can be changed.
   - Press [BACK / UNDO] to undo phases of the recording and [SHIFT] + [BACK / UNDO] to restore, redo the recording.
   - The lit [PAD] indicates the root note by the brightest button.

### Setting a Recording Count-In

1. Press [SHIFT] + press (SELECT) to access the settings menu.

1. Turn (SELECT) to highlight RECORDING

1. Press (SELECT)

1. Turn (SELECT) to highlight COUNT-IN

1. Press (SELECT) to set the count-in option.

1. Turn (SELECT) to choose OFF or ON. This will set the count-in for recording on or off.

1. Count in will operate when set ON.
   - With Deluge as leader, [RECORD] enabled, press [PLAY] to perform a count-in prior to recording.
   - Metronome and display counts down 4-3-2-1 prior to recording.
   - Count-in is disabled if recording is going to begin for just one audio clip from which it’s going to auto-detect the tempo.

## User Interface - Main Grid Pads

Deluge has a 16 x 8 grid of pads which is used when sequencing notes and creating melodies and patterns. The actual programming grid is not limited to the 16 x 8 pads in focus and on view.

### Navigation

#### Scrolling

Higher and lower notes (synth) or different samples (kit) can be scrolled up and down or longer time sequences left / right are available. The focus area can be scrolled and zoomed across the pattern real estate to suit your workflow and area of interest.

**insert picture from manual**

##### Horizontal Scrolling

1. Press [CLIP] to select clip view. This is indicated by the clip button illuminated blue.

1. Select SYNTH or KIT by pressing [SYNTH] or [KIT]. The selected button illuminates red.

1. Turn (SCROLL◄►) to scroll the grid in focus. If there are no notes / steps existing beyond the visible pad grid then no scrolling will take place. Scrolling will move by the full page of 16 steps.

1. Editing of notes and steps is retained irrespective of whether the notes are in focus and viewed within the pad grid. Horizontal scrolling adjust the step columns in focus based on the time division

##### Vertical Scrolling

1. Press [CLIP] to select clip view. This is indicated by the clip button illuminated blue.

1. Select SYNTH or KIT by pressing [SYNTH] or [KIT]. The selected button illuminates red.

1. Turn (SCROLL▼▲) to scroll the grid in focus. Scrolling will take place. Scrolling will move by one row at a time and for synth notes the audition pads will show the root note position for synths and the selected row for kits.

1. Editing of notes and steps is retained irrespective of whether the notes are in focus and viewed within the pad grid. Vertical scrolling adjusts the step rows in focus based on the note pitch for synths or specific sounds for kits.

#### Zooming

Zooming the grid also uses the scroll and zoom rotary control. Zooming is performed across the horizontal timeline of the grid. The grid resolution will change to the zoom level selected and as such may include more or less visible information. Zooming-in is possible from the 16th default to 128th notes.

**insert picture from manual**

##### Horizontal Zooming

1. Press [CLIP] to select clip view. This is indicated by the clip button illuminated blue. 

1. Select SYNTH or KIT by pressing [SYNTH] or [KIT]. The selected button illuminates red.

1. Press + turn (SCROLL◄►) to zoom the grid showing more or less detail. Step resolution will expand up to 128th notes and shrink depending on the zoom level. Default is 16th notes.

1. The bar, beat of the current bar and (if visible) the 16th note in the current beat flashes for a short period on the display as adjustments are made.

**insert picture from manual**

##### Checking Zoom level Resolution

1. Press [CLIP] to select clip view. This is indicated by the clip button illuminated blue.

1. Select SYNTH or KIT by pressing [SYNTH] or [KIT]. The selected button illuminates red.

1. Press (SCROLL◄►). The display will flash showing the timing division resolution depending on the clip length. Examples are:-

**insert picture from manual**

### Adjusting Clip Sequence Length

Default clip length is 1 bar. This however can be changed which will extend the sequence beyond the grid in focus. This can be navigated using the scroll and zoom features. Automatic extending of clips will take place if recorded to a blank clip (no notes or sounds).

#### Extend length

1. Press [SHIFT] + turn (SCROLL◄►) control to adjust the clip length. Clockwise to increase length. Anti-clockwise to reduce clip length.
  - The display will show the length in bars : beats : 16th notes.
  - The column pads on the grid will also indicate the clip length by illuminating dim grey for columns outside of the length. The grid columns within the length will be unlit / off.
  - Automatic scrolling will take place if the length is extended further beyond the right side columns. Automatic zooming will take place when clip length is reduced less than half of the grid. 16th note examples:

**insert picture from manual**

#### Duplicating pattern contents - Multiply clip length

1. Press [SHIFT] + press (SCROLL◄►) to duplicate the clip length once and associated pattern.
  - Automatic zooming out will take place when clip length is increased. The grid resolution time division may automatically change for example from 16th to 8th notes.
  - Multiplying again will therefore ‘double’ the 8th note view.
  - Zoom can be restored and scrolling to view across the entire grid if required.
  - Any iteration dependance settings may be automatically changed when duplicating / multiplying

**insert picture from manual**

### Cross Screen Editing

Cross-screen editing enables duplicated patterns across multiple, equivalent zoom level screens to be edited in-sync with the current screen displayed on the 16x8 grid. This means changing one screen, for example, to add an extra kick at the end of a bar, will be applied to all other out-of-view screens.

#### Applying edits across multiple screens

1. Select a pattern and duplicate it to match your needs. Example 1 bar pattern duplicated twice and visible across 4 x ‘screens’, of the 16x8 grid with 16th resolution.

1. Ensure the screen to edit is in focus. Example, first bar of a 4 bar pattern at 16th resolution.
1. Edit the pattern as desired. Example, place extra kick at the end of the pattern, first bar. The edit will only affect the first bar.

1. Press [CROSS-SCREEN] to switch the mode on. Button lit.

1. Edit the pattern as desired. Example, place extra kick at the end of the pattern, first bar. The edit will be changed in the first bar in view and also bar 2,3 and 4 off screen.

1. Edits in cross-screen mode are dependant on, and locked to the zoom level. Example, if 8th note resolution displays 2 bars in view and changes are made in cross-screen mode at the end of bar 2, this will also change at the end of bar 4, the screen out of view.

Note: Clips individually remember whether, and at what zoom level, they have cross-screen edit mode applied. Entering the mode for one track will not automatically be active for any other track that is then edited.

**insert picture from manual**
