# squeezelite

This is a modified version of squeezelite by Adrian Smith (Triode). 
At the moment of writing (October 2015), original code is here: https://code.google.com/p/squeezelite/

This verison was originally meant to always inspect pcm headers (if awaillable)  to detect the real samplerate, depth and endianess,
in order to override the wrong information coming form the server when transcoding or upsampling, this  way you could save encodind 
after upsampling on LMS.

Since october 4 2015 this mod has been incorporated in Daphile.

It now incorporate an original patch from Daphile: Launched with -h prevent lms to downsample in case original samplerate is greater 
than the maximum imposed with -r in command line. 

This is a safety option, becouse LMS could not actually downsample pcm.
