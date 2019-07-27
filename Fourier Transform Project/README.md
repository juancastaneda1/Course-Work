This purpose of this project was to create computer generated melodies over a sequence of musical chords, with varying degrees of 
"pleasantness".

To accomplish this, the audio file of each chord was analyzed using a fast fourier transform in order to determine the notes being played, 
and from there the name of the chord. Once the chord was identified, a series of musical notes was generated in such a way as to have a 
high or low degree of "pleasantness" 

This was done by finding the major scale that corresponded to the chord that was identified. Each note was then generated at random, and if
it was in the scale, automatically accepted. If not, the circle of fifths was used to estimate how dissonant the note would sound with 
respect to the major scale and ranked as "worst", "bad", or "better". A probability of acceptance was hardcoded for each ranking. These 
probabilities were modified several times in order to accept the dissonant notes none of the time, some of the time, or all of the time, 
in order to judge the "pleasantness" of the resulting melodies.

At the end of the code, some plots of superpositions of sinusoidal functions are generated in order to discuss consonance and dissonance.



Note: some of the helper functions were written by my partner for this assignment
