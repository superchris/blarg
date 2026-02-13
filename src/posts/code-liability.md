---
title: Every Line of Code is a Liability
date: 2026-02-12
description: We've know this forever, but now we can measure it.
---

In the very bad old days of software development one of the worst practices ever to come along was to measure a developer by the lines of code they produced. Yet, here we are in the age AI going "lookie! My agent just wrote 100k lines of code!" as if that were a good thing. And it may be: the problem is that we are measuring the wrong thing. What we actually care about is the valuable features the software (hopefully) contains. This of course is notoriously hard to measure, so lazy and terrible managers sometimes tried to use LOC as a proxy for it. And it's just as bad of an idea today!

The reality is that each LOC is not an asset, but a liability. The simple reason for this is that we coding agents (meat based and silicon based) spend way more time reading code than writing it. This means that when we are able to deliver software with the same functionality for less code, we get that benefit not just just once (1x) when we write it, but many times: nx where n is the number of times we need to read the code. And n turns out to a very large number. 

We've known this for a long time in software development, but since "harder to read code" was subjective and impossible to measure it was possible to ignore. This is no longer true. Meat based and silicon based coding agents have a finite amount of space to fill with information about a task, and now we have a name for it: the Context Window. And with silicon based coding agents we can literally watch it fill up.

# Language Choice Matters

At Launch Scout, we've been a fan of languages that let us clearly express our intent with as little code as possible for a long time. This led us to Ruby in our early days, and more recently to Elixir. We have always optimized for maximum developer productivity and we were well aware of our extremely finite meat context windows, even before we had the right words to describe them.

And frankly, we've gotten a lot of push back for it. Many prospective clients balked at the thought of doing something different from what the "industry leaders" seemed to be doing. We have deliberately gone against the mainstream because mainstream development practices are optimized for a different thing than we chose to optimize for. "What are they optimized for?", you might ask...

# Our industry is optimized for large team delivery

Most of the current "industry leading" practices come out of trying to imitate the practices of FAANG. And these guys, of course, have Very Large Teams doing (presumably) Very Large Things. In order to do this, you need to be able to build a system with not just multiple developers, but multiple teams of developers. You need to have everyone choose from a limited set of technologies so you can hire easily and bring new developers up to speed easily. You need practices that allow you coordinate the work across multiple teams with a minimum of chaos.

The reality though, is that no matter what you do or how hard you try, software development has the opposite of economy of scale. The more developers you have working on a system, the less productive each one is. Ask almost any experienced developer and they will agree this is an inviolate law. Decisions made by one developer affect and have to be understood by other developers. Decisions made by own team affect and have to be understood by other teams. And now we have multiplication working against us, not for us. At Launch Scout, we've been a fan of the "small and mighty team" for a long time for exactly this reason.

# Where is all this going?

I do not have any words to describe the level of change going on in the software development industry caused by AI being increasingly effective at writing code. This is an extremely recent development, with truly effective coding agents being maybe a year old. Our industry has not yet had time to react and we are very much still figuring it out. However, I think we can make a solid case that it is time to optimize for different things. It has never been possible for a small team to accomplish so much. We may very well be headed for a world where large team software development is obsolete. It is worth reconsidering everything we are doing with that in mind.