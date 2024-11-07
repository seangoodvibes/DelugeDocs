# Deluge style guide

This Deluge-specific style guide defined how to refer to song parts, views, controls, and display elements.

## Parts of a project

Project
: A discrete creative endeavour, generally aligned with one (but sometimes several) project files on the Deluge. Note: Avoid using the word "song" unless referring specifically to Song Mode. "Project" is a broader term that captures sketches, 8-bar loops, jams, live recording templates, experiments, and more in addition to the idea of a "song" with a beginning, middle, and end.

Project file
: A file on the SD card that stores all of the information about a song. Use this only when referring to specific technical concepts to do with the file system or stored data. For general usage, use "song", such as saving or deleting a song.

Track
: A single instrument or layer in a song. Each track is one of the following types: synth, kit, MIDI, CV, or audio. Tracks contain one or more clips. NOTE: Don't use "track" to mean song or project, such as "track tempo". Use "song tempo".

Clip
: A stored sequence of notes or parameter automation associated with a track. Each track can have multiple clips.

Parameter
: The name of an adjustable value, such as LPF Frequency, Reverb Room Size, or OSC1 Level, that can be manipulated and saved as part of a song. Some parameters can be modulated and automated. Format the name of the parameter like `LPF Frequency` and use the abbreviated name. Refer to the Parameter Abbreviations Table. 

## Modes

Modes provide different ways of working with tracks and clips. They are mutually exclusive, meaning only one mode can be used at a given time. 

Arranger Mode
: Allows you to arrange a song chronologically from beginning to end. Each track is represented by a single row on a timeline. The clips for a given track are placed in sequence from left to right.

Song Mode
: Allows you to work with tracks and clips using two main views. Rows View and Grid View.

## Views

#### Names

- Rows View
- Grid View
- Keyboard View
- Performance View
- Automation View
- Velocity View

### Style

- Capitalize view names
- Don't use bold unless referring to the text that appears on the display

## Keyboard layouts

#### Names

- isomorphic
- in-key
- chord
- chord library
- kit velocity

### Style

- Don't capitalize keyboard layout names
- Don't use bold unless referring to the text that appears on the display
- Follow with "keyboard" or "layout" depending on the context

!!! example
    - Enter the sequence, then go back to the chord keyboard.
    - To change to the isomorphic keyboard layout, press **Shift** and turn **Select**.

## Display elements and Menus

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
