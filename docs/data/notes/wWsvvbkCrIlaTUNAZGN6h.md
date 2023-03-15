
# Zoom
- `e` - zoom time selection
- `cmd`+`+`/`-` - zoom horizontally
- `cmd`+`shift`+`+`/`-` - zoom vertically
- `cmd+scroll up/down` - resize track height

# Main
- `cmd`+`p` - clear all peaked meters (clipping that occurs when sound too loud)
- `opt`+`s` - toggle snap to grid
- go to start - `w`
- to use box selection with mouse, hold ctrl
- navigate by region - `opt+1/2/3..`
- Jump to... - `cmd+j`
    - time - ex. 1:30
    - marker - ex. m4
    - region - ex. r2

# Midi Roll
- `\` and `~` - toggle between note types: straight and triplet
- `cmd`+`[`/`]` - increase/decrease granularity of grid.
- join 2 midi notes - `j`
- insert note - `i`
- move to next/prev of same note - `option`+`←`/`→`

# Tracks
- Delete `d`
- Open FX `f`
- Record - `r`
- solo - `<C-s>`
- toggle metronome - `c`
- toggle metronome count-in - `C`

# Media Item
Move item to track above/below - `<cmd + up/down>`
- hold shift to move midi notes an octave
- glue items - `g`

## Takes
- cycle takes - `t`/`T`
- delete active take - `D`
- confirm the active take, deleting the rest - `y`

# To be created:
- For comping from multiple takes, I have some custom key-assignments that speed up my workflow. I use "4" to colour selected take green, "5" to colour it red. So, say if I have 10 takes, I'll slice them line by line, or syllable by syllable, then colour the "possible contenders" green. From there I narrow it down. I use "r" key for previous take and "t" key for next take. I have "1" set to go to start of loop. In this way I can comp vocals super fast without looking at the keyboard, as my left hand has all the relevent keys within reach. I also use "v" for reduce current take volume by 1db, and "b" to increase current take by 1 dB, for evening out levels quickly without automation.
- custom action: Transport: Stop... Go to beginning of loop... Delete active take... Transport: Record. So if I'm recording myself, I can use just one key to immediately start the take again from the top, without dropping he guitar to use the mouse and multiple keystrokes.
- Midi: delete all events to the right of the currently selected one

# Tips
- there is an action "Misc: pass through key to main window" which can be a useful utility for creating multistep custom actions.
    - ex. "record when midi window open" can be crafted by sending a record command that can be sent to the main window