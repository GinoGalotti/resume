---
layout: post
title: Three steps to improve the quality of your development process in a startup
date: 2018-08-19 10:04
author: Gino Galotti
image: /img/post/quality.jpg
categories: [Quality Assistance, Testing]
---
I've been working in the IT industry as a QA engineer since the start of my career. Sometimes, my position was just hands-on testing in a waterfall-like process; other times I worked closely with the developers to write all the automation needed before the feature was considered done. Every company offers a different approach on how to increase the quality of their product, and I've also seen companies trying the same thing with completely different results. But there is always something that kept being constant: when a company reaches enough user-mass or the codebase gets big enough, the conversation about ensuring quality gets more and more important. Speed and productivity matter less if you alienate the users with buggy releases, and your engineering team gets afraid of areas in your code which changes _always carry side effects_. That is the moment when the way of _just getting things done_ that has worked till now starts getting on the way of a healthy product. That's the point when the organization thinks on increasing the QA headcount.

Currently, I'm facing this situation again, with the difference that I feel way more prepared. Of course, every company has a different way of working, but starting to be a veteran in the industry allows me to recognize common troupes and analyze the situation with frameworks which worked for me on previous cases. For some of these steps, I highly recommend finding a person who will bring the expertise on automation or testing principles in your team, but a lot of these steps can be performed without by anyone, especially if you already count with a Quality-crusader in your ranks. And that's what I'm going to help you with right now, giving you an example of the steps you can take to start improving the quality of your product and processes by yourself.

Before starting, I would like to share the first step I take when joining a new startup, particularly if there's not a defined Quality process in place. I always start finding the Quality Crusaders currently working with you, those bright knights who, regardless of their work title, push for a quality-first approach of working and cares about following best practices. I even ask for them during my interviews when considering a new job. Having allies who will share their view on how to improve the current situation is invaluable. So, find them, and involve them in these first steps!

# 1 - Describe the development process.

Ok, so we are all making software here. And the process seems pretty straightforward, doesn't it? Some people sit in a corner. They write some code. They push that code somewhere. And our users enjoy it. Pretty simple. So let's add a little bit more flavor to it, shall we?

I like to start naming the different the different states that a task (bug fix, feature, etc.) goes through before our users _enjoy it to pieces_. Of course, this is more of a guideline than a cooking recipe, but I'll describe an example as broad as possible so hopefully, you can get inspired. In this case, a task can come from a bug report, a new feature requested on some work that we want to do internally (tech debt, etc.). At some point, an engineer will pick it up and start working on it. It will land the codebase. It will be deployed to some testing environment. And finally, it'll be in our user's hands. So, without caring about actions and transitions, the states would be:

> Coding - Code on the repository - Testing environment - Production

Now, let's start the fun part. If we know that our code will go through these steps, how can we improve the quality adding actions or extra transitions?

# 2 - How can we inject that quality?
This will drastically change depending on the previous experiences of your team, as well as what are they currently doing. Involve different people in this step, as they'll offer valuable insight from their previous works of things that worked and didn't. This is an example of what I've proposed in previous occasions. I usually include a short description of the different steps.

![](/img/post/quality-processes.png)

For instance, involving people with different expertise on a Design Document before starting to work on a feature has worked with great success for me. That document can take any shape, but having a little discussion on what is the problem that we're trying to solve, where does it interact with other modules, what is the threshold needed to feel the implementation is good-enough helps A LOT to most engineers when working on it. Just having "what might go wrong" in the back of your head while you're coding a solution can work wonders.

Another key element, apart from the description, is figuring out the owners of those actions. As I said, many don't require any new technical expertise in your organization like Design Document, or Demo Testing where the developer runs through the solution with a peer or a product person to spot errors and understand how others verify that feature. Others really benefit from a specific skillset. That's why, for instance, I took the ownership of working on the automation that will provide a smooth and reliable way to assess a solution. I'd work on building and improving the frameworks (Unit, Integration, End to end, Performance testing...), as well as working with the team so we can all embrace quality.

I also recommend that you don't try to tackle all solutions at the same time. Set priorities, where can you get more bang for your buck, which skillsets do you already have, etc. All of these solutions will go through different cycles, and spending enough time and energy to set a nice foundation will help with the resistance that every organization faces when introducing change. Focus on feeling a constant momentum of change an improvement, instead of the speed of that change. Personally, the workplaces where I could focus on a steady pace, end up having a way more impactful change in the end.

# 3 - Measuring the impact, reviewing and improving.

This is, in my experience, the hardest part. It's really difficult to measure the impact of shifting to a quality-focused development process. Are you having more bugs because the engineers are working on a harder problem? Or did we get better at finding those bugs? As a quality engineer, part of my job is also finding ways to measure the impact of any change, so we can iterate through them and find a better approach. We all share a common goal: develop a product that will bring more value to our users, and doing it in an environment that we enjoy working at.

Spend some time profiling the process so you can get data on it. Sometimes, it's as easy as holding periodical meetings where people discuss how it worked or didn't work for them; or you can find entry points of measurements to take a data-driven decision. Be mindful of how hard this task is. If people feel that they would be reviewed by these metrics, they would be reluctant of iterating and embracing them. This is not about pointing fingers, but devising a way to improve the process for everyone.

As in most tasks I usually work on have more an internal impact than an external one, I like to measure my success on the perception of the codebase by our engineers. Of course, I hope that changes in frameworks and automation will impact the end user experience; but I like to focus on our team first. Examples on measurements that I use are: periodical surveys to the engineering team on how much they like working in our codebase, or how safe they feel when doing a refactor or change based on our automation; pairing with different developers so I can see how they work and their interactions with the frameworks; workshops on how to approach different bugs or problems; etc.

Another thing to be mindful of is that, at this stage in a startup, Quality is a buzzword used as an escape goat quite often. Most teams had to focus on quick and "dirty" deliveries on their first steps as an organization. When the conversation about Quality starts arising, it's usually because that speed has started to produce difficult releases, and "the lack of a QA in your team" is frequently used as an excuse. Having people with different expertise always bring value, but it's everyone's responsibility in following the best possible practices to their knowledge, and voicing their complains about the current process. This situation can also create a toxic situation where, after hiring someone who that expertise, it'd be required from them to just fix everything.

# Final notes

To wrap it up, I want to finish that this is not a magical tool that will increase your productivity and ensure the quality of your product by itself. This is a progressive change of mindset. It's about changing how we work to spend more time on "how we can ensure and verify the solution", and less on "how can we get done with this as soon as possible". I personally believe (and I'm backed by plenty of evidence) that an increase of the efforts regarding quality will also bring speed on the long run, as it will require less of the VERY COSTLY redoing and fixing, that can also undermine the spirit of our engineer team.

If you're starting to ask these questions in your organization: congratulations, you're going through a change that your users will thank, and will produce less churn on your engineering team. But, I'm also really curious about your approach. What is the situation that brought you to start talking about Quality? What are the current solutions that your team is working with? Which are the points are you most struggling with?
