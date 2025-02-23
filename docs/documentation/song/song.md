# Song

A song is a discrete creative endeavour, such as an arrangement, sketch, 8-bar loop, jam, live recording template, or musical experiment. A song is always associated with at least one song file on the Deluge.

## Workflow

An example high level workflow for working with SONGS on Deluge:

``` mermaid
stateDiagram-v2
    Start --> NewSong: New song <br> [SHIFT] + [LOAD], [LOAD]
    Start --> ExistingSong: Load song <br> [LOAD], turn (SELECT)
    NewSong --> SessionMode
    ExistingSong --> SessionMode
    SessionMode --> RowView: Default
    SessionMode --> GridView: Optional <br> Hold [SONG] + Turn (SELECT)
    RowView --> EditSong
    GridView --> EditSong
    EditSong --> EditClip: Select the clip to edit <br> Hold [PAD] or the row to edit or select a clip
    EditClip --> ClipParameters: Edit clip parameters while in Session Mode <br> Hold clip [PAD] and adjust
    EditClip --> ClipView: Edit clips <br> Press [CLIP]
    ClipView --> EditSong: Continue building a song <br> Option to arrange <br> Press [SONG]
    EditSong --> SongFX: Tweak the Song master parameters in Session mode <br> Enable [AFFECT ENTIRE]
    EditSong --> RecordToArranger: Capture a full arrangement
    RecordToArranger --> ArrangerMode: Edit Arrangement
    EditSong --> Save
    Save --> End

    NewSong: New song
    ExistingSong: Existing song   
    SessionMode: Session mode   
    RowView: Row view
    GridView: Grid view  
    EditSong: Edit Song
    EditClip: Edit Clip
    ClipParameters: Clip 'Affect Entire' controls
    ClipView: Clip view <br> Press [PAD] to select clip view
    SongFX: Song FX
    RecordToArranger: Record from Session mode into Arranger mode
    ArrangerMode: Arranger Mode <br> Press [SONG] while in Session Mode to switch to Arranger Mode
    Save: Save <br> [SAVE] to save the song.
```

## Master Settings and Parameters

There are a number of master settings and sound parameters that can be configured that apply to the entire song project.

### Settings

#### Scale

#### Swing

The swing feature provides a rhythmic adjustment that brings a more natural and organic feel to songs and operates generically and not at an individual note level.

The swing internal setting can be adjusted in the settings menu under swing interval and is saved as part of a song. New songs revert to default while saved and reloaded songs will retain the swing interval setting.

##### Adjusting the swing interval setting

1. Open the settings menu by pressing [SHIFT] + press (SELECT).
2. Turn the (SELECT) control to navigate the menu top level and select SWING INTERVAL
3. Press (SELECT)
4. Turn (SELECT) to choose between 2 bar, 1 bar, 2nd, 4th, 8th, 16th, 32nd, 64th, 128th note intervals. 16th is the default setting.
5. Press [BACK / UNDO] to back out of the menu when the parameter has been changed or at any time in the menu to back up.
6. The swing interval setting is saved as part of a song. New songs revert to default while saved and reloaded songs will retain the swing interval setting.

#### Tempo

Tempo can be set manually or a tap tempo option is available.

### Parameters

#### Level
#### Pan
#### Filters
#### FX

## Modes

There are two modes you can use to create and play a song on the Deluge: [Session](./song-modes/session-mode.md) and [Arranger](./song-modes/arranger-mode.md)
