
## CPU usage and Realtime process vs Non-realtime process
Consider that we can render a track to disk in less time than the duration of the track itself, while at the same time having audio issues that cause the playback to be choppy
- this is because writing to disk is a non-realtime operation, while playing back audio is a realtime operation.
- therefore, if you are able to render a track faster than the duration, then your playback issues are probably not due to CPU limits
    - this can be verified by checking ActivityMonitor to see how much CPU the DAW is taking up.

Consider recording in a DAW vs a process like video editing or spreadsheet editing.
- in a DAW, the CPU continually takes in WAV data from an audio interface (or MIDI) and plays it back through studio monitors, writes to memory, and also plays back the tracks that already exist in the song. If this process takes >100ms, it will be noticeable.
- in a video editor, our input to the program is to make edits. The nature of this is that our workflow is a cycle of making some edits, then playing it back. 100ms is too short a period of time to notice it in this workflow. 

### How audio gets from the DAW to studio monitors
The DAW provides a continuous stream of digital audio data 
- this data is transferred in chunks of data at a time, called the *buffer size* (set as an audio interface parameter)

the buffer size is related to the responsiveness of the system, because once the audio is moved into the buffer, it times time to do the conversion  
- spec: therefore, the amount time the audio files take to be converted to an analog signal serves as a bottleneck
- because the DAW needs to respond quickly to this buffered audio data, the buffer size must be very small, and therefore refilled very often, because the DAW can only fill one buffer at a time.
    - therefore, decreasing buffer size increases the responsiveness of the system. However, a shorter buffer means that the other elements of the system must be correspondingly more efficient in order to ensure that the CPU isn't locked up for too long (recall that CPUs multitask and handle many different requests seemingly at the same time, but actually does so sequentially)
        - "other elements" here might consist of, video cards, audio interfaces, network interfaces (espectially wireless interfaces), USB controllers, disk controllers
            - often the problem lies in a video card or sound card, which is why installing new drivers is normally the first thing to do when a performance issue like this arises.
- by increasing the audio buffer size, we are essentially increasing the window of opportunity for the CPU to fill it.
    - therefore, if we are having pops and crackles that are caused by devices that deliver audio files to the computer, increasing the buffer size is essentially slowing down the train to give the CPU a chance deliver all of the expected audio data on time.

When a problem device (e.g. audio interface/driver) locks up the CPU, the DAW can't properly fill each buffer, the audio data has a gap in it, or worse, a garbled mess of random data. As the sound card receives this corrupted data, this is manifested as pops, clicks, crackles
- other times, the computer will just put everything on pause until the buffer is filled— in which case playback will produce a stutter.

![](/assets/images/2022-09-13-14-39-28.png)

spec: an audio buffer size can be measured in ms or mb.
- if my buffer is 200ms it means that it will

### Fixing problems related to crackling/popping
- check for latest drivers (note: the latest driver is not always the best for your system.)
- Ensure buffer size is not too small.
    - the more tracks in your project, the higher your buffer needs to be
- Ensure that sampling rate is not too high. (a sensible default on many systems is 44.1khZ)
    - if sample rate is higher, then buffer size needs to be correspondingly bigger.
- use a latency checker with the input devices, and see if anything pops out. If not, then it might indicate a problem with the DAW. Check for updates.
- disable input devices (ie. video cards, audio interfaces, network interfaces etc.) one by one and determine if problem is resolved.

Latency = Buffer size / Sample rate

## Latency
Low rates of latency are not essential when mixing
- increasing latency can free up CPU, enabling you to run more tracks and more plugins in real time.


* * *

## Questions
- why is buffer size in Reaper measured in ms?

## E Resources
- [Realtime vs non-realtime processes](https://www.youtube.com/watch?v=GUsLLEkswzE)