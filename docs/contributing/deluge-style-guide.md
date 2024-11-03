# Deluge style guide

This Deluge-specific style guide defined how to refer to song parts, views, controls, and display elements.

## Terminology

### Parts of a song

Song
: A discrete creative project, generally aligned with one (but sometimes several) project files on the Deluge.

Project
: A file on the SD card associated with a song. Use this only when referring to the file system, such as saving or deleting projects.

Track
: A single instrument or layer in a song. Each track is one of the following types: synth, drum kit, MIDI, CV, audio, or DX7. Tracks contain one or more clips. NOTE: Don't use "track" to mean song or project, such as "track tempo". Use "song tempo".

Clip
: A stored sequence of notes or parameter automation associated with a track. Each track can have multiple clips.

Parameter
: An adjustable value, such as filter frequency, reverb time, or volume. Some parameters can be automated.

### Views

- Capitalize view names
- Don't use bold unless referring to the text that appears on the display

For consistency, refer to the views as follows:

- Song Row View
- Arranger View
- Song Grid View
- Keyboard View
- Performance View
- Automation View
- Velocity View
- Chord View
- Chord Library View

### Display elements

- When referring to elements on the OLED display, use **bold** and Title Case.

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

#### Control combinations

Use `+` for control combinations. The plus sign can be bold or regular.

!!! example "Examples"
    - To create a new kit, press **Shift+Kit**.
    
    - To clear automation, press **Lower**+**Back/Undo**.