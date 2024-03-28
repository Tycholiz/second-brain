
A microphone converts sound waves into electrical waves

Consider the [[Inverse Square law|music.acoustics#inverse-square-law-of-sound]]

note: `on-axis` refers to "where the microphone is pointing"

## Dynamic vs Condenser Microphones
### Dynamic Microphone
Better for capturing loud, strong sounds, especially in a live setting
- ex. drums, guitar amps, loud vocals

Dynamic microphones are older, and thus most primitive in terms of design

### Condenser Microphone
Better for capturing more delicate sounds and higher frequencies, especially in a studio setting.

Needs electricity to function (between 9V-48V), which can be supplied either via batteries in the microphone itself or *phantom power*
- phantom power usually comes from an audio interface or pre-amp, and the switch would be labelled as `+48v`

## Microphone Polar Patterns
A microphone’s polar pattern is the 3-dimensional space surrounding the capsule where it is MOST sensitive to sound.
- this "sensitive area" is known as the *acceptance angle*, and can be defined as the angle before sensitivity drops by 3dB. 

![microphone polar patterns](/assets/images/2022-10-13-08-55-07.png)

### Omnidirectional
equally sensitive to sound from all directions.

Good for overhead (OH) mics on drumkits

### Bidirectional (Figure-8)
very sensitive to sound from the front and rear, but almost completely deaf on the sides.

### Cardioid
Cardioid mics have a wide acceptance angle of about 180°
- the signal strength drops only by 6dB on either side of the on-axis line.

The goal of a cardioid mic is to record the sound of what it's pointed at and ignore everything else, making it useful especially for
- miking up drumkits
- live performances
- untreated rooms

The downsides of a cardioid microphone is:
- there is a noticeable drop in high-frequency sensitivity as you move further away from where the microphone is pointing.
- *proximity effect*, whereby the bass freqencies are boosted when the sound source is too close to the microphone.

"Generally speaking, cardioid and hypercardioid will perform better in reverberant spaces than shotguns or omnis"

Cardioid is a combination of omnidirectional and bidirectional
- sound signals coming from the front (on-axis) are 2x as strong
- sound signals coming from the side are the same as omnidirectional (1x)
- sound signals coming from the rear are cancelled out 

![](/assets/images/2022-10-13-09-00-04.png)

### Supercardioid
Supercardioid mics have a tighter acceptance angle than cardioids (about 150° compared to 180°)
- supercardioid mics are great choices for isolating individual sound sources.

Supercardioid mics are sensitive to vocal plosives (e.g. pops) and wind noise

Supercardioids are good microphones for close-miking in loud environments

![](/assets/images/2022-10-13-09-19-58.png)