# Note

The name of an event that can be programmed in an instrument clip row in order to generate audio (for example, a synthesized sound or sample) or non-audio (for example, MIDI, CV, Gate) output. Each note has specific parameters that determine when and how a note is to be triggered.

## Settings

Several basic parameters of notes can be changed in settings. These include: quantization, scales.

### Scales

Scale mode is automatically set when new synth, MIDI and CV clips are created. Scale mode will lock the notes to a specific scale, by default a major scale. Chromatic scale can be selected by exiting ‘scale’ mode. Other scales can be selected.

Note: All songs with multiple clips set to SCALE mode will always be locked to the same scale. Changes in scale settings on one clip will affect all others in scale mode. This also includes Deluge analysis and evaluation of scale algorithm when entering scale mode, where all clip notes will be evaluated. This may lead to notes being added / changes in the clips when editing scales.

**Insert picture from manual**

#### Selecting scale mode

1. Press [SCALE] to switch scale mode ON. Button lit blue.

1. Press [SCALE] a second time to switch it OFF. Button unlit.

#### Deluge analysis and selection of note scale

1. With notes programmed into the sequence grid.

1. Press [SCALE] to switch it ON. Button illuminates blue. Cycle it off and on if already selected to ON.

1. Deluge will evaluate the notes and establish a ‘best fit’ scale for the selected notes as well as the scale root note.

1. The selected scale will be displayed flashing for a few seconds when selecting [SCALE].

#### Manually setting a root note

1. With notes programmed into the sequence grid and keyboard mode off.

1. Press [SCALE] + [AUDITION] pad for the desired root note. The audition pads can be played to display the notes assigned to each pad.

1. If [KEYBOARD] mode is on, lit blue, Hold [SCALE] + turn (SELECT)

#### Manually changing scale

1. Press [SHIFT] + [SCALE] to cycle through the seven available scales.

1. The grid pattern will change with notes moving to the correct note row for the selected scale.

1. If [KEYBOARD] mode is on, lit blue, Hold [SCALE] + press (SELECT)

#### Creating a custom scale

1. Exit scale mode by pressing [SCALE]. Button should be unlit.

1. Select the notes on the grid that will be attributed to the new scale.

1. Press [SCALE], Deluge will evaluate the notes and establish a best fit scale. Button will illuminate blue.

1. If notes selected form an existing scale this will be recognised. If the notes don't form one of the seven Deluge scales a custom scale identified on the display as OTHER SCALE will be created.

1. Other scales for the notes would indicate CUSTOM SCALE WITH MORE THAN 7 NOTES IN USE on the display if attempted to be selected when the notes don't fit.

#### Manual sharpening / flattening notes in custom scales

1. Ensure [SCALE] mode is on.

1. For the selected note / row, press & hold [AUDITION] pad + press & turn (SELECT) to sharpen or flatten the note.
    - Note will play when pressed. To adjust silently, use [SHIFT] with the [AUDITION] pad.
    - [SCALE] will flash quickly if changes attempted are not available. For example making a sharp the same as the next note / row.

#### Transposing a clip up or down

1. Press & turn [SCROLL▼▲] to transpose the whole octave. 

1. Press [SHIFT] + press & turn [SCROLL▼▲] to transpose by semitone increments.

1. ALL clips that are in SCALE mode will be transposed by the same semitone increment when adjusting the transposition

### Changing the default recording quantization

Quantization sets the accuracy and resolution of how close to the grid intervals notes are placed.

1. Open the settings menu by pressing [SHIFT] + press (SELECT).

1. Turn the (SELECT) control to navigate the menu to select RECORDING

1. Press (SELECT) to drill down the recording menu.

1. Turn the (SELECT) control to navigate the menu and select QUANTIZATION in focus.

1. Press (SELECT) to drill to the quantization settings.

1. Turn (SELECT) to choose between off (384th), 4 bar, 2 bar, 1 bar, 2nd, 4th, 8th, 16th, 32nd and 64th note intervals. A value of 32nd is the default setting.

    - quantization goes even smaller 64th, 128, 256, 512, 1024, 2048, 4096, 8192, and further but just says Tiny on the menu screen at very small values

1. Press [BACK / UNDO] to back out of the menu when the parameter has been changed or at any time in the menu to back up.

1. The quantization chosen will ensure tight alignment on the grid based on the time interval chosen when recording live.

## Parameters

