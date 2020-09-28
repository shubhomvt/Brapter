# Brapter

The video link is available here
https://www.youtube.com/playlist?list=PLMJokqjqAR_gH-KbJe5b01WSkan27ysAj


Brapter-Compact-Braille-Transput-Communicator
A handy device which is a set of braille e-notepad and an embosser that helps blind people to make notes

Code for Braille e-Notepad:
This is the code developed for the Braille e-Notepad Code Description The code is developed to implement the following functions:

Check if SD card is initialized
Take-in the braille input pattern and save it when '#' key is pressed
Compare the entered Braille pattern to the corresponding English abphabet and store it in a variable
Open the text file if exist, else create a new text file named Input_File.txt
If the file is successfully created, the write the alphabet to the file and close it
Play the audio response for the corresponding alphabet; The audio files are stored in the same SD card if the character is invalid, then print 'error'
Code for Braille embosser
This code is developed to operate the 'Braille Embosser'. Braille embosser is a custom made printer that reads the SD card and embossses the characters in Braille language. Two stepper motors used to traverse the punching head along X and Y axes. A servo motor is used to punch holes on the paper to emboss the braille characters on the paper along the Z axis.

The code works as follows:

initialize the SD card
open the file. note that only one file can be open at a time, so you have to close this one before opening another.
open the file for reading: Enter the file name that contains the characters to be printed If the file is opened successfully, read character by character and store it in an array and close the file
Punch the characters on the paper row by row; 30 characters per line Braille characters have 6 dots as shown- .. row 1, .. row 2, .. row 3 This algorithm prints the characters row by row.
