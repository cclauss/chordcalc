chordcalc
=========

Turning  Gek S. Low's chordcalc python script into a full-featured chord calculator/player 


This is a gui verion of Gek S. Low's chordcalc ommand line python tool for displaying chords fingerings for a variety of stringed/fretted insruments.  It used the pythonista ui module heavily.  Also incluided is a scipt to build simple wave files used to sound the chords and tunings.

chordcalc.py

- launches the gui.  You choose the instrument/tuning, the chord and root and all possible chords are displayable using the up/down buttons.   If a chord cannot be presented because all its notes cannot be simultaneously played, the user are prompted to abandon the root, 3rd or 5th.  (mandolins in LOW_3 and HIGH_3 (see below) mode do this automatically).  Selected subsets of fingerings is accomplished using the filters.  Low_3/4 play force the upper notes n guitar/mandolins to unpayed.  Similr for HIGH_3/4.   Aother filteers are available.

- Once the sound files are loaded, you can play the sounds of the notes either as a chord or an arrpegio, and you can play the open strings to hear the tuning.

makeWaves.py

- creates 96 sound files of simulated plucked notes for the lower 8 octaves of a piano.

chordcalc_constants.py

- the various settings, tunings and  some filter related stuff.

to do:

- get "DOUBLE STOPS" filter working
- reverse serch.  PPut in a fingering andhave th program identify the possible chords it represents.
