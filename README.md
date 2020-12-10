# eeelooper

Similar to [pdlooper](https://github.com/zigmhount/pdlooper), but written in vanilla Pure Data, and kept minimalistic with as few moving UI things as possible so that it runs smoothly on an old eeePC 701 (900Mhz Celeron with 2GB RAM).

Designed to be used together with audio input channels, a midi pad to load samples in a drumkit patch, and a midi control surface with 64 buttons and 9 faders, with no external software except Jack.

The intention is to keep it minimalistic and CPU-efficient, taking advantage of Pd's visual routing of audio signals to rearrange the inputs, mixers and effects as wished, with controls and visual feedback via MIDI controllers as much as possible (thus needing to watch the screen as little as possible).

![Main patch](images/current_main.png)

## Current features:
- Input from audio sources
- Sampler drumkit for input from MIDI pads
- Mixer for drums 
- Mixer for 8 instruments (8 columns of the APC), flexible routing of inputs and drums
- Basic effects:
  - Mono and stereo panning subpatches
  - Sidechain compressor subpatch
  - Basic reverb on master mixer (`[Freeverb~]`)
  - Basic delay on master mixer
- Vu-meter (bangs)
- Mute/Unmute input into mixer
- Record/Play/Loop/Stop for each of the 64 buttons of the APC
- Tap tempo
- [WIP] Save/Load session
- Performance recordind/playing (wav)
