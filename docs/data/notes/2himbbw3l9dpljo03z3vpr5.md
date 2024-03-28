
### Threshold
The threshold determines what is to be selected by the compressor (which would be everything louder than the threshold)

### Ratio
The ratio determines by how much we will squeeze down the selected parts

### Gain
The gain determines how much volume will be added back to *everything*

### Attack
Attack determines how quickly compression will kick in when the dB threshold has been met.

Think of attack as letting you shape the transient of a sound. Adding punch (slower attack) or removing punch (faster attack) as you adjust the attack time.
- ie. the compressor lets you control the size, speed, texture, tone of the transient.

Attack time is tweaked to manage the impact of transients but transients have almost nothing to do with our perception of loudness, which is a much slower impression than our impression of impact.

Attack is a way to control how punchy the sound is
- with a slower attack, we let more of the punchiness th

The slower the attack speed, the more of the transient we are letting through.
- this results in a more punchy sound. More focus is on the hits of the instrument
- generally speaking, slow attack is better for percussive sounds

The faster the attack speed, the less sound we are letting through on the initial burst
- this results in a more mellow sound. More focus is on what follows from the hits
- generally speaking, fast attack is better for more melodic parts

If you have a lead instrument in a dense mix, it can be a good idea to let some more attack through (longer attack time), since it allows us to follow the melody a little closer
- if we have a sparse mix, we may want to shorten the attack so that the transients don't poke through the layers.

tip: to hear what the attack is really doing to the sound, turn the volume of your mix to an almost imperceptible level. At this point, you should be able to hear changes you make to the attack setting.
- this is because our perceptual system acts like a natural compressor at high volumes

### Release
Release determines how quickly the compressor will recover from gain reduction.

Release lets us control the movement of the compression.

Fast releases can be perceived as brighter and more aggressive
- generally speaking, fast release is better for more percussive, punchy sounds

Slow releases make the sound darker and a little smoother, and make the compression feel more relaxed.
- https://youtu.be/K0XGXz6SHco?t=1034
- slow release times on a track with strong dynamics (e.g. lead vocals) can result in unwanted compression on quieter passages, resulting in an unwanted stuttering effect.
    - if we have too slow of a release time, then loud parts that trigger the compressor will take too long to recover, and will end up applying the gain reduction to the subsequent quiet parts, sort of defeating the purpose of the compressor.

Consider a compressor on a drum beat track with kick-snare-ride.
- With a fast release, each time the (louder) kick and snare were hit, the ride would duck very quickly, since the kick and snare are being grabbed by the compressor.
    - https://youtu.be/K0XGXz6SHco?t=750
- With a slow release, the ride takes some time to get back to its highest volume level again, after each time the kick and snare hits. This creates kind of a swell effect on the cymbals themselves.
    - https://youtu.be/K0XGXz6SHco?t=798

### Knee size
knee is about the interaction between a compressor’s threshold and ratio settings.

Knee size smooths the way the compressor reacts to the signal

Knee size determines whether the compressor kicks in suddenly or gently.
- a low setting (ie. Hard Knee) of 0dB ensures that the full compression ratio is applied the instant the threshold is exceeded.
- a high setting will result in the compression being applied more gradually.

Knee size blurs the line of the threshold
- ex. 3db knee size means that 3db under the threshold is where the compressor begins to react, increasingly towards the real threshold value. This causes the compressor to start reacting in small amounts early, so it is less obvious where it starts.

## Misc
If you don't know where to start, start with a high ratio so you can really hear the effects of what the attack and release are doing.

## Resources
- [Interactive compression soundwave visualizer](https://codepen.io/animalsnacks/full/VRweeb?fbclid=IwAR2CE0K03deuAOMT8Ccdy9-B80iJJJCjAyiYD3AeZUvYegZrY8arhx6JJfU)
- [visualization of how each compression param affects an audio signal](https://www.youtube.com/watch?v=4gNRGqHzMKc)

* * *

### Mom music analogy
- Threshold - The volume at which your mom tells you to cut down your music
- Ratio - The amount you cut down your music when she tells you to (the threshold)
- Attack - How FAST you cut it down when she tells you to (the threshold)
- Release - How quickly you cut the music back up when she leaves the room
