---
title: "Heating Up With Storytime"
date: 2025-02-16T15:34:30-04:00
classes: wide
max-width: calc(100vw - 200px);
---

This week has a busy one on Storytime; some of the more core components to the whole experience have finally been introduced.

As we inch closer to first playable, there are a few essential features that need be represented in some form before we can really "find the fun" of the experience. So that is what I spent the last week doing!

First up was the undo / redo stack. 

---

StoryTime is a gamified tool but at the core, there are certain features that are required to have it function even as a tool. Undo / Redo stack is obviously high up that list. There's nothing worse than making a mistake and having to live with that mistake, especially when putting together your dream story.

When first approaching the task, it was quite daunting. There are various different commands and features that would need undo / redo functionality, so much so that I couldn't figure out an initial approach. At times like that, I like to take a step back and K.I.S.S (Keep it simple, stupid!) to see if there was a way forward where I could start with a skeleton and flesh it out as I understood my plan of attack better down the line.

Fortunately for me, the Undo / Redo stack ended up being a lot more simplier than I had thought. I was paralyzed by choice on implemention which had led me to think about it way deeper than I really needed to.

At the basic core, to make an undo / redo stack work, I simply needed to track when a command was executed. Once I figured that part out, all I'd have to do is redo that command in the opposite way if undo is called.

In the beginning, I was imaginging linked lists, interfaces, memory management, all the scary coding buzzwords. In the end, all I needed was a simple array, a subsystem to manage the array and a custom class that gets create when an operation is performed.

Once those pieces were together, the system essentially handled itself - adding a command adds it to the stack, undoing reverts the change and redo does it again. Essentially just two arrays; the undo stack and redo stack.

If a command is performed, it gets added to the undo stack. If it gets undone, it gets put on the redo stack. It really ended up that simple. 

The only complex part now is remembering to make a new child class for differing functionality if I introduce a new command the player can use. After that, the system essentially runs itself on auto-pilot.

It's always nice to have an "easy win" when you're expecting a war and it is a good reminder that sometimes if something is feeling super complicated, sometimes taking a step back and saving you from overthinking can simplify everything.

---

Now that the undo / redo stack is in, I had a new battle to face.

I managed to get this far adding cool features such as position, scale and pose (did I mention I added those? I'll talk about them soon, I promise!) to a pre-made scene. I already had the characters in and I did not need to worry about persistence between frames or specifically - the differences between frames.

I've decided to call these frames "scenes" - just to keep the wording consistent in the project and to stop me getting confused. Their name will change at some point (as the gamification process continues) but for now, I've got a "cheated" scene but it is time to stop stalling - I needed to introduce the scene system.

Luckily all the work done to this point helped lay out what is needed to be stored per "scene" - characters in the scene, their positions .etc. All the things I exposed for the undo / redo stack, they need to be represented in the "scene". 

So, using the undo / redo stack classes as a base, I built the struct that collects all the data needed to "remember" a scene exactly as it appears on a players screen.

From this point, the concept of a "scene" has been introduced into the code base and I need to now confirm it functions as intended by creating the "flow" system (allowing the user to traverse through scenes, with decision points .etc). No moer cheat scenes! 

I won't lie, it's another mammoth task but one that I'm inspired to get stuck in with after the massive win of the undo / redo stack. 

I hope the next blog entry will go into depth on how I came up with an epic flow system and not how I miserably failed and lost all hope. Only one way to find out anyway!

--- 

Until next time, as always, thanks for reading and good morning, evening, noon or night, or whatever it is where you are and I’ll see you in the next post.

Cheers, Midafir.