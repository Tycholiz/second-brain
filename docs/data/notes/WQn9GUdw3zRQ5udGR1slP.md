
# Config
We use ReaPack for extension management
1. find the package in browse list, or import the xml
2. highlight the package
3. click ...Actions > Install

We use SWS for added functionality for REAPER

All config files stored in `~/Library/Application Support/REAPER`

# Actions
- Custom actions are similar to macros, in that we can take building block actions (like select, copy and paste) and run them in a sequence.
- The common definition of an action in Reaper is any input you make, for example, if I click on a MIDI item to select it, that is an action; if I select the next track, that is an action.

# Tips
- Cmd + B pulls up the project bay, where you can see the file path for all audio files in the project, and copy/move them to the project folder if they're all over the place.

### Record Monitoring
- Monitoring refers to whether or not REAPER plays back the incoming signal when a track is record armed

* * *

### Bus
Buses are great because they allow you to apply processing to multiple signals at once. 
- ex. maybe you want to apply some subtle saturation to your master bus to sweeten up your entire mix without applying a saturator to each track

You can create custom buses that contain similar instruments. Perhaps you want to create a vocal bus that contains all of the vocal melodies, harmonies, and ad libs in your song. Grouping or "busing" together sounds in this way reduces redundant processing.

Instead of applying a low-cut filter to every vocal track to remove low-end rumble, applying a single low-cut filter to your vocal bus will have the same affect and reduce the load on your computer's CPU.
- Try experimenting with bus compression, reverb, and delay.

### Send (maybe an Aux?)
A send is similar to a bus in the sense that it is for more efficient processing of an FX onto a certain type of sound
- ex. if we want an artistic reverb FX to be applied to both rhythm acoustic guitars, we could create a `Send: rhythm acoustic verb` and route the `Bus: acoustic rhythm` through it. Because the `Bus: acoustic rhythm` is also routed to the `Bus: Guitars`, we can mix the FX 100% on the send. As a result, we have a dedicated `Send` whose volume fader controls how much of the FX will be mixed in with the dry guitar signal itself.
    - this is what's referred to as parallel processing