
Noise gates often implement *hysteresis* 
- that is, they have two thresholds: one to open the gate and another, set a few dB below, to close the gate.

When using a gate, you have to be careful that you aren't gating other sounds that are desirable
- ex. imagine we want to eliminate some breathing noises in our recording, so we naturally add a gate. Consider that breaths are likely to occur after a period of not singing (ex. between verses). Therefore, to ensure we don't trim the start of the vocal part, we want the gate to open quickly (short attack time). At the same time, we don't want to attenuate fading vocals, so we need to make sure the gate is a bit more lax with re-enabling the gate after a signal volume has dropped below the threshold (long *hold* time+slow release time)

If we do this and don't adjust the release to be a bit slower, then we will find that a shorter release will cause vocal fades to attenuate unexpectedly, since they will not meet the threshold of the gate.

### Ducking mode
Some Gates have a ducking mode that when enabled, cause the gate to open *only* when the volume drops below a certain threshold.

Ducking is similar to [[side-chain compression|music.engineering.mixing.compressor#side-chain-compression,1:#*]], but can sound quite different because it's processed as "inverted" gating instead of compression
