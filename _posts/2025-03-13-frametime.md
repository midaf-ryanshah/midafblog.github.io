---
title: "Frame Persistency (or how I learnt to stop worrying and... "
date: 2025-03-13T15:34:30-04:00
classes: wide
max-width: calc(100vw - 200px);
---
Have you ever had a daunting task in front of you that feels so complicated and insurmountable you try your best to push it off as far as you can and hope that you can find some way out of it? Yeah, me neither.

Obviously, I'm kidding. There's one big piece of Storytime I've been pushing as far away as I possibly can but I fear that I'm not running out of railroad track. Persistance between frames. Basically characters talking in place in frame 1, staying in that place for frame 2.

It sounds simple, right? Sure, but then you have to start thinking about the rammifications and edge cases. What if I make a great scene then decide I want rain. Let's say I have 6 frames, right - what if I go back and want to start the rain effect on Frame 2. Great, now frame 2 has rain. But then surely it would be weird if the frame just stopped in frame 3? So it should continue until stopped right? Okay, that's a little more to it then just flicking an effect on but still doable.

What if I now have 100 frames? 200 frames? What if I want to add a character that wasn't there before? These are simple issues, for sure but it quickly makes "persistence between frames" more and more complicated with each dive into the "what if's".

Sometimes, you have to call time and stop yourself becoming paralized with what-ifs and instead just start implementating and deal with the weird fringe things as they happen.

But that's scary. You can drown in hypotheticals for sure but the uncertainty of unexplored hypotheticals can be just as bad. Surely there must be a term for this in the software development world.

At some point, you just gotta grit your teeth and start. You have to silence your mind and push ahead. I'm at that point with with the frames in Storytime but the possible side-effects are definately giving me pause.

---

To be honest, I probably should not have left such an important feature so late. It's clear that some of the other work going on over the past few weeks have been pure procrastination of not tackling the elephant in the room. 

Where I should have been working on this frame issue, I've been building effects, random menus .etc - things that are good to have for sure but are not blockers to "finding the fun". Frame persistence is definately a blocker to finding the fun.

I think the problem I have right now is looking back, if I were to do this again - I think I'd still have procrastinated around the frames issue. It's such a big part of all of this that it is ridiciously offputting to not do in one long sitting with all the possible knowledge of all the ways it can go wrong .etc.

But enough. I can't keep running from it. If the next blog post isn't about how I aced it and fixed all the issues with the frame persistancy issues than I have not only failed you, dear reader. I would have failed myself too.

---

My plan of attack (at least for now), is exactly how I outlined above. I'm going to try and make the previous frames the "dominant" frames. If I add a rain effect on Frame 2, all frames after should rain until I tell it to stop. If I add a character to frame 6/250 then that character should be added to all following frames until I manually remove it. 

It's the only "clean" way I can see this working, otherwise you're going to have to manually enable these things on every single frame you want them. In a game like Storytime, that could be hundreds if not thousands of frames.

But what about branching storylines and branching frames? Oh no, I'm spiralling again.

Right. Clear head. I'll deal with that part when I get there.

Hopefully next time we talk, I've got it all figured out.

Until then, please wish me luck. And oh, if you know the term for whatever the hell this is; my email inbox is awaiting your wisdom.

---

Until then, as always, thanks for reading and good morning, evening, noon or night, or whatever it is where you are and I’ll see you in the next post.

Cheers, Midafir.
