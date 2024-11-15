# Deluge style guide

This Deluge-specific style guide defines how to refer to project parts, modes, views, controls, and display elements.

## Parts of a project

In casual conversation, we often use terms "song", "track", or "project" interchangeably. To make the documentation consistent and predictable, only use the terms as described below.

Song
: A discrete creative endeavour, such as an arrangement, sketch, 8-bar loop, jam, live recording template, or musical experiment. A song is always associated with at least one project files on the Deluge. Note: Don't use the word "project" or "track" for this meaning.

Project file
: A file on the SD card that stores all of the information about a project. Use this only when referring to specific technical concepts to do with the file system or stored data.

Track
: A single instrument or layer in a project. Each track is either an audio track or an instrument track. An instrument track is either a kit instrument track or a melodic instrument track (synth, MIDI, CV). Tracks contain one or more clips.

!!! example "Examples"
    - To save a song, press **Shift** and **Save**.
    - To change the song tempo, turn **Tempo**.
    - To change the volume for a track, press **Volume/Pan** and turn **Upper**.
    - Project files are stored on the SD card in `.xml` format.

## Modes

### Arranger Mode
The mode where songs are arranged chronologically from left to right.

### Session Mode
The mode where clips are organized in one of the two Session View layouts:

- Session Mode Rows Layout
- Session Mode Grid Layout

### Style

- Capitalize mode names
- These terms are long, so only use the part that's necessary for clarity:

!!! example "Examples"
    - Add a track by doing one of the following:
        - In Arranger Mode and Session Mode Rows Layout, press a pad in an empty row.
        - In Session Mode Grid Layout, press a pad in an empty column.
    - In Session Mode, clips are grouped into sections, and each section has a unique colour.
    - To change from Rows Layout to Grid Layout, hold **Song** and turn **Select**.

## Views

### Names

- Audio Clip View
- Melodic Instrument Clip View
- Kit Instrument Clip View
- Keyboard View
- Automation View
- Performance View

### Style

- Capitalize view names
- Don't use bold unless referring to the text that appears on the display

## Keyboard layouts

#### Names

- isomorphic
- in-key
- chord
- chord library
- drum velocity

### Style

- Don't capitalize keyboard layout names
- Don't use bold unless referring to the text that appears on the display
- Follow with "keyboard" or "layout" depending on the context

!!! example
    - Enter the sequence, then go back to the chord keyboard.
    - To change to the isomorphic keyboard layout, press **Shift** and turn **Select**.

## Display elements and menus

- When referring to elements on the OLED display or locations of elements in menus, use **bold** and Title Case.
- When referring to elements on the 7SEG display, use `code` and match the capitalization on the display.

!!! example "Examples"
    - Open Settings and go to **Defaults** > **Automation**, and enable **Nudge Note**.
    - Open Settings and go to `dEFA` > `AUTo`, and enable `nUdG`.

## Buttons and controls

- Use **bold** and Title Case for physical buttons and knobs.

### Buttons and pads

#### Names

- **Level/Pan**
- **Cutoff/Res**
- **Attack/Release**
- **Delay Time/Amount**
- **Sidechain/Reverb**
- **Mod Rate/Depth**
- **Stutter/Custom 1**
- **Custom 2/Custom 3**
- **Affect Entire**
- **Song**
- **Clip**
- **Synth**
- **Kit**
- **MIDI**
- **CV**
- **Keyboard**
- **Scale**
- **Cross Screen**
- **Back/Undo**
- **Load**
- **Save**
- **Learn/Input**
- **Tap Tempo**
- **Sync-Scaling**
- **Triplets View**
- **Play**
- **Record**
- **Shift**

#### Style

- Use "pad" for any of the square buttons in the 8x16 or 8x2 grid.
- Use "sidebar" for the group of 8x2 pads on the right side of the device.
- Use the following for pad and button action timings:
    - Use "tap" for fast (<1 second) actions
    - Use "press" for regular actions
    - Use "hold" for long actions

!!! example "Examples"
    - Tap **Shift** to turn on Sticky Shift.
    - Press **Shift** and **Kit** to create a new drum kit.
    - From Edit Mode, hold the green pad to temporarily enter Launch Mode and tap a clip to launch it. Release the green pad to go back to Edit Mode.

### Knobs

#### Names

- **Upper**
- **Lower**
- **Select**
- **◀ ▶**
- **▼▲**
- **Tempo**
- **Output Level**

#### Style

- Use "turn" and "press" for knob actions.
- When direction matters for a turn, use "clockwise" and "counter-clockwise".

### Control combinations

- Use "and" for simultaneous actions.
- Use "then" for actions that happen in series.

!!! example "Examples"
    - To create a new kit, press **Shift** and **Kit**.
    
    - To clear automations for the clip, press **Lower** and **Back/Undo**.

    - To zoom out, press and turn **◀ ▶** counter-clockwise.

    - To change to the isomorphic keyboard layout, press **Shift** and turn **Select**.

    - To map MIDI channel 1 to the Synth Clip, press **Learn** and **AuditionPad** and play a MIDI note on channel 1.

    - To load a preset, press **Load** and **Synth**. Turn **Select** to change the preset, then press **Select** to load it.

## Parameters

## Modulation mappings

`Source1 -> Destination`  
`Source2 -> (Source1 -> Destination)`

Use `->` to refer to a source to destination modulation depth, or to refer to the source to destination mapping itself. Use abbreviated versions of the source and destination names. When referring to modulating the modulation depth of an existing source to destination mapping, use parenthesis around the existing mapping.

!!! example "Examples"
    - Increase `LFO2 -> OSC1 Transpose` from 10 to 20 to modulate OSC1 frequency across a wider range. 
    - Play a note while turning up the modulation depth for `LFO2 -> OSC1 Transpose`. 
    - Adjust the `ENV2 -> (LFO2 -> OSC1 Transpose)` modulation depth to have `ENV2` control how much `LFO2` affects `OSC1 Transpose`. 
    - `MIDI CC2 -> OSC1 Transpose` refers to `MIDI CC2` controlling `OSC1 Transpose`. 
