## Python Users Berlin Meetup June 2015
# Audio Feature Extraction with Essentia, Python and Sonic Visualiser
#### Lightning Talk by Thomas Walther - thomaswa@ccrma.stanford.edu

## Goal
- Use Sonic Visualiser to explore, play with and choose audio feature extraction algorithms
- Use Essentia and Python to quickly get a production-ready implementation

This repository contains the iPython notebook of the lightning talk, where we applied the *Vicker's Loudness* feature extractor to an audio file, to get a good representation of the volume of the track at a point in time. We started by testing the *Vicker's Loudness* algorithm in Sonic Visualiser, and then re-created it with Essentia in the iPython notebook.

![Vickers Loudness in Sonic Visualiser](https://raw.githubusercontent.com/tcwalther/essentia-lightning-talk/master/sonic-visualiser-screenshot.png)

## About Essentia

Essentia is an audio feature extraction library for C++ and Python. It is being actively developed by the Music Technology Group at the Universidad Pompeu Fabra in Barcelona.

http://essentia.upf.edu

To my knowledge, it's the best open-source audio feature extraction library out there. It contains a plethora of algorithms, great documentation with links to the original papers, is stable, actively developed and extremely fast. Implementations are done in C++, and the Python wrappers use a lot of numpy. Python is a first-class citizen in Essentia, not just a half-hearted add-on (i.e., very much unlike OpenCV, where the Python bindings are always behind the C++ code).

### What It's Good For
Audio Feature Extraction. That means getting some information out of audio, like loudness, variance, pitch, tempo.

### What It's Not Good For
Audio effects. This is not a library for applying delay, reverb, chorus, distortion etc.

### License
Affero GPL3. That's GPL3, with the additional constraint that if you modify it and deploy it to a server, you have to share your source code, too (not only when you deploy it to an end user).


## Sonic Visualiser
A great tool from Queen Mary University in London for visualizing audio and audio feature extractors. See http://www.sonicvisualiser.org

## About Me
Music Software Developer, Stanford CCRMA graduate (Center for Computer Research in Music and Acoustics), working on audio DSP and server backends. http://www.thomas-walther.com


# Essentia + Sonic Visualiser: The Great Combination
All Essentia feature extractions can be tested and viewed in Sonic Visualiser. Here's an example