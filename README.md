# Universal Pause Button
------------------------

<img src="https://github.com/ryanries/UniversalPauseButton/blob/master/NiceLogo.png" width="128" height="128" align="center">

I like to play video games. I also have a significant other, and she often walks into the room to talk to me while I'm playing video games. I would like to pause the game so that I can give her my undivided attention while she's talking to me, but a lot of games (particularly single-player ones) have these "un-pausable" cut scenes or other areas of the game where the normal pause functionality doesn't work.  This annoys both me and her, because I'm supposed to be the computer expert, and it looks like I don't even know how to pause my stupid video game.  So usually what ends up happening is I skip the cut scene and miss the story, or upset my SO by not paying attention to her as well as I should.

So that is why I wrote Universal Pause Button. It's a very simple Windows desktop app that sits in the system tray. Its icon resembles a pause button. When you hit the actual Pause key (also known as Break) on your keyboard, the program determines which window is currently in the foreground (i.e. your game's window,) and pauses it.  No matter where you are in the game. Even in the middle of one of those pesky cutscenes that would otherwise be un-pausable. When you press the key again, the game will un-pause. You can also specify a process by name in the registry to pause and un-pause that process, regardless of whatever the foreground window may be.

I first wrote this app in 2015, but mostly forgot about it since then. But it has always been my most popular app, so today in 2023 I've come back and rewritten the app from scratch, adding several improvements along the way.

Back in 2015, I used this app with The Witcher 3, and it worked great.

Today in 2023, I used this app with Baldur's Gate 3 and it is still working great so far.

However, your mileage may vary. "Pausing" processes is something that usually only debuggers do, and not every process will react the same way to being paused. Pausing processes may lead to race conditions among the threads of that process, but like I said, testing has been very positive for me so far. I've already gotten great value out of the program, as there are lots of cut scenes in The Witcher 3, that I don't want to skip. The main use case for this app is single player games, as pausing your multi-player game will undoubtedly just get you kicked from the session, as if your computer had just crashed or hung. So don't use it in multi-player games. It also works on applications that are not games at all.

There are some new registry settings you should be aware of:

![Registry](https://github.com/ryanries/UniversalPauseButton/blob/master/registry.png)