
Remember that apparent volume is what matters, not dB. The shape of the soundwave also affects how loudly we perceive something
- even at the same dB level, a chainsaw will sound much louder than a flute because of the shape of the soundwave.

Once an instrument playing a certain pattern is heard, it is safe to blend back into the mix, where even if it is barely audible, the listener will be able to clearly discern what is being played, due to the fact they've already heard it.
- ex. a common pattern for a song has a guitar playing solo, only to be joined by other instruments progressively. Once these other instruments get added, it's fine to lower the volume on the guitar, since its distinctive pattern has already been heard and the listener can fill in the blanks on their own.

It is not uncommon for the engineer to vary the volume faders throughout the song as dynamics change (ex. instruments are added, entering a new section of the song etc.)
- [[compressors|music.engineering.mixing.compressor]] can only do so much before they start sounding unnatural.

The volume fader is the volume of the track after the FX pipeline has been applied to it. 
- It is the volume level that will be piped into the it's `send` (ie. the next place in the pipeline)

### Relative volume
When doing your initial volume setting of each track, it's easier to scope small and gently expand outward
- ex. volume-match your cellos first, then your string section, then your brass section, then your string section AND brass section, and so on.

## Framework: Levels of volume
A useful framework for thinking about relative (apparent) volumes is to place each instrument in one of 6 levels

- positioning of snare is quite varied, and depending on the genre, can appear from level 4 to level 2
  - [ref](https://youtu.be/TEjOdqZFvhY?t=6540)
- vocals can also appear at various levels depending on genre and how strong the vocalist is
  - [ref](https://youtu.be/TEjOdqZFvhY?t=6385)
- kick drum may appear at various levels as well.
  - ex. Kick drum in Jimi Hendrix' music is at around level 4 and can barely be heard
  - ex. Heavy metal commonly places kick drum around level 2
  - [ref](https://youtu.be/TEjOdqZFvhY?t=6668)
- bass guitar was traditionally quite low at level 3/4, but has progressively gotten louder and is commonly found at level 2/3
  - commonly, the fewer instruments in the mix, the louder the bass, since it does a good job of filling out the space between the speakers
- consider that a song can have varying ranges of volume levels, that is often influenced by genre
  - ex. some music has a range than spans only volume levels 2-4, while others might cover all
    - Pink Floyd's music typically has quite a wide range of volume levels

### Level 1
An unusually loud volume. Placing instruments at this level is the exception rather than the rule. If not done carefully it can sound like an error
- ex. the alarm clocks at the start of Time by Pink Floyd

### Level 2
Lead instruments and vocals (when vocals/lyrics are meant to be the main focal point of the song)
- ex. Bob Dylan's music normally has vocals at this level
- ex. "kick" drum in hip hop, kick drum and toms in heavy metal

### Level 3
Primary rhythm parts
- ex. guitar, keyboard, vocals (when not meant to be the dominant focal point)
- ex. kick drums (heavy metal), snare (dance music), toms, cymbals, hi-hat (occasionally)

### Level 4
Rhythm beds and chordal pads
- ex. background piano, background strings, keys, guitar
- ex. drums (jazz)
- ex. hi-hat

When reverb is noticeable as a sound on its own, it is usually at this level

### Level 5
- ex. Kick drum (jazz, big bang music)
- ex. Background vocals

lots of FX and reverb live at this level so you can only hear them if listening closely

### Level 6
Soft and hard to detect sounds
- ex. whisper sounds found in Pink Floyd music

* * *

### Gain Staging
The source signal of an audio track goes through a pipeline before it ultimately arrives at the master bus.
- ex. this pipeline might be:
  1. the guitar signal is WAV audio track
  2. the track is in an `Acoustic Guitar` bus (ie. folder in Reaper)
  3. the `Acoustic Guitar Bus` gets routed into the `Acoustic Verb` send, which gets routed to the `Guitars Bus`
  4. and so on

Some steps of the pipeline will naturally involve some level of volume increase
- ex. compression, reverb and EQ are all stages that add volume to the mix

Because one of the first steps of mixing is to set the fader levels, we don't want our compressor/EQ adding perceptible volume to the track. Therefore, when we are happy with the parameters of our FX, we need to A/B test it by bypassing it on and off. Adjust the volume level of the `B` to match the `A`.
- ex. Imagine we are A/B testing our compressor on the guitar. We toggle the FX on, and adjust up/down the post-FX gain (?) so that it matches the perceived volume level when the FX is off
 
* * *

## Measures of Volume
A decibel (dB) is just a ratio, there has to be a reference level for it to become a unit (of sorts). 

### dB SPL (Sound Pressure Level)
When the average person talks about "decibels" they are usually (unknowingly) talking about dB SPL which has some arbitrary definition of the lower limit of human hearing as a reference (according to wikipedia it's about as loud as a mosquito flying 3m away)
- ex. you can't exactly hear a gun shot and say 'that was 80dBs', because it relates to how far you are from the source and what reference you are using. If you were to move 50% closer, that 80 dB (SPL) would become 86 dB SPL, because now your perspective is different

### db FS (Full Scale)
When talking about audio in the digital realm, dBFS is used, but instead of the reference being the quietest possible limit, it's the loudest (imposed as a standard) and thus negative values are used to count back from the top. Any signal that passes above 0dB FS gets chopped off, which is known as digital clipping.

### RMS (Root Mean Square)
RMS represents the average (also called “integrated”) loudness of a signal. 
- It will typically take a measurement every 300ms, which means whatever peaks occur within that time frame get averaged out for the RMS reading. So RMS isn’t as precise as peak metering, but it actually gives us a better understanding of overall loudness based on the average strength of the signal.

RMS is useful for whenever you want a reading closer to a person’s actual perception of loudness.

RMS is usually the unit used for the master track.

### Loudness Unit Full Scale (LUFS)
LUFS is a measurement of perceived loudness obtained by measuring the average level over time.

Two pieces of music that register identical LUFS readings should sound like they’re at the same level, regardless of whatever the peak or RMS readings say
- therefore, LUFS offers a benefit to the mastering process when we want all tracks to have the same volume level.

LUFS-M - Momentary Max
LUFS-S - Short-term Max
LUFS-I - Integrated

### Loudness Range (LRA)
The lower the number, the less dynamics. 
- since classical music tends to have many loud parts and quiet parts, you might find LRA of 9+, whereas rock music, which is typically more stable is usually around 5-6.
- Note that this is not about dynamic range, but rather, musical dynamics.

