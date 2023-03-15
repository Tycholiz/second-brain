
displacement is how far the molecule was moved from its initial spot. This concept is what gives us our amplitude (loudness) 

## How sound travels
- Sounds are brought to our ears by air. When an object (ex. guitar string) moves, it disturbs the air around it. More specifically, it disrupts the natural motion of air molecules near the object. Those disturbed molecules in turn disturb their neighbors, and so on, in a ripple effect.
- The disturbance of these air molecules forms a pattern that permeates in all direction outward. This pattern effectively becomes an entity itself, which we call a soundwave. 
- Consider at a stadium when fans do *The Wave*. Each person effectively influences the movement of the person beside them, and so on down the line. In effect, that wave has become its own entity. This is the sound wave.
- If the movement of an object (guitar string) is rapid and regular (ie. consistent), then regular soundwaves will be produced. This is the type of sound that produces tones (a sound with a particular pitch). We associate this type of sound with music.
    - note: tone here is used in a physics sense. 
## Noise vs Tone
- Imagine taking a handful of stones and dropping them into a pond. Each would make its own wave, and those waves would go outward in all directions, crashing into the other waves and distrupting their natural path and canceling them out. This is analogous to noise, which is basically disorganized sound waves (or more simply, disorganized sound). 

![](/assets/images/2021-03-27-19-34-01.png)

## Timbre
- def - the characteristic difference in sound between instruments. 
- Timbre is created due to the unique combination of different level harmonics. 
    - ex. a clarinet might have relatively loud 3rd and 8th harmonics. This unique combination is what gives the clarinet its tone. 

## Why certain notes sound good together
- Say someone plays a note, a middle C. Now someone else plays the note that is twice the frequency of the middle C. Since this second note was already a harmonic of the first note, the sound waves of the two notes reinforce each other and sound good together. 
- These are the harmonics found in the A note:
```
A A E A C# E G A
1 2 3 4 5  6 7 8
```
* * *

- when a sound wave encounters a wall, it does one of 2 things:
    - It bounces (reflection)
    or
    - It bends (refraction)
- waves can be trapped by multiple objects facing each other, resulting in standing waves.
    - this is how musical instruments achieve pitch (how sharp or flat something is, in a relative sense) 
- When a musical tone is played, only a particular set of frequencies is heard. So when you play a note on a piano, what is heard is actually a blend of multiple pitches.
    - These pitches are called harmonics. They give the sound its timbre.

# Frequency
- all sound waves travel at about the same speed. This means that waves with a shorter wavelength (ie. higher pitch) will arrive at your ear more frequently.
- This aspect of sound (how often a wave gets to your ear) is called frequency.
- Musicians use the term *pitch*.

### Harmonic Frequencies
below: the red line represents a sine wave, whereas the superimposed black wave is a guitar. The guitar wave generally follows the sine wave, but there are bumps. The space between the black wave and the red one are the harmonic frequencies that are put out by the guitar.
![](/assets/images/2022-09-18-15-25-20.png)

It is the unique harmonic frequencies of each sound that give it its timbre.

below: the soundwave recorded with a microphone at the soundhole will produce a wave that is much more similar to the sine wave.
![](/assets/images/2022-09-18-15-30-39.png)

compare this to a microphone at the neck.

![](/assets/images/2022-09-18-15-32-20.png)

This is because the fundamental frequencies are accented over the soundhole, whereas the harmonic frequencies are accented over the neck.

The illustrates how playing an A on guitar and an A on a clarinet will produce the exact same fundamental— it is the harmonics that give each sound its unique timbre.

below: an A on guitar. Notice the fundamental frequency as the leftmost peak, while the others are harmonic frequencies.
- notice that they get closer together as we move higher up the frequency spectrum.
- also notice that past a certain point, harmonics start to become more faint.
![](/assets/images/2022-09-18-15-39-06.png)

A soundwave that has no harmonic, is a sine wave.
- therefore all harmonics are sine waves.

The first 6 harmonics (ie. fundmental+5 overtones) make up a major chord.

below: every harmonic note that isn't an octave of the fundamental is slightly out of tune.
- here "out of tune" is in the context of *equal temperament*, whereby an octave is split into 12 evenly spaced frequency ranges and each represented by a note. Acoustically, the 12 frequency ranges are not equal. Consider that we can describe relationships between tones with ratios (octave is 2:1, 4:3 is a 4th, a tritone is 45:32 etc.). Many of these ratios yield an irrational frequency number. This system of tuning is called *just intonation*.
    - spec: ex. Middle C is at ~260Hz. A perfect 4th (4:3) from C would be at 346.666Hz (260 * 4 / 3)

![](/assets/images/2022-09-18-16-06-39.png)

Naturally, if we were using the just intonation method of tuning, our notes would all be perfectly in tune.

### Equal Temperament
If we are tuning our guitar with a tuner, then our instrument is tuned according to *equal temperament*. If we are using harmonics to tune, then we are using *just intonation*. 

Notes in equal temperament aren't the most pleasing "versions" of those notes, but they will sound approximately right in any context.
- this is why if we make our open C chord perfectly in tune and then go play an E chord, it sounds out of tune.
- for this reason, it might be advisable to tune to concert pitch with a tuner, then make any fine adjustments needed to make the guitar sound good in whatever key you're playing in.

* * *

## Inverse Square Law of Sound
The inverse square law states that "with every doubling of distance away from the sound source, the sound will be four times less intense." 
- Consider that we can visualize sound as an expanding sphere, since it will extend out in all directions from the source. After a sound has been made, the same amount of energy will exist in that sphere no matter if we are close to the source (small sphere), or if we are further away (larger sphere). Therefore, the larger the sphere is, the more surface area the energy must be spread over, resulting in less energy at any single point.
- Also consider that when we double the radius of a sphere, the surface area quadruples. This means that when we move from 1m to 2m away from a sound source, the strength of the sound wave at any single point on the surface of the sphere is actually 1/4. Since our ears/microphones only pick up sound from a small portion of the entire surface area of the soundwave, this effectively means that the sound pressure level of that soundwave is 4x less as we double our distance from that sound source.

![](/assets/images/2022-10-14-09-13-02.png)


### Questions?
- is it that as there are overlapping harmonics in common between the two notes, the more consonant they sound together?

## Resources
- [Acoustic room treatment software](https://www.roomeqwizard.com/)
    - need 2 special kind of microphones explicitly for this purpose, which cost around $200 total

# Related
- [[science.sound]]
