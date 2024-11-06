# Ports
## Audio

### Inputs

#### Line input

For recording from another device’s line output. The line input uses TRS 1/4” / 6.35mm connector, which may accept a single-ended / unbalanced signal, a differential / balanced signal, or a stereo signal. 

Input impedance: 4k.

#### Mic input

For recording with an external microphone use the 3.5mm / 1/8” jack. Gain is set via the “mic gain” switch, which also affects the internal microphone. Stereo and mono microphones are supported. 4.5V plug-in power is supplied on the tip and ring of the connector, each through a 3.9k resistor.

#### CV, gate, and trigger clock (“CLK IN”) connectors

These all have the signal on their “tip”, ground on their “sleeve”, and their
“ring” connected to ground via a 10k resistor.

### Outputs

#### L / MONO and R balanced outputs

The Deluge’s main audio outputs are two quasi-balanced (that is, resistor-balanced but not differential) 1/4" connectors. They will work with non-balanced cables too. For best noise rejection, use balanced cables when connecting the Deluge’s outputs to balanced / differential inputs. 

Output impedance: 47 ohms.

Deluge will detect if only the “L / MONO” output has a cable inserted (but not the “R” output or headphone output), and will output all sound in mono.

In this case all panning and ping-pong delay will be deactivated, and stereo samples will be condensed to mono. This allows you to work on your music on a stereo setup, but not necessarily need to change anything if you are faced with a mono setup.

#### Headphone output

This can drive headphones, or can be used to connect other equipment with a 3.5mm / 1/8” connector - perhaps computer speakers or a car stereo.

### MIDI
#### MIDI in
#### MIDI out
#### USB MIDI

The Deluge’s USB type-B connection can be used as a connection to your computer as a USB MIDI device, for use in any software that supports MIDI.

### USB host

The Deluge can use its USB type-B connection to act as a USB Host. This requires Deluge to be DC powered, a USB device connected and then Deluge to be powered up.