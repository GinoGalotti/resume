---
layout: post
title: Quality Assistance - Lessons learned
date: 2016-04-26 22:52
author: Gino Galotti
style: fill
tags: [Personal lessons, Quality Assistance, Testing]
---
<p style="text-align:justify;">This morning, [during my 10 idea routine,](https://callmegino.wordpress.com/2016/03/31/becoming-an-idea-machine/) I push myself to list techniques and activities that I've tried to change the Quality mindset around the company. You already know that we've been doing modelling some of the process following the [Quality Assistance](https://callmegino.wordpress.com/2016/04/03/meet-quality-assistance/) approach. I know that the outcome of these activities will drastically vary for each team, but hopefully knowing some experiences will help you try something similar. And, [as Scott Berkun explained amazingly here](https://youtu.be/amt3ag2BaKc), it's more important to learn from the failures than to just share the final idea. And certainly writing this will help me remember some details. I don't trust my memory that much...

I'll try to give you as much background as possible, although reading about how the organisation is working now and how I'm facing it know may help. Now.. Let's focus on some things I've tried!

[**Three amigos**](http://www.velocitypartners.net/blog/2014/02/11/the-3-amigos-in-agile-teams/). This is a pretty standard activity, although we needed some twist mainly because of resource issues (just me as QA and one product owner). We started picking some complex tasks per sprint and trying a standard Three Amigos, although at some point we decided that the engineers should do the exercise of listing the scenarios before implementing a solution, leveraging our work to double check and enhance with some "edgy but important" ones.

**QA demo**. We do it after finishing the development of some sprint stories where me (or Product) showed in 10 minutes at their machine how users are most likely to run through it, as well as trying to break it. There's no better way to understand how to test than looking someone testing (and trying you communicate the mental process). There are some developers that, after this, embraced some testing activities as they saw me enjoying it, although others are reluctant.

**Defining metrics to understand the current status**. Things like amount of errors in each version, times, grouping types of errors, clearing non-useful data or even finding ways to generate it (like replicating production load on testing environments). We're all engineers here, and no matter how much you try: data wins discussions. That's a fact. I don't have any data to back it, but you have to believe me.

**Testing hour**. I can't think that I have too much time to run many experiments, but one of the activities I love doing is setting voluntary exploratory testing sessions. I've done it mainly for big new releases, and I try to guide them to focus on a different aspect each time, although it gets wild most of the times. Unfortunately, we don't do enough dogfooding, so this activity helps a lot spreading the knowledge about the tool and getting feedback. In my experience, teams that are usually siloed and less involved with the products are the ones enjoying it more, and giving you fresh feedback (RnD, Ops, etc.).

**Getting involve with the community**. We're quite small, and I love allocating some time helping out the customer support guys giving not technical answers in the "I think I found a bug" section of our forum. It gives me loads of insight about what they care about, and some valuable examples to back my feedback. And they actually find some really weird bugs!

**Proactively spying production**. Gathering metrics, we've come around with some filters to get weird errors and behaviours, and we can use our tool to understand how the a user can get there. We've found edgy bugs because of it. We also use Inspectlet to understand how the users react to new features, helping us understanding further user cases and finding strange behaviours!

**Participate in technical design meetings**. I'm used to joining product meetings to help define some new features or make the product more resilient, but being involved in the technical discussion gives me more insight into the implementation and the challenges, and allow me to raise issues to ensure a more testable product (backdoors to easily reach some states, ways to inject failures, etc.)

**Big picture testing**. That every developer should care about testing it own slice is a fact, particularly in an organisation where there is only a QA. But testing integrations and "end to end" is usually something tedious that no one wants to deal with, but having a smoke verification before and after every release brings A LOT of value. That's why I've taken the responsibility of building a "simple scenarios" big picture testing suite for both backend and frontend, serving me as valuable documentation as well. It's the green light everyone needs before rolling a change.

**Reviewing code** (particularly tests). I wish I had more time to review more bits of code, but I usually just check some of the new stuff who I haven't understand yet; and the code for the functional tests, especially the first batch of tests for a new feature. My main concern are readability, scalability and detecting flakiness. Avoiding integrations when possible (using static versions of webs vs live version), some random waits, retries policy that would masquerade problems, modularize for reusability...

**Pair whenever possible**. Ok, after all of this, I know I don't have much time left. But, when I have, my first list is pairing as much as possible. It teaches me new technologies and ways to develop, I get some understanding about the solution, I can give early feedback and it bonds me with my colleagues. I'll make a post about the benefits (and cons) I see in pairing soon!

And this, guys, are some activities I'm trying to infect the team with the love about Quality. Some of them may end as worthless, and many will be evolved and change, but right now I'm learning something new every time I do them. That sounds like enough reason to keep them for me!