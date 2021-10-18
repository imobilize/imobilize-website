---
title: "WHY TDD?"
date: 2015-04-28T12:14:34+06:00
author: "GENADI TODOROV"
image: "images/blog/Test-First.jpg"
tags: ["tdd", "testing"]
description: "This is meta description."
draft: false
---

The question I would like to ask you is not do you write your tests first or last but rather do you write tests at all? Every professional developer knows that they should write tests for their code. But in fact, few do. If you ask someone why they skip writing tests, the answer would be “I’m in too much of a hurry” or “It takes too much time to write tests”. But the bigger problem is that this can quickly become a vicious circle – the more pressure you feel because of the time, the fewer tests you write. The fewer tests you write the less stable your code becomes. The less stable your code becomes, the more pressure you feel.

In my experience, having used test-driven development (TDD) and also developed without tests thinking my code will just work (naive-driven development) I have been given enough reasons to always write tests. With all the tests in place, I feel confident that my code works and I am not afraid to come later and refactor or optimize it. Writing tests increases the level of quality of software. Everyone knows that when it comes to a choice between the features, time and quality, it’s always the quality that suffers.

**So what is TDD?**

Test-driven development is a process where you write a test before you write the actual code. It relies on a repetition of a short development cycle where the developer first writes a test which initially fails because there is no actual implementation and then he writes just enough production code to fulfill that test. The code written at that stage may not be perfect because the only purpose of it is to pass the test. After that if the test passes the code must be cleaned up. Which leads to the primary goal of TDD –  write clean code that works.

TDD completely turned around my understanding of software development. When you start implementing a new feature, the first question a developer should ask is if the design is the best possible to enable you to implement the new functionality. If so even better, you proceed. If not, you can refactor it to change the part of the design affected by the new feature, enabling you to add that feature as easily as possible. As a result you will always be improving the quality of your design.

Another benefit of using TDD is that your code will have fewer defects. These will still happen but as your practice of TDD matures these types of defects will occur less often. When you find a bug or defect the first thing you do is to write a new test that exposes the defect. From there you can continue following the normal TDD workflow – write just enough code to make the test pass and keep the existing tests passing. Once this is done, assuming you’re correctly testing the condition that produces the defect, it should not return in the future.

The practice of TDD results in writing the simplest code to pass the test. This code tends to be shorter and less complex than code developed by someone not practising TDD. We all know that shorter and less complex code is higher quality code. It is also more readable and understandable which enhances its maintainability. The code tends to be more focused on performing the task, keeping irrelevant functionality out of the picture.

One of the things that made me really happy when doing TDD is that I am proud of my code. And even if it is not that good I can always return and refactor it without fear of breaking something. Writing tests helps me a lot with improving my design. In the past I thought that my code was clean and well written until I started writing tests for it. At that moment I realised how awful my code was. My function were doing more than one thing, I was using a lot of utility classes and most of them were tightly coupled. Tests helped me realise that, they helped me to improve my “well-written” code.

Something more, previously I was proud of my debugging skills. Now I think I spent too much time doing that. I feel embarrassed when I help someone debug their code. Instead of that you can spend twice less time writing tests and you will end with something which I called the magical button which when pressed tells you if your code works or not. And even more it will tell you exactly where your logic is wrong without the need to trace it.

A common complaint about TDD that I hear is that it slows development. This is both true and false. Writing the tests before you write the code can add additional effort to the task because of the time you will need to write tests, that is true. But that time is not wasted. In my experience, this leads to better code the first time and less re-writing after that. When you think you are done with a task and you have to spend time debugging faulty code, this additional effort soon adds up to being something much longer than writing a test in the first place. Not to mention the time taken to fix bugs from changing this code in the future. It very quickly becomes false that TDD slows development. TDD helps you to realise when to stop coding. Tests give you confidence that you have done enough and you can stop tweaking and move on to the next task. They give you instant feedback (I like the feeling when I see the green light). It’s also much easier and faster to pick up where you left off after an interruption because you can see where you got to (that is the next red light that needs fixing).

And finally I feel like I’ve learned a lot about testing and TDD but I don’t consider myself as knowing everything. I’m still discovering how to make it work better. Also I don’t pretend that there aren’t alternative ways that might work as well. But in my experience it is the best thing that I have found so far and I will be even happier to leave it for any practice that works better.
