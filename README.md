![ReadmeBanner](https://user-images.githubusercontent.com/16472141/137603172-119a2cc1-a047-4984-bfc6-0c76123e185b.jpg)

**A prefab for scheduling dynamic soundtracks that musically switch between sections/loops/bars (for VRChat!)**

This system is built around the idea of "audio scenes" in which each scene is a new cue for the music. It uses dspTime (recently exposed in Udon) for precise scheduling! It handles moving between loops/bars, playing one-time transitions section into loops, and can fire off external game events at the end of cues if desired. 

Uses Graphs (Sorry!)

----

### Quick Start:
#### *Simple queueing and scheduling of music sections*



- Drag-and-drop the prefab into your scene hierarchy
- Populate the `audioCues` array with your audio clips/loops
- Change the `audioScene` value at runtime + it will schedule/play through your loops automatically!

#### *Transition Cues / Audio Scenes That Play One Time + Move Onto The Next Scene*

- Add `_transition` to the end of the audio clip you want this to happen on.

![20211016 033734PM](https://user-images.githubusercontent.com/16472141/137600109-2a224efa-3d4a-4154-83ce-5a02382f904a.gif)

You're done! That's it! 👍

### [Please reads the full docs!](https://github.com/kid-kwazine/Udon-Dynamic-Soundtrack-Controller/blob/58dd17fe838fe347a1666fd532c447b6ad0971e8/DSC%20-%20Docs%20(2021-10-16).pdf)
> *Docs further explain the benefits of scheduling, cover firing custom (game) events off audio cue end/start, syncing, interrupt transitions, best practices, etc.*




----

Will try to get some form of demo/tutorial video out before the end of the year for this (and some other stuff!) <!-- yeah, do that -->

Required:
- Unity 2019.4.31f1 + The Patience To Use It
- [VRCSDK3-WORLD-2021.xx.x.xx.xx and above](https://vrchat.com/home/download) (when they exposed dspTime) <!-- Fill this with actual SDK dates when it goes live -->

Have fun + show me if you make anything cool w it! ✨
