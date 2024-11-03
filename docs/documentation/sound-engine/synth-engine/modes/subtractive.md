# Subtractive

The LFOs can modulate the oscillator transpose at audio rate, which imitates FM synthesis while in subtractive synth mode.

1. Initialize a synth clip with **Shift+Synth**. Set `LFO2 Shape` to Sine.
1. Set the `LFO2 Rate` to 40.
1. Play a note while turning up the modulation depth for `LFO2 -> OSC1 Transpose`. Set this modulation depth to 10 for now, and press `Select` to modulate this modulation depth using `ENV2`. Set `ENV2 -> (LFO2 -> OSC1 Transpose)` to a value of 50.

When a note is played, `ENV2` begins to move through its stages modulating the modulation depth of `LFO2 -> OSC1 Transpose`. `ENV2` decays to the value set by `ENV2 Sustain`.

!!! example "Examples"
    - If `ENV2 Sustain` is set to 25, `LFO2 -> OSC1 Transpose` will settle to the set value, in this case 10.
    - If `ENV2 Sustain` is set to 0, `LFO2 -> OSC1 Transpose` will settle towards 0.
    - If `ENV2 Sustain` is set to 50, `LFO2 -> OSC1 Transpose` will settle towards a value higher than 10. 

From here, there are many possibilities.

!!! example "Experiments"
    - Adjust the waveshapes of the LFOs for different tones.
    - The `LFO2 Rate` can be modulated with another source to get variation in tone.
    - `ENV2 Sustain` can be modulated using LFOs.
    - `LFO1` could be used as another audio rate modulation source.
    - The LFOs could be used to FM the `LPF Frequency` instead of `OSC1 Transpose` for a different effect. 
