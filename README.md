# EnTrack
A custom HTML5 video player coded in JavaScript and styled in CSS that allows the user to choose a local video file and up to two subtitle tracks that allows one to seek to the next and previous subtitle, modify their sync times in realtime using hotkeys, and various other subtitle manipulating operations.

I wanted to encapsulate anything you would need to use the program into one file for most accessibility and ease of use.

# How to use/Shortcuts
Just download the repository - the only file you need is the html one.

* ← Left arrow key: Skim to the previous subtitle cue
* → Right arrow key: Skim to the next subtitle cue
* ↓ Down arrow key:     Decrease volume by 5%
* ↑ Up arrow key:       Increase volume by 5%

* S: Toggle primary subtitle track
* R: Toggle secondary subtitile track
* A: Replay video from beginning of current subtitlie cue
* M: mute
* F: toggle fullscreen
* Z: Shift secondary subtitle times back by 0.1 seconds (100 milliseconds)
* X: Shift secondary subtitle times forward by 0.1 seconds
* G: Shift primary subtitle times back by 0.1 seconds
* H: Shift primary subtitle times forward by 0.1 seconds

# Things to Add
As it is now, I am using Font Awesome 5 Video/Audio icons, which require a CDN (i.e. internet connection) for the icons to be loaded so the icons will not all appear without an internet connection, however the buttons are still there and can be used.
I've added a pure CSS alternative for the play/pause button, but other pure CSS/offline solutions are still needed for the:
* Audio icon
* Fullscreen icon

# Things to Modify
Two play/pause button versions exist on the controls bar, pure CSS and FA icons. One of the two should be removed/hidden.
