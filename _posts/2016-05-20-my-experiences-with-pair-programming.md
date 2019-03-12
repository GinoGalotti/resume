---
layout: post
title: My experiences with pair programming
date: 2016-05-20 15:58
author: Gino Galotti
style: fill
tags: [Personal lessons, Software Development, Testing]
---
[Pair programming](https://en.wikipedia.org/wiki/Pair_programming) has been one of the buzz techniques for a while now. In our industry, you can find groupies of it, professionals who understand its value but don't know how to practice it and others who don't see its value but will defend it anyway. Its value has been proved over and over again, so any developer who talks against it will lose points with his peers.

But I'm not here to talk about industry trends and tabus (microservices as the new default solution). but about my experiences with Pair programming, what I've learnt and where I've found value using it. This is the direct response of a "Which are the downsides of pair programming?" question during an interview. So... let's start!

In most situations, when I've worked with developers pairing (either between them or with me), I've got way more out of it than the downsides. That's why I'd love to start with the obvious advantages of the technique:

* Getting early feedback. Code reviews are a standard nowadays, and pair programming is a live code review where someone is questioning your engineering practices. Also, it helps to spot some major issues.
* Learning from different skillsets. Every developer follows his own book and learning other ways to do things (even if the difference is just minimal) which enrich your solution's toolbelt.
* More polished deliverable. When you deliver something after pairing, you know that it had been reviewed, probably tested (even if it's just in your peer's head), better practices has been followed (every shortcut will need an explanation, and you want to impress!). In my experience, pair-developed features need fewer interactions, particularly when the requirements were fuzzy.
* Work out assumptions and incomplete requirements. When requirements are not completely specified having someone asking you about the unconscious assumptions that you are taking allow the team to raise the correct questions to Product, and therefore need fewer iterations or (even better) don't release with assumptions totally unrelated with the product. This is more powerful with cross-functional pairing techniques.
* Cross-functional pairing. Luckily, as a Software Developer in Test, I've paired with programmers to get a better understanding of the solution, as well as helping them identifying potential problems and building more testable applications. I've seen this with Product people as well (designers, business analysts, etc.), although in that case instead of pair programming I'd call it assisted programming. Group programming is one of the evolutions, and there having cross-functional helpers will greatly enrich the development.
* Avoiding the zone (or Flow state). Pairing prevents a developer to entering [the Zone](http://c2.com/cgi/wiki?MentalStateCalledFlow) as we know it. You can get to a highly productive state with your partner, building momentum and getting answers and solutions straight away. As we stayed in the Clean Code review, some professionals try to avoid the Zone as it can prevent good practices being followed.

On the other hand, I've also discovered that Pair programming doesn't have the same level of productivity (nor viability) on every given situation.

* The speed. This technique may slow down the development, especially until the pair learn how to work together and build some momentum. It heavily varies on the developers itself, as it is...
* Difficult for some archetypes. There are developers that don't know how to pair, or they just can't. They're used to having their own introspection moment, usually relying on the Zone to get the job done at good pace. This is an amazing technique to spot this kind of developers if you want to avoid them.
* Building dependencies. Some people get comfortable and rely on the partner to deal with certain kind of jobs, building a dependent relationship where instead of learning they can just use each other. Again, luckily this is not always the case, and it helps to spot this kind of developers to avoid them.
* Avoid the zone. There are developers that heavily pursue getting into the Zone.
* Requiring a pair. Working on startups, when you try to build cross-functional Agile teams it'll be hard to find a pair to code with. If you need 2 frontend engineers, 2 building the services, 2 dealing with the operations, a designer, a product owner...

Which are your experiences with Pair progrmaming? Did you find it useful? Did you like it?