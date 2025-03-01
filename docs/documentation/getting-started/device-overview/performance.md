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

## From the manual

### Processing power and CPU management

Deluge does not enforce firm limits on how many tracks or voices may sound at once thus allowing the user as many as they wish. The ultimate limitation will inevitably be based on Deluge’s CPU loading especially from concurrent voices or effects. Under conditions of high CPU loading, Deluge will switch off a synth or sample voice to lower its load. Deluge will attempt to do this in the most subtle way possible, preferring to switch off voices which are “releasing”, and those which have been sounding for the longest time.

Unaffected sample voices are very light on the CPU. This has been tested with a measure of up to 110 sounding at once. For synth voices, the most simple ones are light enough to allow around 64 to play.

The Deluge’s analog-modelled oscillator types and drive filter consume a little more CPU than the other types, but not enormously more.

Considerations for CPU power:

- Analog-simulated delay, time stretching, and pitch shifting (where pitch and time are treated independently - including live audio input) are the highest CPU users.
- All other effects and synth features, though lighter, will add to the CPU’s load as well.
- Synths with unison switched on will multiply the amount of processing power that that synth consumes.
- Arpeggiation can generate a lot of CPU-eating voices very rapidly, which can add up if polyphony is on (is set to POLY) and if the release time is long. Try changing these parameters if you notice voices cutting out on your song.
- There is a slight CPU overhead for each sound present in the Deluge’s currently loaded song - even if it is not sounding at a given moment. This may begin to affect CPU performance if you have more than 50 to 100 sounds loaded. For this reason, you may wish to refrain from importing large folders of samples as kits where these are not in-fact used. Multi-sampled instruments, count as just one sound regardless of how many separate samples they contain.
- Voice priority can be manually set for a sound, to tell the Deluge which voices to consider (or not) dropping first - see sound editor .
- See sample interpolation / pitch for some additional notes on CPU usage.

### Sampler Interpolation / Pitch

Whether or not actual “pitch shifting”, the process of treating pitch and speed independently, is applied, another process called interpolation is needed anytime a sample needs to be played back at a different pitch, or if its sample rate is different to the Deluge’s native 44.1kHz.

Since firmware V2.1, Deluge utilises 16-point windowed-sinc interpolation for high-quality sample pitch adjustment with minimal aliasing. If you prefer the more “bitcrushed” sound of linear interpolation, which was used prior to V2.1, see the INTErpolation setting in the sound editor.

Songs and presets created with pre-V2.1 firmware which include sample pitch adjustment will continue to default to linear interpolation, to keep your older projects sounding the same.

The 16-point windowed-sinc interpolation uses a little more CPU power than the lower-quality linear interpolation, but not very much more, thanks to the hardware acceleration features of the Deluge’s CPU. If the Deluge’s CPU becomes overloaded, it may revert to using linear interpolation in some cases. It is not recommended that you manually switch to linear interpolation purely for the purpose of saving CPU power - it won’t have this effect in all cases.

### Sample and RAM management

The Deluge streams audio samples directly off the SD card, meaning there is no practical limit on the amount of sample content that may be used per song, and the user does not have to wait for all sample data to be read when loading a song.

You may eject the SD card at any time, the only adverse effect being that if the Deluge is playing any sample, it may stop, and samples may not play correctly until the card is reinserted.

The Deluge has 64MB of working RAM, which is mostly available to hold the currently loaded song’s synths, parameters, and sequenced notes. It’s unlikely that the 64MB limit would ever be reached - this would be enough to hold over 2 million notes.

There may be cases, if both songs contain a lot of samples (i.e. near to the Deluge’s 64MB RAM limit), where the newly loaded song may fail to play some sounds for the first couple of seconds. However, the Deluge does everything it can to avoid such a case, by first discarding any not-currently-playing samples in the old song, and if necessary delay the loading of any not-currently-playing samples in the new song until the old song has been discarded completely.
