## Week 4 Report – Speech Processing

### Goals
- Learn audio basics (waveforms, sampling) and time–frequency views (STFT, spectrogram).
- Extract Mel spectrograms and MFCCs.
- Build a small keyword-spotting demo (toy CNN) to show end-to-end preprocessing → model.

### What I worked on
- `audio_feature_extraction.ipynb`: waveform plotting, STFT/spectrogram, Mel spectrogram, MFCC extraction, and saving features.
- `keyword_spotting_toy.ipynb`: loads a tiny split of Speech Commands, converts waveforms to Mel spectrograms, trains a small CNN for a couple of epochs as a pipeline demo.

### Files
- Notebooks: `audio_feature_extraction.ipynb`, `keyword_spotting_toy.ipynb`.
- Dependencies: `requirements.txt` (librosa, soundfile, numpy, matplotlib, tensorflow, tensorflow-datasets).
