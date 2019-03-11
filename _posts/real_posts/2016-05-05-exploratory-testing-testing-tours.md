---
layout: post
title: Exploratory testing: Testing tours
date: 2016-05-05 19:59
author: Gino Galotti
categories: [Exploratory Testing, Testing]
---
I've been talking about exploratory testing for a while now (either about [Rapid Software Testing](https://callmegino.wordpress.com/2016/03/24/meet-rapid-software-testing/) or [Quality Assistance](https://callmegino.wordpress.com/2016/04/03/meet-quality-assistance/)). I like to focus in this series on some testing techniques that I've learnt from the Exploratory world, although they can be applied to any testing practice. In this particular case, we're going to describe some Testing tours.

Testing tours are guidelines and examples to follow when approaching a new testing challenge. They help to identify where should the focus be, and highlight components highly automatable as well. They're well described by James Whittaker in [Exploratory Software Testing](http://www.amazon.co.uk/Exploratory-Software-Testing-Tricks-Techniques/dp/0321636414) and [How Google Tests Software](http://www.amazon.co.uk/Google-Tests-Software-James-Whittaker/dp/0321803027/ref=sr_1_1?s=books&amp;ie=UTF8&amp;qid=1460113934&amp;sr=1-1&amp;keywords=how+google+test). Let's example some of the tours now!

## Demo tour. 
Find what's going to be showcased, which are the biggest selling points and verify them. If that's where the money is, spend more time polishing it. View the tests from the perspective of the sales staff. Are you able to easily show the functions of the application? Does the application execute as described by the literature?

A variation of this tour is called the Skeptical Customer tour in which the tester would get in the mind of a customer asking a lot of questions about what is being demoed. This tour should test the answers of questions such as "what if we did this?" or "how about if I want to do that?" Imagine the customer that will want to prove that the demo is marketing spin. What kind of questions would be asked?

## Landmark tour. 
Identify the components of the system, the functionalities of every component and the capabilities (or actions) or every functionality. Having that list, you can check the transition between states (and empower automation). This list must be prioritised, and development should be involved to complete it. A nice trick is to share with the team the priorities, everyone would detail the list in order to get their work prioritised. Keep in mind that navigation is important as well (different links to reach the same page, keyboard shortcuts, etc.).

Intellectual tour. In this tour, the tester needs to be asking the hardest questions. What is the most complicated function that can be executed? Test the limits. What inputs would cause the most processing? Which queries would be the most complex? Execute the functions of the power user.
    
## Fedex tour. 

Find the points where data gets modified or passed by, and focus on them. Add verifications around those boundaries. Things like: where the data gets displayed, localised, formatted, extended, etc.

##After-hours tour. 
Focus on the maintenance tasks. Backups, cleaning, garbage collector. Check that the environment is clean after running those, and their task is being accomplished.
    
A variation of this is the Morning-Commute tour where the tester focuses on starting up the application and the initial state of the system.

## The garbage collector tour. 
Like a guy collecting trash, the tester runs the same operation for all the neighbours (menu items, tabs, etc.). It's not testing exhaustively, but checking that everything is in the place, and there are no obvious issues.

You can find more specific tours in the mentioned books, as well as lot of literature about [which's the best tour](http://kaner.com/?p=96), [keynotes from testing mesias](http://www.developsense.com/blog/2009/04/of-testing-tours-and-dashboards/), or [implementation examples (in this case, from Google)](http://googletesting.blogspot.co.uk/2009/10/fedex-tour.html). Have you applied any of these tours personally?
