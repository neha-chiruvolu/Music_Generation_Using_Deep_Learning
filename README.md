Music Generation Using Deep Learning
Abstract

Music generation using artificial intelligence is an emerging field that combines deep learning and musical creativity.
This project implements a music generation system using a Long Short-Term Memory (LSTM) neural network.
The model is trained on MIDI files, learns musical patterns, and generates new piano music automatically.

The project demonstrates how deep learning models can understand sequential data such as music and produce original compositions.

 Objective

The main objectives of this project are:

To understand how deep learning models can learn musical patterns

To process and analyze MIDI music data

To generate new music compositions using an LSTM-based neural network

To implement an end-to-end AI music generation system using Python

 Technologies Used

Python 3.14

PyTorch – Deep learning framework

music21 – MIDI file processing and music representation

NumPy – Numerical and array operations

 Dataset Description

The dataset consists of piano MIDI files

MIDI files store musical notes, chords, and timing information

MIDI format is efficient for symbolic music generation compared to raw audio

 System Architecture

MIDI File Input

Note & Chord Extraction

Sequence Creation

LSTM Neural Network Training

Music Prediction

MIDI File Generation

 Methodology
1️ MIDI Preprocessing

MIDI files are parsed using the music21 library

Individual notes and chords are extracted

Chords are represented as grouped note values

Musical elements are stored as sequential data

2️ Data Encoding

Musical notes are converted into numerical values

A dictionary mapping is created for note-to-number conversion

This allows the neural network to process musical data

3️ Sequence Generation

Fixed-length sequences of 50 notes are created

The model learns to predict the next note in a sequence

Input-output pairs are generated for training

4️ Model Architecture

A 2-layer LSTM (Long Short-Term Memory) network is used

LSTM is chosen because it handles long-term dependencies in sequential data

A fully connected layer outputs probabilities for each musical note

5️ Model Training

Loss Function: CrossEntropy Loss

Optimizer: Adam

The model is trained for multiple epochs

Training loss decreases as the model learns musical structure

6️ Music Generation

A random seed sequence is selected

The trained model predicts new notes iteratively

Generated notes are converted back into MIDI format

The final output is saved as a .mid file

 Output

Generated file:

generated_music.mid


The file can be played using:

Windows Media Player

VLC Media Player

MuseScore

FL Studio or any DAW

 Results

Successfully trained an LSTM model on MIDI data

Generated original piano music sequences

Demonstrated effective learning of musical patterns

Conclusion

This project successfully demonstrates how deep learning can be applied to music generation.
By using an LSTM-based neural network, the system learns musical patterns from MIDI files and produces new compositions.
The project highlights the potential of AI in creative fields such as music.
