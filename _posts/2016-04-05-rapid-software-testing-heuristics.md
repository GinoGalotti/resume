---
layout: post
title: Rapid Software Testing - Heuristics
date: 2016-04-05 14:59
author: Gino Galotti
style: fill
tags: [Exploratory Testing, Rapid Software Testing, Testing]
---
As [I mentioned before]({{ site.baseurl }}{% post_url 2016-03-24-meet-rapid-software-testing %}), Rapid Software Testing is a testing methodology defined by James Bach, Michael Bolton, and Paul Holland. This methodology focuses on the skillset and experience of the tester alongside with some rules and techniques to achieve a cost efficient quality assessment of a product.

This post will only focus on the Heuristics proposed by the methodology as a guideline for Exploratory Testing sessions although I've been using them as a source of inspiration for testing purposes. You can find the [original document among other RST appendices](http://www.satisfice.com/rst-appendices.pdf). Let's start the show!

I agree with RST approach that Testing is a context-driven activity, so you shouldn't expect a cookbook explaining you step by step what you have to test. These represent "general techniques" which are generic enough to be relevant for a wide spectrum of contexts. Personally, these examples have helped me defining specific heuristics for a given product. These are the groups of test heuristics with some examples:

**Functional testing**. Determine the things the product can do, or this feature can offer. See that each function does what it's supposed to do, and no what isn't.

- C'mon, you're used to this testing! You don't need help thinking about how to test functionality, do you?

**Claims testing**. Challenge every claim you find about the product (either explicit and implicit). Test the veracity and clarity of the claims.

* Read the specification, is the product align with it?
* Is the manual relevant to the current version of the product?
* Are the descriptions, onboarding tips and help statements inside the product aligned with it?

**Domain testing**. Segment the data the product can process into tiers (invalid values, boundary values, best representatives, etc.). Consider combinations of data.

* Is that numerical operation running the same logic with positive, negative or colossally long numbers?
* Is the producing recognizing the language that String is using?
* Does the product process differently Geo points from different countries?

**User testing**. Learn about user roles and categories, determining what are the differences in their needs and permissions.  Get real user data and involve the users (from different categories) in the test (or learn how to simulate one).

* Is the "techie loner" persona  part of our user base?
* Are we testing the admin side of the product?

**Stress testing**. Look for part of the product vulnerable to being overloaded, and generate challenging data to test its limits.

* Extend the usage for a very long period of time with a steady load, or maybe try with peaks.
* Test the limits on the input and output of our product.
* Check concurrency is being handled correctly with some more data than the expected one.

**Risk testing**. Imagine a problem, then look for it. Focus on the kind of problems matters most. How would you detect problems? Your experience and knowledge about the product and the team will shine here!

* Distributed applications struggle with concurrence. Exploit it!
* Transactions have to deal with consistency. Exploit it!
* This team has been failing to deliver cross-browser solutions, focus on it!

**Flow testing**. Perform multiple activities connected, don't reset the system between user paths and vary timing and sequencing.

* Run overlapped actions in a parallel way.
* Verify that the product transits correctly between states, even on the non-happy sequences.

**Scenario testing**. Tell a compelling story. Design tests that involve meaningful and complex interactions with the product.

* Reflect a scenario simulating someone who matters doing something that matters.
* Think about the different applications of the product and how the scenarios would differ.

**Automatic checking**. Check a million different facts, hopefully getting coverage in the process and using oracles. Tools that empower the tester are always welcomed!

* Automatic change detectors. Catch those regressions!
* Automatic data generators. Help the tester with the easily automatable parts of the job.
* Check permutations and combinations easily.
* [Tools that support the tester](http://www.satisfice.com/articles/agileauto-paper.pdf).

In my experience, this is an amazing starting point when you face a new product. These heuristic rapidly evolve into context-customized during your first exploratory testing session, serving as a baseline for the next ones.

I have to admit that the main reason to write this post is serving as documentation to me, as well as helping me interiorise it. But I hope you find it useful as well!

