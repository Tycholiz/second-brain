
## What is it?
A compressor is a [[volume|music.engineering.mixing.volume]] function. After a certain threshold of dB, the volume is decreased.
- The result is a reduction in the dynamic range of an audio signal

If we visualize music in a 3D space, where volume is represented as distance from us, a compressor is like a wall that sits between us and the sound. If using a limiter (ie. a compressor with a max threshold), then the wall will not allow the sound to get past that threshold at all.
- [ref](https://youtu.be/TEjOdqZFvhY?t=3138)

The original purpose of a compressor was to reduce dynamics. While they can, and that was their original intention, it isn’t the entire story. They’re actually relatively poor at this job compared to other tools. Think of compressors as tools that help you shape the Envelope of the source. Compressors can reduce or expand the dynamics of a source.

Playing with the attack is a good place to start for beginners because it’s the easiest to hear. Hearing the effect of the release is a little trickier but really great once you get the hang of it. Being able to create depth with just compression and EQ really elevates your mixes, without having to rely on reverb etc to do this for you exclusively.

If you set the threshold lower than the attack, it'll take a bit of time to get down to the new compressed level every time a sound starts, causing it to have a 'punch' or 'snap' like sound when the sound starts.
- Sometimes you like that snap, sometimes you want that snap to push into the limiter/master chain to saturate it a bit. Or even just slap a saturator on the end so the level is still the same as before, but now it has a bit more saturation on the start of phrases.

### Flavors of compressor
The stated goal of a compressor has always been to "tighten the leash on a source". While transparency was always the intent, historically, analog compressors always had their own sound to them. With the advent of the DAW, digital compressors are able to offer true transparency, though the artifact flavor imparted by the analog compressors have since been considered desirable.
- the stock compressors in a DAW usually offer a transparent (flavorless) compressor

## Why use it?
3 main purposes
- better signal/noise ratio (ie. less hiss)
- stabilize the sound image (ie. more presence)
- bring sound elements closer/further away from listener

### Better signal 
if we have quiet parts and loud parts in a song, simply reducing the volume will take care of unintended distortion from the loud sounds, but it will make the quiet sounds too quiet, and lead to hiss. 

### Stabilize the sound image
More chaotic mixes need more compression. Compression will stabilize sounds, giving them more presence. 
- You might to decide to compress one sound moreso to give it more relative presence, or you may decide to compress everything to increase overall presence of the mix

Adding heavy compression to a sound and then turning up the volume is a technique that can do 2 different things:
- make a sound front and centre (e.g. electric guitar)
- prevent a softer sound from being lost in the mix
    - [ref](https://youtu.be/TEjOdqZFvhY?t=3059)

### Bring sound elements closer/further away from listener
As explained [[here|music.engineering.mixing.volume#volume-as-a-measure-of-depth-control]], volume alone does not do a sufficient job of letting the engineer move sounds closer/further away from the listener.

Note: the following is a rough guide

to bring a sound element closer in the mix:
- set ratio somewhere around 3:1 to 6:1
- set a threshold so that gain reduction is only around -2dB to -3dB
- set an [[RMS|music.engineering.mixing.volume#rms-root-mean-square]] value of between 200-250
- add in as much gain as required from the wet output fader.

to push a sound element back in the mix:
- set ratio somewhere around 8:1 to 16:1
- set a threshold so that gain reduction is engaged most of the time, with gain reduction of around -6dB to -10dB
- set an [[RMS|music.engineering.mixing.volume#rms-root-mean-square]] value of 0
- add between 1dB-3dB of gain to the wet output fader.

to bring a sound element up front in the mix
- use settings similar to those suggested for pushing sound elements back in the mix
- add in a lot of gain with the wet output fader (around 9dB, or even more)

## How to use it?
A ratio of 4:1 and threshold of 6dB gain reduction is usually a good place to start

### Mix Bus
Attack + Release times are crucial on the mix bus

Normally set at a 4:1 ratio

SSL G compressor is industry standard

slower attack times will give you more punch, but faster attack times will grab things and help glue them together
    
## Types of compressor
There are 2 types of compressor
- downward
- Upward 

Downward compression reduces the volume of loud sounds above a certain threshold. This is the more common type of compression. 

Upward compression increases the volume of quiet sounds below a certain threshold.

Threshold timing behavior is subject to attack and release settings. When the signal level goes above threshold, compressor operation is delayed by the attack setting. For an amount of time determined by the release after the input signal has fallen below the threshold, the compressor continues to apply dynamic range compression.

The amount of gain reduction is determined by ratio: a ratio of 4:1 means that if input level is 4 dB over the threshold, the output signal level is reduced to 1 dB over the threshold. The gain and output level has been reduced by 3 dB. Another way of stating this is that any input signal level over the threshold will, in this case, be output at a level which is only 25% (i.e. 1 over 4) as much over the threshold as its input level was.

The highest ratio of ∞:1 is known as *limiting*, and effectively denotes that any signal above the threshold is brought down to the threshold level once the attack time has expired.

### Expansion
Some compressors also have the ability to do the opposite of compression, namely expansion. Expansion increases the dynamic range of the audio signal. Like compression, expansion comes in two types, downward and upward.

Downward expansion make the quiet sounds below the threshold even quieter. A noise gate can be thought of as an extreme form of downward expansion as the noise gate make the quiet sounds (for instance: noise) quieter or even silent

Upward expansion make the louder sounds above the threshold even louder.

### Compressing before or after EQ
using EQ in front of your compressor produces a warmer, rounder tone, while using EQ after your compressor produces a cleaner, clearer sound. So, the question you need to ask yourself for each channel in your mix is, “Do I want to EQ the compressed signal or do I want to compress the EQed signal? What sound do I want for this signal?”

* * *

### Where in the FX chain to use compressor.
Compressors should typically be applied after subtractive [[EQ|music.engineering.mixing.EQ]]
- imagine we had a singer who grabbed the mic when singing, resulting in a low rumble at sporadic points in the song. Since a compressor doesn't know the difference about frequencies, the low rumble would cause all frequencies to duck. Therefore, we must EQ out the rumble first so the compressor doesn't get triggered and lower the volume of all frequencies.

Sounds with harsh transients (e.g. handclaps, snare) can be tamed with a compressor with _slow attack_ in order to allow a portion of the transient through. Afterwards, apply additive EQ (~2000 hZ for handclaps) to make the sound more apparent.
- if we had applied the additive EQ before compression, that boost could push the compressor in an unwanted way, and actually negate the EQ's effect.

## UE Resources
- [How to hear compression](https://www.youtube.com/watch?v=K0XGXz6SHco)
- [Parallel Compression](https://www.soundonsound.com/techniques/parallel-compression)