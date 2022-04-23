# Anime Music Generation

LSTM model to generate anime music.

## Description

* piano_transcription_inference.ipynb: Translate normal .wav music to .mid MIDI Music.
* music-generation-lstm-comic.ipynb: Provide training code and reuse pre-trained model to generate new music.
* comic.zip: Training set
* ./saves_comic/model200.h5: pre-trained model.
* ./saves_comic/symb_comic.npy: Contains all the possible notes.
* ./saves_comic/X_seeds_comic.npy: Contains random beginning of the music, used by the model as it needs some initial notes to continue with.
* ./example_output: An sample output, in .mid and .wav.
## Getting Started

### Dependencies(install via pip): 

* music21: A toolkit for computer-aided musical analysis
* piano-transcription-inference: Provide piano transcription inference, transcribe piano recordings to MIDI file
* tensorflow
* pandas
* numpy
* seaborn
* IPython
* sklearn
* dimi2audio

### Dependencies(install via package manager apt):
* lilypond: for displaying music notations
* fluidSynth: interpret from MIDI signals and synthesis audio
* ffmpeg: convert file format from MIDI to WAV and MP3 to MIDI


### Generating Music
* Download this rep
* Open music-generation-lstm-comic.ipynb
* Run the last four blocks(from the reloading of model) to generate new music.

### Training
* Use piano_transcription_inference.ipynb to convert your .wav to .mid
* You can also use the comic.zip as training set(our choice)
* unzip the music to ./input/comic
* Run music-generation-lstm-comic.ipynb

## Help

Do not use this model for commercial purpose, as the music in the training dataset can be only used for studies.
If you have any trouble running the code, you can set up an issue or email me at xalphinions@gmail.com.

## Authors

Deep Learning Music Generation Team