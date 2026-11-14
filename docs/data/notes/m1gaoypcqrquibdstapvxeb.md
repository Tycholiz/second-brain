
A microphone converts sound waves into electrical waves
- therefore, it is an example of a transducer (a device which changes energy from one form into another; in this case acoustic into electrical)

There are 3 main considerations when choosing a microphone:
- operating principle (ie. dynamic vs condenser)
- frequency response - The variation in output level or sensitivity of a microphone over its useable range from lowest to highest frequency
    - A microphone whose response is equal at all frequencies is said to have a “flat” frequency response. These microphones typically have a wide frequency range. Flat response microphones tend to be used to reproduce sound sources without coloring the original source (desirable in instruments such as acoustic guitar/piano)
- directionality - The sensitivity to sound relative to the direction or angle of arrival at the microphone.

![](/assets/images/2025-05-07-11-30-05.png)

Consider the [[Inverse Square law|music.acoustics#inverse-square-law-of-sound]]

note: `on-axis` refers to "where the microphone is pointing"

For most unidirectional types, bass response increases as the microphone is moved closer to the sound source.

Most acoustic instruments are designed to sound best at a distance (say, two or more feet away).

## Dynamic vs Condenser Microphone
A good way to understand why dynamic and condenser mics sound different is to understand the differences in their transient response.
- In order for a microphone to convert sound energy into electrical energy, the sound wave must physically move the diaphragm of the microphone. Because the diaphragm of a dynamic microphone may have up to 1000x the mass of the diaphragm of a condenser microphone, it starts moving much more slowly.
    - anal: a truck and a sports car in traffic. They may have engines of equal power, but the truck weighs much more than the car.  As traffic flow changes, the sports car can accelerate and brake very quickly, while the semi accelerates and brakes very slowly due to its greater weight. Both vehicles follow the overall traffic flow but the sports car responds better to sudden changes.
- Since condenser microphones generally have better transient response then dynamics, they are better suited for instruments that have very sharp attacks or extended high frequency output such as cymbals. It is this transient response difference that causes condenser mics to have a more crisp, detailed sound and dynamic mics to have a more mellow, rounded sound.

![](/assets/images/2025-05-07-11-49-58.png)

As we can see from the picture above, it is evident that it takes almost twice as long for the dynamic microphone to respond to the sound. It also takes longer for the dynamic to stop moving after the impulse has passed (notice the ripple on the second half of the graph).

### Dynamic Microphone 
Better for capturing loud, strong sounds, especially in a live setting
- ex. drums, guitar amps, loud vocals

Dynamic microphones are older, and thus most primitive in terms of design

The dynamic has some limitations at extreme high and low frequencies.

#### Ribbon Microphone
Ribbon microphones are a variation of the dynamic microphone

Ribbon microphones are typically bidirectional, meaning that they pick up sounds equally well from either side of the microphone.

Ribbon microphones are highly regarded in studio recording for their “warmth” and good low frequency response. 

### Condenser Microphone
Better for capturing more delicate sounds and higher frequencies, especially in a studio setting.

The main limitations of a condenser microphone relate to its electronics. These circuits can handle a specified maximum signal level from the condenser element, so a condenser mic has a maximum sound level before its output starts to be distorted.
- note: the microphone will not be damaged by excess level.

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