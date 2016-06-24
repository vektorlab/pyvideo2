---
Category: 'EuroPython 2014'
Copyright: 'http://creativecommons.org/licenses/by/3.0/'
Language: 'English'
SourceUrl: 'http://www.youtube.com/watch?v=6ewIEOyC5v0'
Speakers: [Andreas Klostermann]
Tags: []
ThumbnailUrl: 'http://i.ytimg.com/vi/6ewIEOyC5v0/hqdefault.jpg'
Title: 'Brain Waves for Hackers'
date: '2014-07-22'
---
A new class of cheap consumer EEG devices allows ordinary hackers and even high school students a glimpse into the human brain.

This talk will present how to use the "Neurosky Mindwave" headset with python software, and lay out the basic scientific and technical background.

The Mindwave Mobile is a device that can be easily talked to using bluetooth, and it talks a binary protocol which is specifically designed to be useful without  much computing power in the receiving device or advanced knowledge of signal processing. In fact, an Arduino with a few lines of code is perfectly capable of parsing some of the byte stream and reacting to the mental state of the user, while fully-featured python software can do advanced analysis using PyEEG and Pandas.

The same hardware module and protocol is used in the Nekomimi headset (mind-controlled cat ears for cosplay) and some Boardgames (MindFlex).

A python library for interfacing with the headset is presented and will be demonstrated on stage. Mostly kivy applications will be used.

Also I will present some data analysis you can perform with pandas and scipy.

Neurofeedback is a type of mental exercise where a computer uses the EEG data to direct the user towards certain mental states. In the easiest configuration a program would display a bar with the "concentration" level, and the user would learn how to tilt this bar upwards. In more complicated setups a game could react favorably towards states like relaxation or concentration. Using Gamification, Neurofeedback can provide a more engaging experience for children or adults, than other techniques with similar goals, like mindfulness meditation, and the more immediate feedback should enhance the effectiveness of mental training, though that has not been investigated scientifically yet.

Neurofeedback has been shown to be effective (albeit not recommended as sole treatment) in Patients with Attention Deficit Hyperactivity Disorder (ADHD), Epilepsy and Dementia. Some background about these conditions and applications of Neurofeedback to them will be given. The first use of Neurofeedback was done in Cats, during early experiments with EEG electrodes in the 60ies. Cats where conditioned to exhibit certain wave patterns, and later, due to a coincidence, the researchers noticed that the conditioned cats where more resistant to epilepsy-inducing medications. The effect has since been reproduced in humans, in cases where medications did not work sufficiently.

Ample hints on not to treat any of this information as medical advice will be provided.

The goal of this talk is to promote Neurofeedback as a useful mental training and to encourage development of applications around Neurofeedback and the analysis of EEG data, from the perspective of a python hacker.

I gave a similar talk at PyConDe 2013 in Cologne. The new talk will be in English, show some improvements on the software, and more advanced demonstrations.