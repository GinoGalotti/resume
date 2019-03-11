---
layout: post
title: It's always worse elsewhere
date: 2016-06-09 13:27
author: Gino Galotti
categories: [Personal lessons, Testing]
---
Yesterday I share a couple of beers with some old friends who also work in the Software industry. They're working on a small Consultancy agency building websites using the same core, cutting most of the production costs as most of them use fairly similar implementations. Everything sounds right until they get surprised when I asked about their testing framework. "Well, before sending them to the client, we navigate through the site checking that anything breaks". Fair enough, I don't expect everyone to use Selenium. "The problem is when a client finds a bug. Most of them are part of the core so that bug is probably on every one of our projects, and we're afraid of refactoring anything". If the core is not a volatile piece of code, probably it'll be a good investment to build some functional tests verification on top of your unit test. "Unit what?". Bum. And then I remembered.

I was also part of a Consultancy brand (it was my first job in the industry). I remember the "we can't afford to write the unit tests, our problem is really complex and we don't have time, we'll just verify it at the end". I bought it. I truly believed that we were good enough that unit test was only a _plus_, and the projects were difficult and fast paced... NO WAY we could afford _wasting_ time on tests! I remember some senior colleagues explaining that to me. Why would I don't follow their example? They had way more experience than me, and they developed way faster. I wanted to be like them.

And I remember the struggles. I remember that every single bug fix carried weird and unexpected regressions. How the clients complained every week, and the constant fight about who is the responsible for the fix (_Was it a bug, or a failure in the requirements_?). The hellish deployments, the tedious manual verifications of _just what was needed_, the numerous problems with our version control tool as we always realised too late that the release didn't contain that change.

I also remember the change. When I left the company and learnt something new in the next one. And then the next one. On my first day, one of my new colleagues was disturbed because I wasn't writing unit tests. He didn't even ask a reason, but I tried to convince him that they _just slow my momentum_. I remember his face. He just taught me how to make it easy, and handled me a copy of [Clean Code](http://www.amazon.co.uk/Clean-Code-Handbook-Software-Craftsmanship/dp/0132350882). I had to pair with him and... Oh God, that was beautiful. He showed to me what TDD feels. And I started realising that, actually, the team didn't spend that much time dealing with the horrors I was used to. It was so simple and beautiful.

That's why I spent some time yesterday trying to show them the importance of this practices. Explaining to them why most of the companies they want to work in ask for TDD practices or writing functional tests. Exampling to them how they've been important during my projects. Giving them resources, guidelines and the chance to ask any question. But, obviously, I'm just a QA, so what the heck I'd know about coding.

Yeah, dear readers, **it's always worse elsewhere**. That's no excuse to not try to be the very best you, including the best professional you can be; but sometimes appreciating what you've learnt and why you're doing it is needed. It is also important to identify who would use some help, and offer it. For me, life is how you feel sharing with the people you choose your knowledge, resources and smiles. I'll talk in further posts about some of the

I'll talk in further posts about some of the anti-patterns I've seen (and do) during my career, and some lessons I've learnt fighting them. But, for now,
