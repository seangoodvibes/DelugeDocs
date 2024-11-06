# SD card

The Deluge uses SD (or SDHC) card storage to load and record audio samples, store presets and save songs. Typically a 16GB or 32GB is recommended, but any size can be used, formatted to FAT32. The Deluge’s firmware can also be updated via the SD card.

The Deluge is supplied with a formatted SD card loaded with the factory library. Samples are streamed directly from the SD card when in use, making it an integral part of the device. Ensure the card is inserted in Deluge when in use.

## File Structure

The Deluge’s SD card contains the presets for kits and synths in XML format which stores the parameter settings and for kits points to the specific samples used.

## Slot

- SD card used for presets, streaming samples, firmware updates and storage. Any size, formatted to FAT32. Insert pins-up.
- Be careful to slide the SD card in straight and not angled, otherwise SD card can fall inside the Deluge

## Formatting

For best results format the card with `32kB cluster size`.

## Card Selection

Most consumer SD cards are intended for cameras and video cameras, and the speeds advertised are for reading and writing a single large continous file. For Deluge what matters is _random access speed_. This is often not mentioned at all. A1/A2 class is an indication of a card intended for "application use", and should mean good random access speed. (A2 is not supported by Deluge: the card will work, but isn't going to be any faster.)

While specific testing for Deluge is still in early steps, in addition to the information below you may want to refer to the [recommendations for the Dirtywave M8 tracker](https://dirtywave.com/pages/recommended-microsd-cards).

### Good

- [Kingston Canvas Go! Plus microSD card](https://www.kingston.com/en/memory-cards/canvas-go-plus-microsd-card). Tested size 64GB. Note: microSD, not full size! Achieved 9-12 simultaneous streams.

- [Kingston Canvas Go! Plus SD card](https://www.bestbuy.ca/en-ca/product/kingston-canvas-go-plus-128gb-170mb-s-sdxc-memory-card/14707230). Achieved 12 simultaneous streams with no dropouts

### Decent

- Sandisk Extreme Pro. Achieved 6-8 simultaneous streams.

### Poor

- Verbatim Premium (stock card that comes with the Deluge). Achieved 3-7 simultaneous streams.

Test procedure - export arranger stems for a song, load them into a kit, and watch for dropouts. Kit is important as audio clips will paper over the dropouts and attempt to resume, kit rows will stop playing. The song must have enough tracks for the total audio size to exceed available memory, 12 stereo tracks at around 1 minute should do it