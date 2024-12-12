# Note

The name of an event that can be programmed in an instrument clip row in order to generate audio (for example, a synthesized sound or sample) or non-audio (for example, MIDI, CV, Gate) output. Each note has specific parameters that determine when and how a note is to be triggered.

## Settings

Several basic parameters of notes can be changed in settings. These include: quantization.

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

Press (SCROLL▼▲) + Turn (SCROLL◄►) control to adjust the clip note events i.e. notes and automation horizontally across the grid.
    - The note events will move 1 step incrementally across the horizontal grid. The steps are based on the zoom level.
    - Note events which scroll off the edge left or right will wrap back onto the grid from the opposite side.

#### Adjusting the position of all notes in a note row horizontally

Insert instructions

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

## Scales

Scale mode is automatically set when new synth, MIDI and CV clips are created. Scale mode will lock the notes to a specific scale, by default a major scale. Chromatic scale can be selected by exiting ‘scale’ mode. Other scales can be selected.

**Insert picture from manual**


