![ReadmeBanner](https://user-images.githubusercontent.com/16472141/137603172-119a2cc1-a047-4984-bfc6-0c76123e185b.jpg)

**A prefab for scheduling audio that musically switches between sections/loops/bars (in VRChat!)**

This allows you to create dynamic soundtracks directed by player action/gameplay or even build dynamic "music video" experiences

This system is built around the idea of "audio scenes" in which each scene is a new cue for the music. It uses dspTime (recently exposed in Udon) for precise scheduling! It handles moving between loops/bars, playing one-time transition sections into loops, instant stab/stinger transitions, and can fire off external game events at the end of cues if desired. 

Uses Graphs (*Sorry!* It's only one behaviour, though!) </br>
I plan to make a U# version when I have more time so it can have a better inspector!

----

### Setup:

- [Download](https://vrchat.com/home/download) + import the latest version of *SDK3 - Worlds* from VRChat
- [Download](https://github.com/kid-kwazine/Udon-Dynamic-Soundtrack-Controller/releases) + import the latest version of Dynamic Soundtrack Controller into your project
- Drag-and-drop the newly imported Dynamic Soundtrack Controller prefab into your scene 

-----

### Quick Start:
#### *Simple queueing and scheduling of music sections*

- Drag over + populate the `audioCues` array with your audio clips/loops
- Change the `audioScene` value at runtime + it will schedule/play through your loops automatically!

#### *Transition Cues / Audio Scenes That Play One Time + Move Onto The Next Scene*

- Add `_transition` to the end of the audio clip you want this to happen on.

![20211016 033734PM](https://user-images.githubusercontent.com/16472141/137600109-2a224efa-3d4a-4154-83ce-5a02382f904a.gif)

You're done! That's it! 👍

### [Please read the full docs!](https://github.com/kid-kwazine/Udon-Dynamic-Soundtrack-Controller/blob/8cf763de0a3b56e15ab699d9a819aadaaf8ca7b0/HTI%20DSC%20v1.0.0%20-%20Documentation.pdf)
> *Docs further explain the benefits of scheduling, various start behaviours, covers invoking custom (game) events off audio cue end/start, syncing, interrupt/instant transitions, common errors/troubleshooting, best practices, etc.*




----

Will try to get some form of demo/tutorial video out before the end of the year for this (and some other stuff!) <!-- yeah, do that -->

Required:
- Unity 2019.4.31f1 + The Patience To Use It
- [VRCSDK3-WORLD-2021.xx.x.xx.xx and above](https://vrchat.com/home/download) (when they exposed dspTime) <!-- Fill this with actual SDK dates when it goes live -->

Have fun + show me if you make anything cool w it! ✨
