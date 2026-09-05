
### Install extensions
Simply drag the `.dylib` file into `~/Library/Application Support/REAPER/UserPlugins`

## Recording
### Loop recording with pre-roll each time
This will allow us to loop record while being able to hear the part that comes before the actual section to be recorded *on each iteration of the loop*
- [source](https://reaperblog.net/2021/08/loop-rec-pre-roll/#:~:text=Pre%2DRoll%20is%20when%20you,looping%20there%27s%20no%20pre%2Droll.)

1. Disable options > Loop points linked to time selection
2. Record mode > time selection auto punch
3. Enable options > new recording that overlaps existing media items > splits items and creates new takes
  - already enabled by default
4. Set monitoring mode of the track to *Monitor input (Tape auto style)* (so we don't hear the previous take during the pre-roll)
5. Drag in a ruler for the whole section including the pre-roll
6. Create a time selection in the area you want to record into
7. Metronome settings - *count-in* turned off, *pre-roll before recording* turned off

### Render MIDI: Record the output of one track to another
Imagine we have a MIDI track with some VSTi plugin (origin track), and want to get the soundwaves of that output onto a new track (destination track).

1. On the destination track, enable:
  - *Monitor Input*
  - *Record Output* > *Record Output (stereo)*
  - *Record Output* > *Output mode: post-fader*
2. On the destination track, add the origin track(s) as a *receives*
3. Record

### Use computer keyboard as MIDI controller
1. Enable Input Monitoring on the track
2. Input: MIDI: Virtual MIDI Keyboard > All channels
3. View > Virtual MIDI Keyboard (`opt+b`)
4. Arm track for recording

### Record output from Mac to a track in Reaper
Useful for instance if we find a Sitar drone track on Youtube that you want to insert as a track into the project

- https://www.youtube.com/watch?v=BzIwPV1b8M8

### Automation for media item
In the FX, hit `param` > `show media item take envelope`

## Editing
### Side-chain compression
- see [[side-chain compression Dendron note|music.engineering.mixing.compressor.techniques#sidechain-compression]]

example use-case: vocals cause the guitar to duck

1. on the track we want to compress (guitar), open routing
2. specify 4 track channels 
  - if you also want, say, a violin lead track to compress the guitar, then add 2 more channels
3. set a new receive from the track that will trigger the compression (lead vocal track)
  - this receive should be post-fader
  - it should receive the vocal signal to channels 3 and 4 of our compressed track (guitar)
4. add the compressor onto the compressed track (guitar)
  - open Plug-in pin connector and ensure Main Inputs are set to Channel 1 and Channel 2 (left and right, respectively), and that Left and Right Auxiliary inputs are set to the Receives from Channels 3 and 4, respectively. Compressed Output 1 should be Channel 1 and Compressed output 2 should be Channel 2. These settings are default.
5. In our compression plugin, set it to be triggered by the auxiliary input
  - in ReaComp, find the *detector input* dropdown and select *Auxiliary inputs*
  
### Check if sound is mono or stereo
Even though a media item may have 2 channels, it may not actually be stereo. We can check this by reversing the polarity of one of the channels, and panning both channels to center. If it's actually a mono sound, we won't hear anything, due to [[phase cancellation|music.engineering.recording#phasing]].
- use plugin *JS: Stereo Channel Volume/Pan/Polarity*

### Melodyne multiple tracks linked together
In Melodyne in Reaper, sometimes we'll have 2 different tracks that sing the same melody. By default, Reaper may link these 2 together, so that editing a blob in Vox1 will cause the corresponding blob in Vox2 to move in lockstep. Follow these steps to disable that behaviour:

1. Options -> Preferences -> Plugins -> ARA
by default" is TURNED OFF. This will fix the blobs of the other track with Melodyne
Make sure that the option "Pool ARA edits for all copies of the same source media
from following another instance whenever it also has another Melodyne ARA vst
running.

2. In Melodyne, Options -> Follow Selection in DAW. I've turned this off as well. Not
100% sure if the first one is enough to fix it but I've just turned this off along
with the other one and works just perfectly for me.

## MIDI learn TouchOSC XY axis
The problem: MIDI learn functionality within VST settings detects knob presses, but face problems when a single knob controls 2 different parameters (e.g. XY axis that controls vibrato and expression levels of a violin, soundthing found in Embertone TouchOSC apps)

To properly MIDI learn one of these (X or Y) at a time:
1. With MidiView, identify which CC# is being used in the XY axis (identify which is which by looking at the velocity levels. Finger at 0, 127, and then finger at 127, 0).
2. temporarily assign one of the knobs in the TouchOSC interface to that CC#
    1. TouchOSC Edit View
    2. Touch temporary knob
    3. In side window that pops up, go to Messages > Controller
    4. Change value to the CC#
3. In VST, MIDI learn on the desired parameter
4. In TouchOSC, adjust level of the temporary knob

The parameter in the VST should be mapped to the desired X/Y value in the axis, since the temporary knob CC# controls the same parameter as the desired X/Y value in the axis