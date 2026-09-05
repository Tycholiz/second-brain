
# Parts of a DAW
## Types of Tracks
### Bus
- By default all sound gets routed to the master bus. What if you added a distortion plugin onto the master track? Every audio file would gain that distortion. What if we wanted to only apply distortion to the 3 electric guitars? We could output the 3 guitar tracks to a bus track, then apply the distortion plugin on that bus track. Then that bus track would output it's combined audio to the master track, mixing it with the rest of the tracks and buses. 
- This is useful for things like distortion/EQ/compression
- In actuality, the bus is simply the connection between origin and destination. You'd add effects to the channel that you assigned the bus to, rather than to the bus itself.
- buses are simply the connections between origins and destinations in a mixer
- Imagine you have a string section, then you set the levels so they sound good between them, and now you mix them as a chunk.
- In Reaper, a folder === bus

### Send
- Imagine we wanted to separate out the distorted part of the sound from the original sound?
- ex. We record a snare drum and add reverb to it. What if we wanted to mix the original snare sound and the reverb differently? If we sent the snare to a bus and mixed the bus, we would have effectively glued those two parts of the sound together, rendering us unable to mix them separately.
- A Send Track is similar to a bus track, with the difference being: the original snare sound is sent directly to the master, thereby bypassing the bus (and the effects it applies).
    - In reality, the original snare sound is sent along with the reverb to the send. In essence there are 2 copies of the snare.
    - A send is a split in the sound signal, so that it gets sent to 2 different places.

#### Types:
- each send is defined as one of 3 types:
    - Post-fader (post-pan)
        - default
    - Pre-fader (post-FX)
    - Pre-FX
- Different send types send the audio at different stages in the signal flow.
    - ex. the volume of a send that is Post-Fader (Post-Pan) will be affected by
changes made to the source track's volume fader. A `send` that is Pre-Fader (Post FX) will not. An audio `send` that is Pre-FX will be affected by the source track’s volume fader but not by any FX in the source track's FX chain

### FX Track
- an FX track outputs directly to the master, but it will take in inputs
- For instance, say we have a delay and reverb combination that we want to put into an FX track. Anything that routes to this FX track will now pick up that delay and reverb before going on to the master.

### VCA (Voltage control amplifier)
- a VCA track will have a volume fader, which is used as a controller for the volume levels on other tracks.
- ex. We assign guitar 1, 2, 3 to VCA1. So now when we reduce volume of VCA1, guitar 1, 2, 3 are also reduced in volume.
- VCA does not actually route the audio, as a bus does.

#### Usage
1. View > Grouping matrix
2. Select `show group details`
3. set your VCA track (named `VCA1` here) as MASTER (M)
4. set your slave tracks (S), causing their volume to be adjusted any time `VCA1` is adjusted.

![](/assets/images/2021-03-27-19-35-55.png)

## Routing (I/O)
- Sound files are read from the hard drive into Reaper, then will run through the tracks, and then be routed to the master.
- On each track's route button, there is a master send checkbox, meaning if selected, that track gets routed to the master (which is the default behaviour)
    - The master track itself will route to the hardware (audio interface)
![](/assets/images/2021-03-27-19-36-06.png)

## Mix Automation
- The most popular use of automation in mixing is to adjust the volume of a track. For example, it allows you to bring an instrument to the forefront for a moment and fade it back out when the lead vocal comes back in
    - Think Band on the Run, during the 3rd part when acoustic is front and center at first, but lowers in volume as the other instruments enter. 
- Examples:
    - Automate an effect bypass on and off in certain sections of your song. This could be super useful if you want to create a delay or a long reverb tail only on a couple specific words to help emphasize them.
    - Automate individual plugin parameters. This can be particularly handy when creating EQ filter sweeps, or when you want to alter the delay feedback amount in a section of your song.
    - Automate a VCA or a bus to control the level of a group of instruments at once.
    - Automate the master fader to create a fade out for the end of your song. 
- Use automation any time you want to adjust a parameter on any track or in any plug-in in your song.

### Automation modes
- Automation modes determine how automation is treated on a particular track.
- Automation can either be read or written
Types:
- Read - When we are playing the track, the DAW plays back all the automation on
    the track. This is the most basic, and considered to be default.
    - if we've set up automation to automatically adjust the volume at a certain
        part of the song, the volume fader will move automatically.
    - if we move any knobs, it will not write anything to the track. It will
        merely be temporary.
- Touch - When we are playing the track, the DAW plays back all the automation on
    the track. The difference is, that if we move the knob while it's playing
    back, we will adjust the automation on the fly.
    - When we release the knob, the changes stop.
    - This mode is useful if you only want to touch up (thus the name Touch) certain portions of your automation without affecting the rest.
- Latch - like `Touch`, but when we release the knob, it will stay where it is.

![](/assets/images/2021-03-27-19-36-23.png)

# Comping
- def - taking multiple tracks of the same part of a song, and slicing in the
    best parts of each.

## Slice and Dice
- When we have recorded the same thing multiple times, we have our lanes as a result. Our strategy is to split each take into phases, which roughly correspond to distinct sound waves.
- Doing this, we can choose the best pieces, not only in raw performance, but also in the context of the other best guitar parts.
    - first we choose the best 1st phrase, then the best 2nd phrase (while still playing back the 1st), then the best 3rd phrase (while still playing back the 1st and 2nd), and so on.

![](/assets/images/2021-03-27-19-36-35.png)

- Each combination of these phrases is called a comp.

## Comping tips
- It's easier to comp a part that has been worked on in sections, because the singer's vocal tone will be more consistent between the takes

# Features
- Solo in Front - same as solo, except it just lowers the volume of everything else, instead of muting it
    - found in `actions`

# Tips
- apply soft compression to glue everything together

# Gain vs Volume
- volume is the master level of output that a track will give out. It is the raw sound that comes out. In other words, it is after processing.
    -  It’s the volume level being sent into your plugins, preamps, and amplifiers.
- gain is the volume level of a signal before processing.
    - How loud something is AFTER processing doesn’t change the tone of the sound. But how loud something is BEFORE processing definitely will.
- changing the volume knob will change perceived loudness, and that's it. changing the gain will cause a literal difference in the sound.

# Resources
- [free kontakt libraries](https://www.flstudiomusic.com/2017/03/38-best-free-kontakt-libraries.html)

# UE Resources
- [Blog posts for understanding mixing concepts](https://www.izotope.com/en/learn.html)
- https://heroic.academy/essential-guide-becoming-music-mixing-professional-part-2-signal-flow-plugins/
- [How to comp](https://www.soundonsound.com/techniques/vocal-comping)


# Questions 
- what is a channel?
    - a channel is an audio signal, while a track is the place where that signal can be read/written.
    - channels appear on the mixer, while tracks appear on the "canvas"
    - channel represents the instantaneous path for a signal
    - The track is like the read/write part of the program, while the channel is the route that the signal takes, while it is on its way to being written into the track.
- When you mix a track, what is the high level? Are we getting raw sound from the microphone, then taking that output, passing it through a channel which gets put on a track, which gets routed to another channel on a mixer? 
- how do sends and receives work in the context of midi? is a send/receive for sending or receiving midi signals? for instance, can I have a midi track that sends to a reverb bus (ie that bus receives it) ?
- Why use a VCA track when you can just use folders (buses) to control the overall volume?
- Can we use channels in midi in order to apply "effects" to a certain group of notes?
    - I want to somehow apply effects once and have it affect all notes of a "type", like the softer snare hits in the Hagia Sofia intro.
