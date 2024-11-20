# Clip

Clips are unique instances of a track and include the additional building blocks (e.g. sequences, samples, modulation) required to generate an output (e.g. sound, midi, cv).

Based on the track type, the clip will either be an Audio Clip or an Instrument Clip.

A single clip instance can only be assigned to one track. A track may have many clip instances assigned to it (this allows you to create variations of a track).

## Clip settings

### Type

A clip an be an Audio clip or an Instrument clip.

#### Audio

An audio clip belongs to an Audio Track.

#### Instrument

An instrument clip can belong to a Synth Track, Kit Track, MIDI Track, or CV track.

### Name

You can set the name for each clip.

### Mode

A clip can operate in infinite (default), fill, or once mode.

#### Infinite

The default clip mode. Once launched, a clip will loop indefinitely.

#### Fill

Instead of aligning a triggered clip start, a fill clip is designed to play at the end of a loop, coming to an end at the point of starting the next loop. 

When triggered it will automatically be scheduled to start so that it finishes at the start of the next loop. 

If the fill clip is longer than the remaining time, it is triggered immediately at a point midway through. 

The loop length is set by the longest playing clip, or by the total length of a section times the repeat count set for that section.Note that a fill clip is still subject to the one clip per instrument behavior of the Deluge. 

Fill clips can steal an output from another fill, but they cannot steal from a non-fill. This can lead to some fills never starting since a default type clip has the needed instrument. This can be worked around by cloning the instrument to an independent copy.

#### Once

When triggered it will schedule itself to start at the start of the next loop. Then it will schedule itself to stop, so it just plays once. This type of clips also work when soloing them, they will solo just for one loop and unsolo after that.

Limitation: a Once clip is still subject to the one clip per instrument behavior of the Deluge, A Once clip can steal an output from other normal clips, so take that into account when you plan your performance.