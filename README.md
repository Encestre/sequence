# sequence
Sequence is music tool to sequence audio files.
It allows to define a song structure playing in sequence audio fragments.

Main goal is allowing end user working on song structure using a simple text file as configuration, without knowlegde about MAO and music sequencer.

The configuration file first describe audio fragments availlable.
Then a single line describe the playing sequence, allowing looping and repetition.


# Configuration file usage

[lib]
# Define the audio files library
# audioName:filename
# space are not allowed in audioName
# only wav files are supported
# A:a.wav
# B:b.wav
# C:c.wav

[song]
# Song is describe on 1 line

# two kind of loop can be defined :
# [   ] : only this loop is played when the whole song is played
# <   > : this part is looped during song playing 
# (n) : n repetition. Can be used for audio motif or for loop (after last symbol)
# symbols are separed by space except for repetition     
# A B C
# A(2) < B C >(3)
