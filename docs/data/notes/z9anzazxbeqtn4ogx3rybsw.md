
see [[compressor param Dendron note|music.engineering.mixing.compressor.param]] for param explanations that are not specific to ReaComp

### RMS size
RMS size is an averaging calculation that leverages previous values to alter the signal that the compressor is reacting to. The RMS size is how much it time it references to create the average. On percussive content this will make a big difference to how it reacts to the signal.
- ie. RMS size is the window of time over which the signal/input level is root mean squared

RMS (root mean square) compression means that the compressor will react according to the “average loudness” of the input or sidechain signal. As the “average” of the compressor control exceeds the threshold, the compressor will kick in.

Turning up this control basically means the effect responds more to the average level than to the peaks.
- A low RMS will be a lot "grabbier", quickly reacting to sudden changes in level, while a high RMS will be more "smoothing", making subtler changes over a long period of time.

Like knee size, RMS size smooths the way the compressor reacts to the signal.
- anal: Think of this like blurring a picture. In photo editing software, we can reduce the sample size of an image, making it blurrier. RMS size is analogous to this.

the longer you set the RMS window, the lower the level that hits the detector and shows on the meter, and the lower the threshold needed to get the same amount of gain reduction.

### Low Pass / High Pass
These settings allow us to set filters, so that only that part of the signal that falls within the specified frequency range will be compressed.

Often, these can be simply left alone, and you can do pre/post EQ

## Techniques
### Transparent volume leveling
example use-case: vocals

This technique is to be used near the final stages of a mix. That is, the dynamics of the mix should have already been tamed by the time this technique is applied.

Put a compressor right on the Master track, to get a bit more "loudness" without losing so much transient information.

The trick is to set the RMS window pretty big, but then set the pre-comp to somewhere around half the RMS window. 
- This way, the compressor is reacting to the average level around the current sample - both past and future - so that if one bear is significantly louder than the next, it sort of gently dips the volume leading into the louder hit, and then comes back up afterwards in a pretty natural way
- When pre-comp is exactly half of RMS, then it is applying maximum gain reduction exactly when it is loudest, it heads down a little early, and comes back a little late, and it lets anything fast that happens kind of just sail on through. If pre-comp is a little less than half, then it's a little more like a traditional attack/release, in that it reaches maximum crush a little late. Going the other way is like having a very timid soundguy anticipating your moves and turning down the fader when it looks like your going to get loud.

Attack and release are basically built into the process, so set those parameters to 0, and use a very low ratio - 1.1 or 1.2
- Basically, the relationship of the pre-comp to the RMS time determines your attack/release times

for even greater transparency, set the threshold so that it just barely starts squishing on some of the louder parts, and then crank the knee where up so that it's almost always doing just a tiny bit, but it's almost always in the knee, and almost never hits the full ratio.