Several basic parameters of notes can be changed. Some can be changed in settings, others can be changed in the sequencer. Parameters include: position (quantization), length, velocity, probability, iterance, fill, repeat, and length.

### Changing a recorded note velocity

1. After a pattern has been recorded, notes will be at a default velocity level.

1. Press & hold one or more [PAD]’s for the note to change and turn (SCROLL◄►).

1. The system default velocity is 64, however the velocity used on the last note entry / edited will be applied to the next note entered.

1. Velocity will be displayed and its value.

**insert picture from manual**

Velocity can also be changed in **Velocity View** and in **Note Editor** (insert links to documentation)

### Setting a note to repeat

1. After a pattern has been recorded, notes will be trigger individually

1. Hold [PAD] + Press & turn (SCROLL▼▲). [PAD] is the note to repeat.

1. The value selected will determine the number of repeats to assign to the selected note, positioned equally in the time interval of the pad.

### Changing the position of recorded note's

#### Nudging individual note horizontally

1. Hold [PAD] + Press and turn (SCROLL◄►) to nudge the selected [PAD] note event forward or backwards, indicated by +/- values.

1. This will nudge at the song’s minimum resolution, default is 384th notes.

#### Adjusting the position of all notes in a clip horizontally

1. Press (SCROLL▼▲) + Turn (SCROLL◄►) control to adjust the clip note events i.e. notes and automation move horizontally across the grid.
    - The note events will move 1 step incrementally across the horizontal grid. The steps are based on the zoom level.
    - Note events which scroll off the edge left or right will wrap back onto the grid from the opposite side.
    - Placeholder: talk about how you can disable moving automation in clip view.

#### Adjusting the position of all notes in a note row horizontally

1. Hold [ÂUDITION PAD] + Press and turn (SCROLL◄►) to adjust the note row events i.e. notes in a specific row move horizontally across the grid.

#### Quantizing / Humanizing Instrument Clip Rows

This is a destructive process and the option is set ON by default in the Settings > Community Features.

1. Select [CLIP] view, button lit blue.

1. Hold the [AUDITION] + Turn (TEMPO) clockwise to quantize the selected row or counter clockwise to humanize the selected row.

1. Hold any [AUDITION] Pad + Press & Turn (TEMPO) clockwise to quantize the all rows or counter clockwise to humanize all rows.

### Changing the length of recorded note's

1. Note lengths can be set when entering clip notes by pressing the note START [PAD] + END [PAD] on the same row. For kits, samples will automatically map across the pads matching the sample length.

**Insert picture from manual**

1. Reduce the note length by pressing one of the extension [PAD]’s to shorten it.

1. To extend a note across grid views:
    - Press the [PAD] for the note start.
    - Scroll to the next grid view ‘page’ using (SCROLL◄►). This would be further in time from the original note.
    - On the same row, press (SCROLL◄►) + [PAD] at the end position.
    - The note will be extended across the ‘page’.

1. To create a note for the duration of the clip, for example as a pad or to create a ‘drone’ note:
    - Press the [PAD] for the note start on the first column (left position) of the clip.
    - On the same row, press (SCROLL◄►) + [PAD] at the last column (right position).
    - The note will be extended across the full clip.
    - Deluge will ensure that these type of notes play continuously through the clip and will loop. This is handled as a special case and the note does not restart.

## Copy / Pasting Notes

1. Press [LEARN / INPUT] + press (SCROLL◄►) to copy the clips notes.
    - This will copy the step range of notes in the current view on the grid at the current scroll and zoom position.
    - The time range of notes is what is copied including all notes out of view above and below the pad range.
    - Copy can be performed from one clip to another in the same or different songs as well as within the same clip.

1. Select the new location for pasting the previously copied range. For example extend the clip length or scroll to another part of the clip.

1. Press [SHIFT] + [LEARN / INPUT] + press (SCROLL◄►) to paste the current clips notes:
    - When pasting, the notes are pasted into the current view.
    - If the destination view is transposed from the original copied location the notes are pasted into the new transposed position.
    - If only a part of the grid is selected as the destination, the notes for the available columns are pasted and the rest discarded.
    - Notes will be pasted into any new zoom levels where notes

## Removing Notes

#### Remove individual note

#### Remove all notes

1. Press (SCROLL◄►) + [BACK / UNDO].

1. Display shows ‘CLIP CLEARED’. Notes and their associated automation will be cleared from the clip, including notes out of view.


