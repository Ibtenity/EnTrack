# EnTrack
A custom HTML5 video player coded in JavaScript and styled in CSS that allows the user to choose a local video file and up to two subtitle tracks that allows one to seek to the next and previous subtitle, modify their sync times in real time using hotkeys, and various other subtitle manipulating operations.

I wanted to encapsulate anything you would need to use the program into one file for maximum accessibility and ease of use.

# How to use/Shortcuts
Just download the repository - the only file you need is the entrack html one.

* ← Left arrow key: Skim to the previous subtitle cue
* → Right arrow key: Skim to the next subtitle cue
* ↓ Down arrow key:     Decrease volume by 5%
* ↑ Up arrow key:       Increase volume by 5%

* Numbers : skim to different parts of the video using the number keys. 1 corresponds to a tenth of the way through the video, 0 to the beginning of the video, 9 to nine tenths, etc.

* S: Toggle primary subtitle track
* R: Toggle secondary subtitile track
* A: Rewind to the beginning of current active subtitle cue
* M: mute
* F: toggle fullscreen
* -: Decrease subtitle font size
* +: Increase subtitle font size
* Q: Shift primary subtitle times back by 1 second
* W: Shift primary subtitle times forward by 1 second
* Z: Shift secondary subtitle times back by 0.1 seconds 
* X: Shift secondary subtitle times forward by 0.1 seconds
* G: Shift primary subtitle times back by 0.1 seconds (100 milliseconds)
* H: Shift primary subtitle times forward by 0.1 seconds
* P: Copy video title, current subtitle timestamp and text to clipboard

## Support
Since this is a browser-based video player, file support depends on the browser. 
In general, webVTT subtitles are the best subtitle files to use, however srt support has now also been added. mp4 files are good, h264 (and h265 now) is good. Google Chrome basically supports MKV, but FireFox doesn't. All in all, Google Chrome is the best browser to use with EnTrack, then it's FireFox. Internet Explorer seems to be a lost cause, and I haven't tried it on any other browsers.

[Here's a link](https://subtitletools.com/convert-to-vtt-online) that can very quickly convert subtitle files of a multitude of types to webVTT at once.

# Things to Add
As it is now, I am using Font Awesome 5 Video/Audio icons, which require a CDN (i.e. internet connection) for the icons to be loaded, so the icons will not all appear without an internet connection, however the buttons are still there and can be used.
I've added a pure CSS alternative for the play/pause button, but other pure CSS/offline solutions are still needed for the:
* Audio icon (pure CSS)
* Fullscreen icon (pure CSS)
* Onscreen feedback for when primary/secondary subtitle track offset times are changed (technically this can already be seen in the top banner)

# Things to Modify
Two play/pause button versions exist on the controls bar, pure CSS and FA icons. One of the two should be removed/hidden.
