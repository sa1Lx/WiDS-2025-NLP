# Week 5 Report — Speech-to-Text Basics

## Goal
Try a small speech-to-text workflow: load speech data, do basic preprocessing, run feature/tokenizer steps, and test a pretrained ASR model.

## What I did
- Loaded a tiny slice of Common Voice (with fallbacks) and resampled audio to 16 kHz; saved a demo clip for reuse.
- Ran Wav2Vec2 and Whisper processors to generate model-ready inputs from one sample.
- Ran an end-to-end inference with the pretrained `facebook/wav2vec2-base-960h` model as a mini project demo.

## Notebooks
- [Week 5/01_dataset_preprocessing.ipynb](01_dataset_preprocessing.ipynb): dataset slice, resample, normalize, save example audio.
- [Week 5/02_feature_tokenizer.ipynb](02_feature_tokenizer.ipynb): feature extraction with Wav2Vec2/Whisper processors on a single sample.
- [Week 5/03_mini_project_stt_demo.ipynb](03_mini_project_stt_demo.ipynb): ASR pipeline inference demo; includes a commented fine-tuning skeleton.
