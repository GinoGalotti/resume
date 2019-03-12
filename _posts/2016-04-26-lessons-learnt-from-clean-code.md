---
layout: post
title: Lessons learnt from Clean Code
date: 2016-04-26 21:17
author: Gino Galotti
style: fill
tags: [Books, Personal lessons, Testing]
---
Before start talking about how [Clean Code:A Handbook of Agile Software Craftsmanship by Robert C. Martin (Uncle Bob)](http://www.amazon.co.uk/Clean-Code-Handbook-Software-Craftsmanship/dp/0132350882) affected me, I want to start recommending this book. It's well known inside the Software Development industry and, even if you don't see eye to eye with Uncle Bob, it has really good reflexion about how to structure your code. I was lucky that during my career I joined a company where reading this book was part of your first-year commitments, and we use it a lot while code reviewing as a common ground for arguments. But now, let's focus on what I learnt reading this book!

Being able to solve complex problems is not what defines a professional software developer. It's absolutely a good skill and, at some point, you're going to need analytical thinking and problem-solving abilities but a professional developer also focuses on the readability of the code as well and building scalable, maintainable and simple solutions.

This book made me realise that wording, naming and modularizing the code are more important than I thought to start my career. I started to spend some time finding the best variable, method and class names, for example.

Learn how to better use hierarchy. I've been working with object oriented languages during the majority of my professional life, and learning how to master this powerful tool makes a huge difference.

Refactoring to achieve readable code usually takes longer than coding the solution itself. It's a good practice to just focus on getting the job done, and then start iteratively refactoring until the code is readable enough.

[Always leave the campground cleaner than you found it.](http://programmer.97things.oreilly.com/wiki/index.php/The_Boy_Scout_Rule)

Having a guideline during code reviews make them less harsh. When a clash happens, you can use the book to specify why a change should be done, instead of just using your "I know better than you" argument.

Professional programmers care about testing. Mr. Martin thinks that TDD is the only way for a professional programmer because no code is complete without enough testing verifying that it works.

I should not abuse commenting. During my degree, teachers told me that I have to comment as much as possible to achieve a readable code. Then, you discover that no one updates the comments when refactoring, so it ends like a misleading piece of information. Instead, if you focus on a readable code per se, and you forbid yourself to comment; you'll build an understandable solution that doesn't require them. And, for documentation, nothing explains better than an extensive testing suite. And if you don't update them... they'll break!

Programming literature can teach me more than I thought. I assumed that every you have to learn from coding is online, and books are outdated and useless by definition. How wrong I was. After reading this, I picked books about Testing, Programming, and Design patterns. And, without any doubt, my code got better after doing so!

Here was the first time I heard about principles like [Don't repeat yourself](https://en.wikipedia.org/wiki/Don%27t_repeat_yourself), [Keep it simple stupid](https://en.wikipedia.org/wiki/KISS_principle), [You aren't gotta need it](https://en.wikipedia.org/wiki/You_aren%27t_gonna_need_it). And I realised how little I was following them!

Those are some of the lessons I learnt reading this enlightening book. In a future post, I'd love to talk about what I learnt from [Clean Coder:A Code of Conduct for Professional Programmers (Robert C. Martin)](http://www.amazon.co.uk/Clean-Coder-The-Professional-Programmers/dp/0137081073), part of the same series but focusing on the relationships between software professionals.