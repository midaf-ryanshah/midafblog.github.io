---
title: "Check In With Storytime"
date: 2025-02-04T15:34:30-04:00
classes: wide
max-width: calc(100vw - 200px);
---

Let's talk more about Storytime! Gather around the campfire, happy campers and let's chat about what I've been up to.

Before we begin, I should touch on what the end goal is. The goal of Storytime is for a vertically played mobile experience for the imaginary man on the tube / subway / train to be able to open up for 5 or so minutes and either create or discover stories. If that sounds weird to you, I don't blame you but please check out the previous blog post on what Storytime is for more information.

The reason I bring this up is the fact that I've made some changes to the build since we last spoke. Whilst mobile is the goal, I found that not only ideating on how things would function but cramming it onto a mobile screen to be a pain area really slowing things down and stifling creativity. 

In an effort to circumvent the limitations (albeit temporarily), I decided to remix how I was looking at the project. Previously, I had been looking it through a pinhole going wide whereas I felt going from big picture and shrinking down would better assist my creative flow.

What this means for Storytime is that instead of putting it together as a mobile experience (for now), I'm putting it together as a 16:9 experience to be played on a computer. This mainly allows for faster iteration time from idea to practice and allows the experience to be feature-rich THEN converted to a mobile experience instead of having "how does this work in mobile" being the main blocker.

---

Doing this subtle remix, it has allowed me to take a step back (as I've been iterating quite a lot already) and rebuild some of the foundations now that I have more of a mature understanding of what we're building.

Through the iterations, I've come to understand that what Storytime is is a collection of systems. Very specific systems at that. Breaking down the experience, there's two main types of "play", followed by the systems that make those two types of play possible.

- Create
- Discover

What I mean by this is that the player is going to be either creating a story or reading stories. 

If they're reading stories, they might not need all the tools to create a story but most (if not all) systems required for reading will be required to create a story.

If the user is creating a story, they will need one or more of the following systems:
- Pose creator
- Character creator
- Background creator
- CG Creator
- Story editor

Since they don't nessisarily need all systems active depending on their intent (Maybe they have no need to pose characters or create backgrounds and they're simply wanting to re-read a created story .etc) - these systems need to go in in a modular way.

The core of it all is the story editor. No matter what, if you're doing anything that isn't reading a story, you're in the story editor. After that, the other pieces aren't nessisarily required and are only needed to achieve their specific functions (should the user want to perform such tasks).

Due to this, each of the modular pieces should be seperate where possible. In theory, this means we can shrink the final file size right down as people will only need the features they actually want at that time. The theory is sold, anyway.

---

So at the moment, we're in 16:9 and have this new feature based design of the code base. Not bad for a minor remix.

In terms of boots on the ground stuff, this has allowed me to enhance how character placement and editing them works. When I say editing, I mean changing their scale, position, mesh .etc. Pretty cool stuff.

The next steps from here is persistance of characters between frames and transitions (characters appearing and dissapearing).

I have no idea what part comes after that, but that's my main focus right now.

--- 

Until next time, as always, thanks for reading and good morning, evening, noon or night, or whatever it is where you are and I’ll see you in the next post.

Cheers, Midafir.