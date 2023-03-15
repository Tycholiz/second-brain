
Vocals are normally panned center, and double-tracked if stereo.

use a dual delay (say with 1/4 note delay length), cutting a lot of low and high out of the delay so that the delay doesn't interfere too much with the original vocal, and instead provides a bed of sustain for the vocals to sit on.
- https://youtu.be/9ho9SyxrqHI?t=494

### Compression/EQ
Compression is a great way to bring a vocal forward in a mix
- it can also cause unappealing sonic artifacts. [[Parallel compression|music.engineering.mixing.compressor.techniques#parallel-compression]] can be used to remedy this issue.
- [guide: adding parallel compression to vocals](https://sundownsessionsstudio.com/parallel-compression-vocals/)

Use a high-pass filter if there are any rumbly low frequencies, and perhaps some lower-mids to make sure that the compressor isn’t getting overloaded — then apply compression to taste — and then with another EQ, perhaps boost around 10-15k to add air. Maybe then send all the vocals to an aux that is part of a multibuss setup and EQ or saturate at that stage, and then again when mastering.

#### De-essing
Strongly consider using a de-esser when using multiple vocal tracks, since the same consonant sounds done by multiple tracks can muddy things up considerably. Consider putting aggressive de-essing on the background vocals only, and only light de-essing on the lead vocal.

#### Try
2 compressors in sequence:
1. fast-ish attack, fast release, ~4:1 ratio
2. slower attack, slower release, ~4:1 ratio (to even out the average level of the signal)

### Delay
Stereo slapback delay is a great way to get a sense of space on vocals without pushing it back too far in the mix
- [A/B](https://youtu.be/dO1OOzfGmLQ?t=269)

#### With ducking
Try applying delay only at the end of phrases. This can be accomplished by having a [[Gate|music.engineering.mixing.gate]] set to [[Ducking|music.engineering.mixing.gate#ducking,1]] mode, and routing the vocals through it via a Side-chain source (an option of the Gate plugin)

### Reverb
Too much reverb on vocals pushes it back too far in the mix.
- try stereo slapback delay instead

Try less density (diffusion) when it comes to reverb for vocals. It helps with clarity, as diffusion can make things sound mushy. We are trained to react to the human voice, so the intuition is to preserve the quality of a voice in the reverberation.

### EQ
When EQing vocals, your default should be to stick with a subtracting EQ approach

If vocals sounds a little dull, experiment with:

| Male/female   | 40-60Hz | 200-400Hz | 1000-3000Hz | 5000-8000Hz | 10000-12000Hz |
|---------------|---------|-----------|-------------|-------------|---------------|
| Female Vocals |         | +2dB      |             | +2dB        |               |
| Male Vocals   |         | +3dB      |             |             |               |

