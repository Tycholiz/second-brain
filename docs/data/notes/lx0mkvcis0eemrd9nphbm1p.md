
Remember that apparent volume is what matters, not dB. The shape of the soundwave also affects how loudly we perceive something
- even at the same dB level, a chainsaw will sound much louder than a flute because of the shape of the soundwave.

Once an instrument playing a certain pattern is heard, it is safe to blend back into the mix, where even if it is barely audible, the listener will be able to clearly discern what is being played, due to the fact they've already heard it.
- ex. a common pattern for a song has a guitar playing solo, only to be joined by other instruments progressively. Once these other instruments get added, it's fine to lower the volume on the guitar, since its distinctive pattern has already been heard and the listener can fill in the blanks on their own.

It is not uncommon for the engineer to vary the volume faders throughout the song as dynamics change (ex. instruments are added, entering a new section of the song etc.)
- [[compressors|music.engineering.mixing.compressor]] can only do so much before they start sounding unnatural.

The volume fader is the volume of the track after the FX pipeline has been applied to it. 
- It is the volume level that will be piped into the it's `send` (ie. the next place in the pipeline)

### Volume as a measure of depth control
Conceptually, in a 3D space, a higher volume would indicate that the sound is closer to us. But if we want a sound to be perceived as closer to the listener, the solution is not always as simple as increasing the volume. There are 2 things to understand with this:
1. Different frequencies decay through space at different rates, meaning that as you move closer to or further from a sound, the relative levels of different frequencies will change.
  - higher frequencies decay at a faster rate, which is why when a distant sound first approaches you, you may find that you hear only the bass frequencies at first, followed by the rest of the sound (or vice versa, depending on the physical environment)
2. The clarity of a sound deteriorates with distance. The further away a sound is, the more muffled it appears.

For these reasons, we need some other tools (together along with volume) to create the illusion of depth, such as [[compression|music.engineering.mixing.compressor]]

### Relative volume
When doing your initial volume setting of each track, it's easier to scope small and gently expand outward
- ex. volume-match your cellos first, then your string section, then your brass section, then your string section AND brass section, and so on.

## Volume balancing
Volume balancing should be the first step of any mix.

Can use a strategy of *height order*, where we loop the loudest part of the sound (with likely the most instruments playing simultaneously)
1. Turn everything all the way down
2. Choose which instrument is the most important (e.g. kick, snare, vocal etc), and bring it up to -5dB
3. Next, bring up the next most important element and balance it with that first most important instrument
4. Continue this process until everything is balanced around that single most important instrument

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

## Strategy for volume level setting
A good way of achieving good balance of volume is to put your volume very low and walk into the next room. Get to a point where you can barely hear the sound. The element that pops out the most is too loud and should be brought down 

* * *

The biggest game changer for me was when I realized how important the volume sliders on each track are and developing a good strategy for how to use them. My goal when mixing is to let everything have its turn. I do this by imagining you only get to hear one thing at a time. If a drum is struck, its attack should be louder than anything else and it is the only thing that needs to be heard. But luckily there’s lots of space between drums because they are percussion instruments. As soon as the transient attack decays from its peak I don’t need to hear it anymore, and now there’s all this wonderful open space inbetween each drum hit where I no longer need to hear the drum and am free to hear something else: but again, I only get to pick one thing to hear at a time in these spaces between the drums. Using this idea I try to set my levels loudest on the tracks that have the highest transients and lowest for the things that have the slowest decays.

So for example let’s say I have the following tracks: a drone synth pad, some guitars, bass, vocals, and drums. First thing to do is pull down all your faders so everything is silent. Then I’ll start by bringing up the synth pads first because they are long passages of relatively equal volume that don’t change a whole lot. They are the least dynamic of all the tracks. I bring them up to a decent level but not too high because everything else needs to go on top of them. Maybe about halfway. Next I’ll pull up the bass guitar because it has more dynamic attack than the pads but still lots of sustain (second-least dynamic of my tracks, so I address it second). My goal here is to bring the volume of the bass up so that when I watch the meters, the attack of the bass string being struck pops up above the volume of the synth pads. So long as that attack on the bass is louder than the pads, then I know I’ll hear the bass in my mix, even if the sustain drops below the pads afterward.

In essence what we’ve got now is kind of like a rolling fog of synth pads with mountain peaks of bass transients popping up through that fog. I’ve made space for both now. When the bass is plucked I hear it (and not the synth pad) but when it decays below that fog I hear the synth (inbetween the peaks of bass note attack). By doing this I’ve made dynamic space for both in the temporal plane. It’s like eq for time instead of frequency! Everybody knows you should  use eq to carve space in the frequency domain. But it took me forever to realize I need to use volume dynamics to carve space out of time! How did I not see that sooner???

So next I’ll do the same for guitars. They’re generally similar in volume to the bass, but with a bit more transient attack. I also use wide panning on the guitars so their peaks can be heard above the fog in the L/R space whereas the bass peaks pop up down the centre. But yeah, I want their peaks just above the bass, but doesn’t need to be by much for the reasons I just mentioned.

