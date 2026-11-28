
### Multi-stage compression (a.k.a serial compression)
Multi-stage compression involves using multiple compressors each applying a few dB of gain reduction.
- ex. when compressing vocals, we may apply the first compressor (a fast compressor) to tame the sharpest peaks in the dynamic range, then we might apply another compressor (a slow compressor) to "glue" everything together.

The result is that we retain the same amount of control, but because each compressor isn't working as hard, we get a much more natural sound.
- therefore, this technique is used to preserve the natural tone that our sound has, while still getting the compression we're after.

Different attack and release times are a good idea
- use fast attack/release times on first compressor to control transients
- use medium attack/release times on 2nd/3rd to shape the tone

[How to](https://www.musicianonamission.com/vocal-compression-how-to-compress-vocals/)

### Parallel compression
Parallel compression is blending an uncompressed sound with a heavily compressed sound
- we must determine the appropriate level of blending to find the desired balance between control and naturalness.

Parallel compression pushes a track forward and makes it sound bigger or more aggressive

The benefit of using parallel compression is that it allows the engineer to achieve a more even and consistent sound while still preserving the natural dynamics and character of the original signal. By blending the compressed signal with the original signal, the engineer can achieve the desired level of compression without completely squashing the dynamics of the sound.

Sounds great on vocals that just aren't sitting well in a mix and are getting buried.
- here, when the uncompressed track drops below a threshold, the compressed track comes up and makes the track sound fatter.

In your DAW, make a copy of the track you want to parallel compress and put a compressor on it. You’ll want to hit it hard, so exaggerate your compressor’s settings even to the point in which it doesn’t sound pleasant and starts to distort.

Make sure the original track is at the desired level, and bring up the compressed copy’s fader until it sits just beneath the original. Parallel compression gives the impression of control without sounding completely squashed. It’s a fantastic way to compress vocals, but works with almost any individual instrument, too!

### Sidechain compression
Sidechain compression is a type of compression where the effect level on one instrument is controlled by the volume level of another instrument. 

A typical use-case is on tracks that compete in the same frequency space.
- ex. make the compression level on a bass guitar controlled by the output volume of the kick drum. The idea is that when the kick drum sounds, the bass guitar gets more compressed so that it can stay audible in the mix.
- ex. imagine you had a bass synth sound along with a kick drum every measure. In order to make the kick drum more present and punchy, we duck the sound of the bass synth every time the kick drum is hit.

Because this affects how 2 or more similar-frequency sounds sit together in a mix, this is something we want to do before EQ.
- in other words, this allows us to give each instrument its space without messing with the frequencies.

The general way we achieve sidechain compression is by 
- opening up additional channels on the track we want to compress
- sending the signal from our trigger track (ie. the track that will trigger the compression to occur) into those newly opened channels
- setting the compressor plugin to apply only in response to those signals 

Side-chain compression has prominent usage in dance music

#### Example: Reaper usage
say you want your bass track to compress (or duck) a little to let your kick drum occupy the primary space of that frequency in those moments...

what you would do is go to your bass track and click the i/o button (input output). within that you will see a receive section, add your kick drum. now go slightly below that and change the output of the from 1/2 to 3/4 (this will be an aux output you will recognize with your compresson in the next step)

now go to your bass effects and add a reacomp (reaper compression) to the front of your chain. inside your compressor effects you will see a drop menu for the aux 3/4 (this is where your kick was sent. now solo your kick and bass tracks (just to audition for now), make sure to set your ratio, drop your threshold to a desired db, and watch the kick duck the signal down when it plays.

basically the bass track now contains both the bass signal and the kick drum signal but the kick signal (on the bass track) is routed to outputs that aren't being sent to the master, which triggers the compressor

#### Ducking
Ducking is an effect commonly used in dubbed foreign films, where an actor speaking in a foreign language will get quieter once the dubbed voice comes in. The original actor's voice is linked to the overdubbed voice and will decrease in volume when the overdubbed voice reaches a certain volume level.

Another example is for use by DJ, whereby when he starts speaking, the music decreases in volume.

Ducking is an effect that is achieved with a compressor's sidechain input.

Ducking can also be used to achieve the well-known and very popular 'pumping' effect

#### De-essing
De-essing is a technique achieved through side-chain compression

### Multiband compression
A multiband compressor is a compressor that works on a specific set of frequency ranges, instead of the whole track.

You can actually use a multiband compressor in place of an EQ, and in some cases they are more effective than EQs
- in fact, in cases where you want to radically alter a sound, a multiband compressor may be the way to go.

note: Multiband compression must be used with care as it can easily destroy a mix.
- it's been said not to use multiband compression if you are getting your music mastered by someone else.

Examples:
- ReaXComp