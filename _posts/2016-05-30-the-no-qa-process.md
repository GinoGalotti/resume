---
layout: post
title: The no-QA way
date: 2016-05-30 18:50
author: Gino Galotti
categories: [Quality Assistance, Testing]
---
We're still finding out sweet spot regarding Quality and there are always some developers that think no "formal tester" is needed in our process right now. This approach even gains more followers [when you have an ex-Facebook in your team](http://www.zdnet.com/article/why-facebook-doesnt-have-or-need-testers/).

Don't get me wrong, I never take the bait to jump yelling "You NEED me, this will be a MESS without me!", mainly because I think this approach is as valid as any other if you focus on the right things, and meet some conditions. And I really enjoy discussing testing, especially when it allows me to understand my peers' point of view.

So we started a conversation, but it didn't lead to anything because we were just pointing the pointless parts of our current process, instead of really talking about how to make it work. Afterwards, I schedule some time on my calendar to sit in one of the meetings rooms and use the Whiteboard to clear my ideas. _Would it be possible? What are we missing to get there? What would it offer us? How would it impact our team and process? Which are other solutions?_

Then I felt way more ready to have that conversation again, but I decide it will improve with a broader audience, and sharing the questions in advance so everyone's is better prepared. And, this time, I really enjoyed the chat. We still complained about what is currently failing, but we managed to come with tentative solutions. As well as some answers to the previous questions.

Let's start with motivation. _What would it offer us?_ The answer was almost unanimous: less friction in the process. As developers will be more autonomous and the QA layer is not going to be annoying, coders can focus on the code. It also carries some challenges, but we'll talk about them later on. The goal is having a simpler and smoother process, and also, you don't have to spend on QA itself. Win / win situation!

But, obviously, there are some requirements to get there. So, _what are we missing to get there?_ First and more important, by far, is the culture of owning quality. If there won't be a "quality gatekeeper", everyone should be responsible for their deliverables quality as well as ensuring that everyone's working on it. We've been moving towards that (as well as [most of  the Agile testing approaches](https://callmegino.wordpress.com/2016/04/03/meet-quality-assistance/)), but we're not there yet and it's really needed making this huge step.

This is especially tricky when you think about testing the "big picture". It's quite straight forward that when you deliver your solution, it should contain unit and functional automated tests verifying its behaviour. Hopefully, you have a culture regarding integration and component testing as well. But what about ensuring that the application works as a whole? Who will be responsible for that? Who will create, maintain and run those tests? What about the strange and complex cases that are almost impossible to automate? When and who should explore it?

One of the huge differences between the Facebook and our case is the amount of dogfooding that they do. We don't have beta users, we don't do canary releases, we don't even use our tool that much internally. That's one of the biggest challenges that we'd need to solve before taking this approach. It can be done, things like getting used to exploratory testing the application after when the development is done, but no developer is used to do it. One of the reasons why Quality Assistance keeps a testing expert available for the team is to help in this transition.

Then... _how would it impact our team and process?_ Well, spreading out the responsibility about quality need some process changes, like defining some steps or techniques to review the solutions in pairs, not only reviewing the code and the tests. Get some understanding of the application that we're building, and we need to play with it if we want to verify the changes. We'll need more involvement with the product in order to find dependencies and better testable solutions from the beginning, although it will improve after the team gets better knowledge about it.

So, _would it be possible?_ Well, one of the Agile principles I TRULY believe and share is "Fail fast, fail often". As long as we timebox the try, set some retrospective meetings and are aware of the potential impacts; I think is stupid to answer the question instead of trying it out for a while, analysing and understanding the outcome afterwards. For sure, the first version won't be the good one, but will teach us some tricks for the next one.

And _which are the other solutions?_ I'm still keen on giving it a go, so it helps us identify what are we missing from the current approach and what we love from the change. But it's always good keeping other solutions in mind. We can always go back to the old model of a QA wall where we throw everything, having someone to help us embracing quality and building tools to aim us (Quality Assistance), heavily invest in automation, or whatever pop your mind that might work.

There are thousands of different approaches to find Quality at Agile speed, and none of them works flawlessly. They neither work in every organisation. And I know a thing for sure: spending time and resources on finding a sweet spot for your process is always a good investment. Period.

Do you have experiences with a non-QA environment? I'd love to hear them!