Next is the vocals. Consonants and plosives are even more dynamic than guitars, bass or pads. So my goal is to get the vocal transients to pop up above the cloud cover of everything else so far. I raise the fader on my vocals until the volume peaks crest the summed volume of everything else set so far. It can be handy to temporarily group or route your synth, bass and guitars to one bus so that you can watch their summed volume meter next to the vocal track meter to ensure the vocal peaks crest everything else.

And lastly, drums are the most dynamic with super fast attack and decay. So I set them loudest so they peak above everything else.

If I’ve successfully done my job here, when a drum is hit I hear the drum and then it quickly gets out of the way with a fast decay to make space. And in that space between drum hits, a vocal consonant pops up and is heard above all else and then gets out of the way for other things to be heard. And in the spaces between drum hits and vocal consonants, the pluck of a guitar string rises above everything else and then gets out of the way. And now in the space between drum hits, consonants and plucked guitars, a bass note rises above and then drops away… to reveal the synth pad that is droning along in all the remaining spaces between and under everything else.

The idea here is that you don’t actually get to hear everything at the same time. If everything was hard compressed and set to equal volumes you’d just hear a long muddy wash of all tracks playing at once. Unless that’s what you’re specifically going for that’s generally not what you want. It’s boring to listen to because it isn’t changing. But if your brain hears a drum and then a word and then a guitar chord and then a bass note and then a synth pad… one at a time in quick succession… it gets excited!!!! There’s a lot of different things happening quickly over time for it to process… instead of everything happening at once all the time without any change in focus.

Now since music generally has a rhythmic component you may wonder how this can work when all tracks play on the same beat? Well, it still works because we ordered it so that the quickest decay is loudest. In this case you hear the drum on the beat first because it’s loudest. But it dies away so quickly (fast decay) that it drops out to reveal the consonant of the vocal milliseconds later. It should decay fast enough that you don’t miss hearing most of the consonant! But then the consonant drops off too and you hear that guitar chord coming through now… and you may only be getting that last bit of the guitar strum attack but it’s enough. And as that last bit of the guitar attack decays it reveals the bass underneath. And maybe you missed hearing most or even all of the actual bass attack underneath everything else but that warm early sustain now shines through and is like syrup after the percussive attack of everything else, and as it dies away, it reveals below everything else our ever-present synth pad holding it all together. At this point you for sure missed hearing the attack of the synth but it doesn’t matter because it barely has any attack to speak of anyway. So yeah, that’s why it’s important to set your levels so the meters peak loudest on the fastest, most dynamic tracks. Because even if every track plays each note at the exact same time this strategy allows each layer to peel away and reveal the track underneath.

Once I started thinking about things this way I realized I could get 80% of the way there with just the faders and nothing else. Which is crazy because I saw them as second-class citizens to the jobs of eqs and compressors and reverbs and panning for so long. But they are SO critical despite their bare simplicity!!! I’m self-trained so maybe I’m an idiot for not having understood this sooner and everyone else already knew all this. But man, the simplest of things had the greatest effect.

Furthermore, once you understand the “only one thing at a time” paradigm you realize the other tools are just more granular versions for achieving the same thing. For example: are all your tracks too dynamic? If they’re all super percussive then there’s not enough time to reveal those layers beneath. So what do you do? Well, that’s the compressor’s time to shine! Throw lots of compression on your synth, slightly less compression on your bass, a little less on your guitars, almost none on your vocals, and none at all on your drums, and now suddenly you’ve got a good range of low vs high dynamic tracks so that the layers can be peeled back to reveal everything beneath just like we want. Obviously there are so many more applications for compressors than just this, but prior to my thought that you should only be “hearing just one thing at a time” I never would have thought to use them in this application. Reverb is a good way to reduce dynamics too, but it can offer a pleasing stereo spatial component too. So it’s kind of like a “blurry” compressor if you think about it. Again… perhaps an oversimplification but not something I would have considered prior to understanding this paradigm! And I realized side-chaining is sometimes so effective because it’s just brute-forcing the “one thing at a time” concept to the extreme!

But yeah, seriously. It’s ALL about volume and only having one loudest thing at a time. Once I got that, everything else just got better. And at the end of the day, I could still compress the hell out of the master to sound “loud enough”, but so long as I first gave everything it’s “time to shine” as the loudest part in the mix, then it still sounds relatively ok. Even if you have to brick wall the whole track because the client wants it “louder” and all the dynamics are lost (not great but sometimes that’s what they want), the clarity still remains intact in the temporal domain because you made sure only one primary thing needed to be heard at a time.

Anyway, sorry that was so long. But just felt like if somebody had explained this to me at the outset I would have saved myself so many years of grief and confusion. So yeah, I hope at the very least that I can save somebody else from some of that misery.

Lastly- I should say that if it sounds good you’re doing it right. This is as much art as it is science. Use the advice that works for you and drop the stuff that doesn’t. Don’t use my advice here if it does nothing for what you’re trying to accomplish. My word is certainly not law, and neither is anyone else’s. There’s a million ways to make this work. Find the ways that work best for you!

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

Mathematically, we derive the RMS by taking the average value (ie. mean), squaring it, then taking the square root.
- we do this process of squaring then taking square root so that the resultant value is always positive.

### LUFS (Loudness Unit Full Scale)
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

