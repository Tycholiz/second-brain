### Preferences > Device > Request Block Size
This is the interface buffer size
This will set the latency for any live inputs and outputs, whether audio or MIDI
This also directly affects CPU performance.
- 512 is the default, but if we drop it to 64, the CPU usage will increase, while latency will be almost instantaneous.
	- therefore, we might want to drop the size of the buffer when recording, and return it to default when we aren't
