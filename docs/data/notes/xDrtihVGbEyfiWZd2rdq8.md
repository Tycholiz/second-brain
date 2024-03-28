
Midi is a protocol

Stands for *musical instrument digital interface*

Midi events are the building blocks of a Midi part.
- with virtual drums, each hit is an event.
- each event carries information about the note: its velocity, its pitch, vibrato level, pan etc. 

A MIDI file essentially a giant list of events, and values for the events.

A single MIDI link through a MIDI cable can carry up to sixteen channels of information, each of which can be routed to a separate device or instrument

Every midi event has a value range of 0-127

When you first learn MIDI, you learn perhaps its most common application: playing virtual instruments. But it's helpful sooner or later to think of MIDI more as a simple protocol for sending messages. What these messages are? that's for the MIDI controller (physical or virtual) to determine.
- ex. a virtual drum kit might have a MIDI signal that equates to the drummer tightening the hi-hat pedal. This is not a "hit" of the drum per-se, but is rather a signal that informs the DAW that the pedal has now been depressed.

MIDI architecture imposes a limit of 16 channels per device.
- this restriction can be worked around by using a MIDI patch bay to allow multiple devices to be connected

You can theoretically use midi to control just about anything that requires events and values.
- you can control the light show at a concert with midi

### Omni on
- A device can be configured to only listen to specific channels and to ignore the messages sent on other channels ("Omni Off" mode), or it can listen to all channels, effectively ignoring the channel address ("Omni On")

### CC (Control Change)
Think of CC as a virtual knob with values of 0-127. Every Midi Channel has 128 CCs. Meaning for every channel, you can control 128 values, or "128 different knobs, sliders, switches."

CC is used to extend the range of functionality of a MIDI message.

Manufacturers of MIDI controllers assign unique CC numbers to each knob/encoder and are immutable.

- ex. a hardware synthesizer filter cutoff could be controlled using MIDI CC, without having to physically turn the knob. 
- ex. a Roland drumkit can be configured to give greater control over which part of the drum was hit.

### Plug-in pin connector
We have 2 parts: the input channel and the output channel

![](/assets/images/2022-04-05-11-31-49.png)
- When we use stereo, we need 2 channels, so the above image could correspond to one instrument. 

### Step recording
- This method of recording MIDI lets us enter midi notes, then automatically jump to the next column in the grid (of piano roll). Put another way, it is perfectly in time.
- ex. we have a 4/4 song and we define each step as a quarter note. We decide to record the kick drum, so we hit the midi key. That key press will be recorded, and then the position in the song will move to the next quarter note. Again if we hit the midi key, that will be recorded and the position of the cursor will move to the next quarter not
- Doing it in this way by nature will result in the sound being robotic, since it is perfect timing.
- The velocity is tracked when we hit the midi keys

### Quantize
- Quantizing is a concept that accomplishes the problem: how do we take our badly timed midi track and make the notes fit perfectly with the tempo?
- when we are laying down a midi track, we can quantize the notes so that they are perfectly aligned with the grid. This alignment will depend on how granular the grid currently is.
- we can decide which part of the note will line up to the grid
    - position (start of note), end of note, whole note length, and any
	combination of the preceding.
- We can also determine how close to the grid it will be with `Strength`. Using 100% will make it perfect, but this can detract from some of the expression
    that comes through the playing of a skilled musician.
- We can permit the notes to align to the grid on either side, which by default will be fully checked.

### Simulating Legato with stringed instruments
- ex. hammer on, pull off
- allow the first note to overlap the second note slightly. This will reduce the
    staccato nature of the guitar, and make it sound like a smoother transition.
- Another method is to use pitch bends, but don't make them smooth. Make the pitch bends quantized at semitones. It sounds realistic for slides/pull-offs/hammer-ons.
