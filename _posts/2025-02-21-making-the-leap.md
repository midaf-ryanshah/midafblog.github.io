---
title: "Making the Leap (Linux for Unreal Engine Game Developers)"
date: 2025-02-21T15:34:30-04:00
classes: wide
max-width: calc(100vw - 200px);
---

Have you ever had a moment on clarity where you just want to shake things up in a big way? That kind of happened to me this week.

After years and years and years of Windows, something in me finally snapped this week. I couldn't tell you what specifically it was but I finally realized how unhappy I've been dealing with Windows... windowy-ness. 

The truth is ever since the rise of SteamOS 3.0 - I've been wanting to jump to Linux for a while but as you can guess, crafting AAA games limits what you can and can't do in terms of using a PC. 

There are simply too many questions when changing your whole operating system; what if Unreal Engine doesn't work, or the rest of my dev stack? What if the UX is even worse than how it is when trying to develop the future of games in Windows?

These questions kept me in the clutches of Windows for the longest time - leaving me to stare at people having fun in Linux from afar.

---

Linux is growing as a games platform. It's no where near big at the moment (at time of writing, the Steam hardware survey shows that Linux still only counts as 2% in the "most used OS" category) but Valve have been making great strides in making Linux a viable platform for gamers and general users alike.

In various corners of the web, you can see the growing excitement for the platform. You occasionally see on Reddit, Youtube, Tiktok .etc - people showing off that sometimes Linux runs things even better than Windows can. Even BETTER? Back when I was younger, even having things run at all on Linux was impressive. But now we are in a world where somethings are running even better? This definately gave me pause.

One thing most of the general gaming Linux community seems to agree on is the fact that Linux will "one day be the go-to". It's a rhetoric that has passed through the generations, almost becoming a meme of the OS as a whole. "It'll be good enough one day!". I think I've heard this for most of my computing life. But when will that day come?

I'm not certain that day is today, but I definately feel like Linux is close. Mainly thanks to Valve and the hard work of the creators / maintainers in the Linux community, I think Linux is closing the gap between the "just works" experience you get when using Windows - in fact, I think we're the closest we've ever been. But things aren't _quite_ there yet. At least in my opinion.

---

As you can probably tell, I made the jump. At some point this week, something finally snapped. There was no "right, that's it!" moment or anything as incredible at that but after seeing for a few years now people posting things such as "hey, Linux is good now!" and "Hey, this app works 5% faster on Linux" .etc - something finally clicked and I made the switch.

To be perfectly honest with you, this isn't my first forray into Linux. I'm not a Linux god or anything like that - I mearly spent some time in Desktop mode on the Steam Deck. During my time in Desktop mode, there was something about the experience I didn't hate. In college and university, I had tried Ubuntu and absolutely hated the user experience and those two things have been my main expose to Linux.

After hearing Valve was working on a general release of SteamOS (and quite enjoying the Steam Deck desktop experience), I began looking into how to replicate that without having to wait for Valve.

So I had two goals before I could make the jump: I had to be able to continue using my dev environments to craft AAA games and I wanted to try and replicate that experience I had enjoyed on the Steam Deck.

I ended up using Arch Linux with KDE Plasma - specifically using EndeavourOS, as I had heard it's a way to get Arch Linux in a simple way (there are horror stories on installing Arch). This got me to an experience that even surpassed the good time I had with Steam OS.

In terms of the dev environment stuff, I decided (potentially stupidly) to just wing it. There was limited information online and I finally decided that "hey, if it doesn't work, I can just go back to Windows".

So I did just that. I installed EndeavourOS and I've been here ever since. We're talking a straight up full instance (no dual boot .etc). So how did it go - especially as a person making AA / AAA video-games?

---

I won't bore you with the specifics of all the applications I use to create video-games, we'd be here all day. Let's just talk quickly about the big ones. Communication wise; Zoom, Slack and G Suite all work out of the box. Coding wies; Visual Studio Code and Jet Brains Rider both worked out of the box too. P4V and Github (obviously) work absolutely fine in Linux. Now we get to the elephant in the room, the one you're probably most interested in if you stumbled across this post on your travels: Unreal Engine.

Installing Unreal Engine on Linux is a little more involved than on Windows. You either need to build from source or grab a .zip file from a secret part of the Unreal Engine website. Either option doesn't give you access to the Fab marketplace (though there are community made workarounds / tools to do that). Doing either option is as simple as it would be if you performed said actions in Windows. 

One install later and I was in Unreal Engine. 

Obviously there is no Direct X in Linux, so it defaults to Vulkan. For my projects that is fine but your mileage may vary (especically if you're heavily using DX12 exclusive features). But in about 30 minutes (including pulling latest in P4V), I was back in my projects and working as if I didn't just completely change the OS I was using.

Very cool stuff!

There has been some minor teething issues; especially with Unreal Engine but nothing that a quick google search couldn't fix. Text Input was a bit inconsistent out of the box and there is some weirdness with getting screen co-ordinates (possibly a problem with my own code, to be honest with you). But the important part is Unreal Engine just works on Linux.

---

People say a lot of things about Linux, some of which isn't even true. For the record, I'm using an Nvidia GPU (4070) with Gamescope for most of my gaming needs (something some people in the community swear is not possible).

What I will say is using Arch / Plasma KDE (Linux), I've begun enjoying using the computer again. Having control of everything makes me feel more comfortable when debugging and the community as a whole for Linux is super helpful and it's been a really enjoyable experience thus far.

If I move back to Windows (I doubt console SDKs have linux ports, so I'll probably either have to jump back for that or setup a build machine for that!) - I'll let you know. But for now, I have been converted. I see what the community has been saying and why they're so passionate about Linux. It's been a great ride so far and I'm super happy I decided to make the blind jump into the ecosystem.

--- 

Until next time, as always, thanks for reading and good morning, evening, noon or night, or whatever it is where you are and I’ll see you in the next post.

Cheers, Midafir.
