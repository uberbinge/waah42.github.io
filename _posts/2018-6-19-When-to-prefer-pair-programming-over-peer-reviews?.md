---
layout: post
title: When to prefer pair programming over peer reviews?
permalink: pair-programming-vs-peer-reviews
---

When to prefer pair programming over peer reviews?

First let's get some help from Wikipedia in defining what pair programming and peer review process is, according to Wikipedia:

[Pairing Programming](https://en.wikipedia.org/wiki/Pair_programming) is an agile software development technique in which two programmers work together at one workstation. One, the driver, writes code while the other, the observer or navigator, reviews each line of code as it is typed in. The two programmers switch roles frequently.

[Code review/Peer review](https://en.wikipedia.org/wiki/Code_review) Code review is a systematic examination (sometimes referred to as peer review) of computer source code. It is intended to find mistakes overlooked in software development, improving the overall quality of software.

Now that definitions are out of the way lets talk about discussion types, there are some developers who really think only coding is **work** and discussions are **waste of time**, but for sanity’s sake lets not focus on them. There are some who value quality discussions but are skeptical of (rightly so) discussions for the sake of discussion. Or fighting over popular Tabs vs Spaces, Emacs vs Vim kind of discussion apart from those ones, I think the right amount of communication is really critical between developers of the same team and across teams.

I think **, when** to discuss something, is as important as **what**. For example, there are moments during implementation when five minutes of discussion with a potential reviewer can be the difference between shit hitting the fan and a pleasant smooth feature done.

But finding the right balance between the number of discussions and implementation time is hard. Every developer to some extent likes tasks which they can do alone without involving other people. I think partly because open space office stuff already has lots of distractions and people finding un-interrupted time in office is becoming increasingly difficult nowadays. Also the idea of having to go to a specific meeting room to discuss. Which could feel like overkill for smaller tasks and dreadful for bigger tasks which can take hours some times.
> This is where pair programming really helps a lot as you can discuss potential implementations or even thought process with another developer when trying to find the right clean solution to the problem at hand. No need to schedule separate meetings or explain design decisions at the end like in peer reviews. The reviewer also knows ‘w*hy’* of decisions and helps make the right trade-offs.

## What went wrong in the peer review process?

![Photo by [NeONBRAND](https://unsplash.com/@neonbrand?utm_source=medium&utm_medium=referral) on [Unsplash](https://unsplash.com?utm_source=medium&utm_medium=referral)](https://cdn-images-1.medium.com/max/9792/0*VMejG81Xswz5Lfiv.)*Photo by [NeONBRAND](https://unsplash.com/@neonbrand?utm_source=medium&utm_medium=referral) on [Unsplash](https://unsplash.com?utm_source=medium&utm_medium=referral)*

Our team is structured in a way that every dev is kinda full-stack and supposedly can work on Android, iOS, Backend, and OPS stuff. In practice, most people can work on backend and ops task but there are dedicated people for Android and iOS.
> # When for a longer period of times there were only peer reviews and almost no pairing people kept starting new tickets and then somebody had to be review scapegoat ( stuck in reviews and OPS tasks for weeks meanwhile others are just enjoying the holy trinity of “doing” stuff).

## Solution:

![Photo by [rawpixel](https://unsplash.com/@rawpixel) on [Unsplash](https://unsplash.com)](https://cdn-images-1.medium.com/max/5000/0*NywgvGiBenI8dws2.)*Photo by [rawpixel](https://unsplash.com/@rawpixel) on [Unsplash](https://unsplash.com)*

If you find your team in a similar situation then try to increase pairing over peer reviews. We had a decision that for each story two devs will take lead and responsibility and they can mutually decide what tasks could be done better via pairing and what is better to let someone work alone and then the other lead of the story can review it. Till now it’s working a lot better in our cross-platform team.

For me personally, most times pairing is far better than waiting for review and starting other tickets and having to come back to it later when I’m in the middle of some other ticket. It’s challenging to find out specific scenarios where pairing works better than peer-reviews because those scenarios are different for each team. That’s why
> # Your development workflow decision shouldn’t be too strict for pairing or peer-reviews but let the people decide what works best for them.

There is this great [thread](https://twitter.com/sarahmei/status/990968833547497472) by [Sarah Mei](https://twitter.com/sarahmei) which will help you to keep in mind the power dynamics when pairing so that it’s a pleasant experience for both parties. Teams should pay attention to what could be improved because in Agile process taking advantage of the retro process is really important to improve workflow and team dynamics.

What tweaks you had to make in review process which resulted in better dev workflows and team communication?
