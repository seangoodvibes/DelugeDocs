# Performance

## CPU and Memory Management

Provide an overview of what contributes to high CPU usage and memory consumption. Both of which contribute to culling.

- samples take memory, voices and fx take cpu
- You can run out of memory and cpu power independently, both cause culling
- performance is based on how long it takes to render a sound
- The more complex a voice, the longer it takes to render, the higher the cpu usage
- The more samples you have, the more memory they consume
- If you try to render something new and you’ve hit limits in terms of the deluge's cpu usage and memory, it needs to cut back on stuff to allow the new stuff in - this is culling
- the higher the cpu usage / memory consumption, the more noticeable the effect of dropping voices / samples
- Under high, but not high enough load, a voice may be dropped by releasing it, instead of it cutting off right away (force vs hard culling)

All the above should be tied into a discussion on polyphony, voice priority, etc

- You’ll get culling when rendering 128 samples is taking longer than outputting them or when the sd card can’t read the next cluster before it’s needed
- samples take almost no cpu time, they only stress the sd card
- Take a look at the scheduler stats print out and in sample heavy songs you can be culling at under 50% cpu usage
- I think it’s important to differentiate - filters in an fm synth double the cpu load per voice

More info from Mark:
- Reduced 7SEG performance from Official to Community Firmware
- There’s a significant difference in performance from 7seg to OLED and the community firmware is based on the OLED codebase
- you lose about 5 voices for the oled version
- the firmware grew by about 100k to accomodate the OLED and that takes up memory that would otherwise be used for samples
- they're running out of ram/streaming bandwidth and when I compared to the last official OLED release they performed the same. It's multi faceted since less ram means less ability to cache, which means more streaming is required, which requires more time spent servicing the SD card etc. etc.
- I don't think it handles situations where the bandwidth is overwhelmed cleanly (e.g. if you're streaming 9 stereo samples when there's only bandwidth for 6 it'll tend to drop 4-5 voices instead of 3) and that makes it very sensitive to having less ram available

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
