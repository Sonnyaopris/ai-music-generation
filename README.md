# ai-music-generation
Music composition using LSTM, RNN, CNN on MIDI and FMA datasets

Automatic Music Composition using LSTM, CNN, and RNN
This repository contains two main modules:

MIDI music generation using LSTM networks

Audio music generation using MFCC coefficients with RNN

Repository Structure
-folder-
├── mfcc_fma_proiect_psv.ipynb        # Audio generation based on MFCC coefficients
├── midi_AI_generare_muzica.ipynb     # Symbolic music generation (MIDI) with LSTM
└── README.md                         # This file


Requirements
Python 3.8+

Google Colab or Jupyter Notebook

Python libraries:
pip install tensorflow numpy pandas music21 pretty_midi librosa matplotlib scikit-learn pyfluidsynth
and:
sudo apt-get install fluidsynth

Usage Instructions
midi_AI_generare_muzica.ipynb – MIDI-Based Generation
Description:
Trains an LSTM model on note sequences extracted from MIDI files and generates new compositions based on the selected musical genre.

Steps:

MIDI files were manually organized into genre folders in /data/midi/.

Run the notebook step-by-step:

MIDI Preprocessing

LSTM Model Training

Sequence Generation

Output:

Automatically generated .mid file

Converted to .wav using FluidSynth

Visualization:

Spectrogram of the generated sequence

mfcc_fma_proiect_psv.ipynb – MFCC-Based Audio Generation
Description:
Trains a simple RNN to generate audio using MFCC coefficients extracted from music fragments.

Steps:

Uses the FMA Small dataset, available at:
https://github.com/mdeff/fma

Run the notebook:

MFCC Extraction

LSTM Model Training

Generation of new MFCC sequences

Output:

Reconstructed .wav audio file from the generated MFCC

Visualization:

Spectrogram of the generated audio

 Dataset Sources
FMA Small Dataset: https://github.com/mdeff/fma

MIDI Collection: Manually curated MIDI files from public resources, categorized by musical genre

Author
Opriș Sonnya-Mariana
Technical University of Cluj-Napoca
Faculty of Electronics, Telecommunications and Information Technology
