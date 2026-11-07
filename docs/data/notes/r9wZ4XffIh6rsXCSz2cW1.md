
Audio interfaces convert microphone and instrument signals into a format your computer and software recognize.
- also routes audio from your computer out to your headphones and studio monitors

Audio interfaces are closely related to sound cards
- a sound card is optimized for audio playback
- an audio interface is optimized for low-latency analog-to-digital conversion.

### How audio goes from analog to digial
Digital audio is about taking an analog sound wave and extracting certain characteristics from it— its frequency, its amplitude... We take these and we convert it into data so that it can be read by a computer.

The process by which a sound wave is converted into data is carried out by taking a series of snapshot measurements, or samples.
- each snapshot is taken at an even interval of time, and snapshots are taken 1000's of times per second. We measure the amplitude of each interval of time, and output the samples that represent the original sound wave.

Because so many snapshots are taken, we are able to realistically reconstruct the analog wave.
- The principles of [[math.calculus]] apply here, in that that we can get infinitely close, but not 100% of the way there.

![](/assets/images/2021-12-16-19-58-49.png)

### Sample Rate
The *Sample Rate* measures the interval of time at which these samples are taken.
- measured in kilohertz

The most common audio sample rate you’ll see is 44.1 kHz, or 44,100 samples per second. This is the standard for most consumer audio, used for formats like CDs.
- this number is derived from the fact that humans can hear frequencies between 20 Hz and 20 kHz.

If the sample rate is too low, then latency goes up accordingly.

# E Resources
- https://www.izotope.com/en/learn/digital-audio-basics-sample-rate-and-bit-depth.html
- https://hub.yamaha.com/proaudio/recording/what-is-an-audio-interface/
