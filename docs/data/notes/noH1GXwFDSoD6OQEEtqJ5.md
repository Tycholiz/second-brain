
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