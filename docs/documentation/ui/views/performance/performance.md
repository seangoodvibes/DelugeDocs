# Performance

## Description:

Polyend Play inspired Performance View for the Deluge.

Each column represents a different "FX" and each pad/row in the column corresponds to a different FX value.

Specifications:

  - Perform FX menu to edit Song level parameters and enable/disable editing mode.
  - 16 FX columns
    - 1 Param assigned to each column
  - 8 FX values per column
    - Long press pads (>= 100ms by default) in a column to change the value momentarily and reset it (to the value before the pad was pressed) upon pad release
    - Short press pads (< 100ms by default) in a column to change the value until you press the pad again (resetting it to the value before the pad was pressed)
    - Quickly clear all held values by pressing `HORIZONTAL ENCODER ◀︎▶︎` + `BACK` (resetting FX values back to their previous state)
  - Editing mode to edit the FX values assigned to each pad and the parameter assigned to each FX column
  - Save defaults as PerformanceView.xml file
    - Adjustable default Values assigned to each FX column via `VALUE` editing mode or PerformanceView.xml
    - Adjustable default Param assigned to each FX column via `PARAM` editing mode or PerformanceView.xml
    - Adjustable default "held pad" settings for each FX column via Performance View or PerformanceView.xml (simply change a held pad in Performance View and save the layout to save the layout with the held pads).
  - Load defaults from PerformanceView.xml file

## Usage:

#### 1) Enter performance view from song / arranger views by pressing the keyboard button.

#### 2) Short press (< 100ms by default) a pad in the columns to hold that pad's value (parameter and held value is displayed on the screen)

- Note: If you save the layout while pad's are in a "held" state, the next time you re-load that layout it will re-load the held pad's and change the associated parameter's value based on the previous held state.

#### 3) Long press (>= 100ms by default) a pad in the columns to play the FX but not hold it (when you let go of the pad it will snap back to previous value).

- Note: The long press / short press time used for Performance View can be configured in the global settings menu under `DEFAULTS` as `HOLD PRESS TIME`.

#### 4) Press `HORIZONTAL ENCODER ◀︎▶︎` + `BACK` to clear all "held" FX values.

#### 5) You can Undo/Redo your changes in Performance View

#### 6) You can edit the default values for each pad in the Performance View by entering a [Value Editing Mode](value-editor.md)

#### 7) You can edit the Parameter assigned to each FX column by entering a [Param Editing Mode](param-editor.md).

## Default FX and Colour Assignments
* The default Param and Colour Assignments for each FX column in Performance View are as follows
* Note: if you re-arrange the parameters to different FX columns (e.g. using Param Editing Mode), they will bring the colours noted below with them.
* Params marked "Unassigned" below are available to be assigned to a Performance View column with Param Editing Mode.

Columns:

Red:
1 = LPF Cutoff
2 = LPF Resonance
Unassigned = LPF Morph

Orange:
3 = HPF Cutoff
4 = HPF Resonance
Unassigned = HPF Morph

Yellow:
5 = Bass EQ
6 = Treble EQ
Unassigned = Bass Frequency
Unassigned = Treble Frequency

Light Green:
7 = Reverb

Light Blue:
8 = Delay Amount
9 = Delay Rate

Light Pink:
10 = MOD-FX Rate
11 = MOD-FX Depth
12 = MOD-FX Feedback
13 = MOD-FX Offset

Dark Pink:
14 = Decimation
15 = Bitcrush

Dark Blue:
16 = Stutter Rate + Stutter Trigger