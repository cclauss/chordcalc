chordcalc
=========

Turning  Gek S. Low's chordcalc python script into a full-featured chord calculator/player 


This is a gui verion of Gek S. Low's chordcalc command line python tool for displaying chord fingerings for a variety of stringed/fretted insruments.  It uses the pythonista ui module heavily.  Also incluided is a script to build set of simple wave files used to sound the chords and tunings. The fretboard is a custom view including a draw method.

chordcalc.py

- launches the gui.  You choose the instrument/tuning, the chord and root and all possible chords are displayable using the up/down buttons.   The part of the chord is labelled on each fingered or open string that is sounded.  Deadened strings are displayed with an "X" at the nut, while open strings are marked a the nut with their chord tone.  

-- If a chord cannot be presented because all its notes cannot be simultaneously played, the user are prompted to abandon the root, 3rd or 5th.  (mandolins in LOW_3 and HIGH_3 (see below) mode do this automatically).  Selected subsets of fingerings is accomplished using the filters.  LOW_3/4 filter forces the upper notes on guitar/mandolins to go  unplayed (dead).  Similar for HIGH_3/4.   Other filters are available.

- You can play the sounds of the notes either as a chord or an arpeggio, and you can play the open strings to hear the tuning.  The former have labelled buttons.  The later is the display above the "nut" of the fretboard.  If the sound files are not available, you are warned to run makeWaves.py to created them  Takes about 10 minutes on an iPad 2.  

makeWaves.py

- creates 96 sound files of simulated plucked notes (first 8 harmonics, all of equal intensity) for the lower 8 octaves of a piano.  If you run it a second time, you are asked to confirm.  You may want to adjust the number/distribution of harmonic or the attack and decay envelop.  Enjoy.

chordcalc_constants.py

- the various settings, tunings and  some filter related stuff.

to do:

- get "DOUBLE STOPS" filter working
- reverse search.  Put in a fingering and have the program identify the possible chords that the fingering represents.
