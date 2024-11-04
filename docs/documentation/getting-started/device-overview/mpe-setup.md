# MPE setup

## MPE overview

MPE is essentially a hack on top of normal midi channels to allow per note pitch bend, aftertouch, and timbre control (cc74). It works by dividing the 16 midi channels into two zones - upper and lower - which can each have 0 to 15 channels in them. This allows a single zone with 15 member channels, two zones with 7 member channels each, or any combination in between. If not all the channels are in use for MPE zones then the remaining channels will function as normal midi channels. This allows configurations like using channel 10 for drums while all other channels are in the upper or lower mpe zone.

An example config might look like this - Lower zone of 7 and an upper zone of 6, leaving channel 9 as a normal midi channel
```
16. Upper Zone Master   
15. Upper Zone Member   |
14. Upper Zone Member   | 
13. Upper Zone Member   |
12. Upper Zone Member   | 6 member channels
11. Upper Zone Member   |
10. Upper Zone Member   | (last upper zone member)
9.  MIDI Channel 9
8.  Lower Zone Member   | (last lower zone member)
7.  Lower Zone Member   |
6.  Lower Zone Member   |
5.  Lower Zone Member   | 7 member channels
4.  Lower Zone Member   |
3.  Lower Zone Member   |
2.  Lower Zone Member   |
1.  Lower Zone Master 
```
## Configuration

### MIDI device
In the deluge MPE is configured per device in the midi menu, at `settings->midi->devices->device name->mpe`

#### Zones
The lower option configures the number of channels in the lower zone, and the upper option configures the number of channels in the upper zone. The zones cannot overlap, and any channel between the zones will be normal midi. Setting a zone to 0 disables it.

This is controlled seperately for inputs and outputs. Input settings control whether incoming midi is treated as MPE, and output settings control whether MPE or normal midi get sent to the device

### MPE clip settings

Deluge offers some settings to help match external devices. Access these settings by clicking select while in a midi clip

#### Bend Range
The bend range can be set seperately for the master channel and for the member channels. This allows using a pitch wheel alongside MPE. Typical settings are 2 for `normal` and 48 for `mpe`. If using a controller with full pitch bend such as the linnstrument or the seaboard this setting must match the controller in order for bends to be in tune

#### MPE output conversion settings

Deluge offers some output settings to help send MPE to synthesizers that don't implement the full MPE standard

#### Convert y to CC1

A common partial implementation of MPE recieves y axis on mod wheel. Enable this toggle to send y axis as mod wheel (cc1) instead of cc74. This is needed for the dreadbox nymphes, the Sequential 6 series, and the audiothingies micromonsta (and probably more)

#### Convert to monophonic expression

Deluge can also convert incoming mpe to non-mpe output as best as possible. Settings for this are available in the midi clip menu under `poly expression to mono` (7seg:`POLY`). You can choose to convert MPE aftertouch to either channel or poly aftertouch, and choose to convert y axis to mod wheel (will be added to any incoming mod wheel from your mpe zone)

## Troubleshooting

### Some notes are being missed

The most likely cause is mismatched mpe settings. If the device is sending on more channels than deluge thinks are in the MPE zone then the notes won't sound

### Timbre control isn't recognized by my external synth

Some synths need to receive CC1 instead of CC74. In the midi clip setting you can enable `Send Y as CC1` (7seg: `y->m`)

### Aftertouch/timbre sometimes applies to all notes

This indicates that the deluge is receiving some notes on its mpe master channel. Make sure your device and deluge agree on what mpe zone is being used