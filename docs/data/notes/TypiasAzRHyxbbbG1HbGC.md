
### How to set up MIDI instrument track
1. insert > virtual instrument on new track...
2. confirm the routing confirmation (for instruments where you want granular control, like drums)
3. insert > new MIDI item
4. double click on the track

### Load in third party virtual instrument to Kontakt
- In Reaper, make a new virtual instrument with Kontakt
- Click the file tab, and find the `.nki` file for the virtual instrument (we store these in the external hard drive in `SingleSamples/`)
- Add them to the quick-load for easier access, but otherwise just double click the `.nki` file.

### Quantization
Quantization range
- `from` - indicates how aggressive the quantization should be for tracks far off time. The lower the %, the more "perfect" the quantization will be. As the % gets higher, the quantization algorithm cares less and less about tracks that are only slightly off time, and will focus on bringing into line the real offenders.

### MIDI recording modes
- *Record MIDI overdub* - adds new MIDI events without replacing the ones that were already there
- *Record MIDI replace* - replaces all MIDI notes from the time you start recording
- *Record MIDI touch-replace* - existing notes will be replaced by any new notes played over them. All other existing material will remain as is.
- *Record MIDI latch-replace* - existing notes remain unchanged until you strike the first note, at which point all further notes will replaced.
- note: don't forget you can still use *Record Input* (the same recording mode as you do with real instruments), for example if you want to generate takes so you can comp them.

* * *

## Tips for playing virtual instruments
Some instrument families tend to have their note a bit delayed from the moment the note is hit. Brass for example has a noticable delay between when the player starts to blow and sound actually comes out of the instrument. Therefore quantization will not work well automatically in these cases. What you need to do is:
1. record the midi part, playing by ear
2. zoom in and gauge where the note is in relation to the official start of the bar. Does it appear before the start? Take note of its position
3. record the full midi section on the midi keyboard
4. quantize the notes
5. select all notes (`cmd+a`) and adjust them to the correct position.