# Deluge style guide

This Deluge-specific style guide defined how to refer to song parts, views, controls, and display elements.

## Terminology

### Parts of a song

Song
: A discrete creative project, generally aligned with one (but sometimes several) project files on the Deluge.

Project
: A file on the SD card associated with a song. Use this only when referring to the file system, such as saving or deleting projects.

Output
: A single instrument or layer in a song. Each output is one of the following types: synth, kit, MIDI, CV, or audio. Outputs contain one or more clips. NOTE: Don't use "output" to mean song or project, such as "output tempo". Use "song tempo".

Clip
: A stored sequence of notes or parameter automation associated with a output. Each output can have multiple clips.

Parameter
: The name of an adjustable value, such as LPF Frequency, Reverb Room Size, or OSC1 Level. Some parameters can be modulated and automated. Format the name of the parameter like `LPF Frequency` and use the abbreviated name. Refer to the Parameter Abbreviations Table. 

### Views

- Capitalize view names
- Don't use bold unless referring to the text that appears on the display

For consistency, refer to the views as follows:

- Arranger View
- Song Row View
- Song Grid View
- Keyboard View
- Performance View
- Automation View
- Velocity View
- Chord View
- Chord Library View

### Display elements and Menus

- When referring to elements on the OLED display or locations of elements in menus, use **bold** and Title Case.

    !!! example
        Open Settings and go to **Defaults** > **Automation**, and enable **Nudge Note**.

- When referring to elements on the 7SEG display, use `code` and match the capitalization on the display.

    !!! example
        Open Settings and go to `dEFA` > `AUTo`, and enable `nUdG`.

### Buttons and controls

#### Pads

Pad
: Any of the square buttons in the 8x16 or 8x2 grid.

Sidebar (TBD)
: The group of 8x2 pads on the right side of the device.

#### Knobs

- Use **bold** and Title Case for physical buttons and knobs

For consistency, refer to the controls as follows:

- **Upper**
- **Lower**
- **Select**
- **◀ ▶**
- **▼▲**
- **Back/Undo**
- **Load**
- **Save**
- **Learn/Input**
- **Tempo**
- **Output Level**

Use the term "press" when pressing a pad or an encoder.
Use the term "press and hold" when pressing a pad or an encoder and holding it down for an extended amount of time. 
Use the term "turn" when rotating an encoder. Turing to the right is clockwise, turning to the left is counterclockwise. 

#### Control combinations

Use `+` for control combinations. The plus sign can be bold or regular.

!!! example "Examples"
    - To create a new kit, press **Shift+Kit**.
    
    - To clear automation, press **Lower**+**Back/Undo**.

    - To map MIDI channel 1 to the Synth Clip, press **Learn+AuditionPad** then play a MIDI note on channel 1.

#### Modulation

`Source1 -> Destination`  
`Source2 -> (Source1 -> Destination)`

Use `->` to refer to a source to destination modulation depth, or to refer to the source to destination mapping itself. Use abbreviated versions of the source and destination names. When referring to modulating the modulation depth of an existing source to destination mapping, use parenthesis around the existing mapping.

!!! example "Examples"
    - Increase `LFO2 -> OSC1 Transpose` from 10 to 20 to modulate OSC1 frequency across a wider range. 
    - Play a note while turning up the modulation depth for `LFO2 -> OSC1 Transpose`. 
    - Adjust the `ENV2 -> (LFO2 -> OSC1 Transpose)` modulation depth to have `ENV2` control how much `LFO2` affects `OSC1 Transpose`. 
    - `MIDI CC2 -> OSC1 Transpose` refers to `MIDI CC2` controlling `OSC1 Transpose`. 