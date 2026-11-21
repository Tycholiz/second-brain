
a.k.a Block Size

Generally lower buffer size reduces latency but increases CPU load. Higher buffer size increases latency and decreases CPU load.
- The reason to adjust the buffer size is to switch between these states.
- If you are recording and monitoring the recording from the DAW you want as low of a buffer size you can get without causing your computer to crash or stutter audio playback. If you are editing and mixing with lots of plugins that use CPU resources you may want to increase the buffer size to allow more resources to be allocated to the plugins instead of the audio playback.

### Analogy
A buffer is like a conveyor belt. There is a robot that takes bits out and moves it to the next machine. The longer it is, the longer it takes for the audio data to move to the processor, but if it is too short, then there might be no more room to put additional bits in, and we have to throw it to trash. This is buffer overflow, when the processor can't keep up, we get crackles and gaps in data.
- Therefore, we want as low buffer as possible without creating crackles and pops in the audio.

### Preferences > Device > Request Block Size
This is the interface buffer size.
- This will set the latency for any live inputs and outputs, whether audio or MIDI
- This also directly affects CPU performance.
	- 512 is the default, but if we drop it to 64, the CPU usage will increase, while latency will be almost instantaneous.
		- therefore, we might want to drop the size of the buffer when recording, and return it to default when we aren't
