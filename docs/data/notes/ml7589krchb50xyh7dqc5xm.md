
### Modes
- *Trim/Read* - Existing envelopes are applied, but the onscreen knobs don't move. Adjusting the volume fader in this mode will adjust the track's volume relative to the envelope.
- *Read* - Applies envelopes and moves onscreen knobs for armed items automatically.
- *Touch* - start writing only once the knob has been moved, and stop writing once you've stopped moving the knob
- *Latch* - start writing only once the knob has been moved, and continue writing until playback is stopped.
- *Latch Preview* - changes to the automated parameter will exist only in a preview state, which can be committed with one of the actions `Automation: write current values for actively-writing envelopes ______`
    - `____ to time selection` works well if we are, say, adjusting the volume of an instrument during an instrumental break.
- *Write* - write and remember current settings as edit points, writing all changes made from the moment playback starts until playback stops.