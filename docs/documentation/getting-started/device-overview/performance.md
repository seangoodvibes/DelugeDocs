# Performance

## Scheduler

Provide an overview of the scheduler and how it helps the Deluge manage performance

## Synth voices and samples

The Deluge can handle much fewer samples than synth voices.

Here are some approximate numbers:

- 100 voices for FM and Subtractive based synths without filters
- 60 voices for normal synths
- 30 voices for DX7 synths
- 30 voices for wavetable / very short sample based synths
- 24 mono (12 stereo) samples streaming at once with a good SD card

With regard to samples, the Deluge is limited by how many samples can be read from the SD card at once. For suggestions on the types of SD card's to use, please refer to the [SD Card](sd-card.md) page.

There are also other factors that can lead to reduce synth voice and sample performance:

- Heavy automation use
- Heavy modulation use
- Heavy filter use
- Long sustains
- High polyphony, with lots of note on's triggering at the same time
- Higher bitrate samples (e.g. 32 bit instead of 16 bit)
- Stereo samples (instead of Mono samples)