---
layout: post
title: Cool automation tools
date: 2016-06-20 16:19
author: Gino Galotti
style: fill
tags: [Automation, Testing]
---
Few months ago I started gathering all testing articles and examples that I came across. I have a really awful memory, and discussing with my QA Lead about different approaches I could just remember some of the details, which led to awkward conversations; so starting to build my own "Testing Bible" sounded like an amazing idea. And so I did.

It's actually a Google Doc where you can find chapters about specific testing methodologies (Rapid Software Testing, Quality Assistance), automation tricks, arguments to convince stakeholders and developers, a bullet point list of my achievements and some cool automation examples. Today I want to talk about the later!

I really love hearing about tools or techniques that organisation has developed to meet their really weird and niche testing needs. [Google Testing Automation Conference](https://developers.google.com/google-test-automation-conference/) is an amazing place to find some of them, as well as companies with tech blogs (although in some cases they think testing is not an enough appealing subject to talk about). So let's talk about some of the ones I felt in love with!

[Netflix Simian Army](https://youtu.be/xkP70Zhhix4)

This is bringing fault injection (https://en.wikipedia.org/wiki/Fault_injection) to the next level. In order to build a resilient system, Netflix realised that they need to be ready for errors. The best way the found to probe it was injecting errors in the pieces that are out of their control, so they understand what's going to happen when those genuinely occurs. The talk is centred about the army of simians that they have causing AWS errors in production.

Things, like killing AWS instances or faking an entire region downtime on Amazon, are the duties of this monkey gang. They periodically trigger them on production to see the progress and be ready for when shit happens. Because we know that shit always happens. Part of the source [can be found here](https://github.com/Netflix/SimianArmy).

[Facebook's test killer](https://youtu.be/_5Sr4EYH7M8)

As I've already mentioned, Facebook is known for not having Testing roles. They heavily rely on automation, although we know that flakiness and inconsistency is one of the biggest pains automating tests. That's why they've come with a system where tests have to gain trust before the system will consider them as necessary; as well as a way to identify, heal and fix tests that cause more noise than benefits.

The system automatically marks the failed tests as "_unknown value_", passing them through various states and identifying the responsible of it. It helps to review the code, and the system is the one disabling someone else's test when it starts feeling flaky, so it's not a "me against you" argument.

[Generate tests from logs](https://youtu.be/ExXATBlygl0)

Creating a complete suite of unit testing can be a daunting task. particularly when you scale up the product size. With this solution, they rely on an extensive logging and machine learning techniques to generate stateless and contextual assertions, building the skeleton of the functional tests.

You'll still need some human intervention, but this is undoubtedly an amazing starting point, leveraging the most tedious part of the process. This is proper automation: something that assists us to achieve our goals!

[Spotify's Rapid check](https://labs.spotify.com/2015/06/25/rapid-check/)

Testing all the range of values in a unit test is impossible, that's why Spotify has used the [RapidCheck](https://github.com/emil-e/rapidcheck) idea to help them build better coverage of the range. It randomly tests a broader set of values, setting a skeleton of important cases. Every tool that helps us get confidence on the solution faster is welcomed!

Do you know about another interesting testing tool? I've left some of them unsaid, but only because I love having pending subjects to talk about in future posts!