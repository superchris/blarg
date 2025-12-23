---
title: Give your buddy what they need
date: 2025-12-20
description: Your LLM coding buddy needs two things to be successful
---

Your robot coding friend needs two things to be successful: **context** and **feedback**.

**Context** is the one that gets the most press and attention: it just meants giving your LLM enough information that it can actually be useful on your specific problem. You see attempts to improve this everywhere, and LLM tooling has gotten pretty good at dealing with it, at least in the "context" of coding. We all know about the context window at this point and understand the fact that it is a finite resource. Things like Agents.md, CLAUDE.md, library specific llm files, and Claude skills, are all ways to address this issue.

**Feedback** is the thing that gets less press but I kinda think is more important. For me, LLM assisted coding only became useful when I saw the first attempt to address this issue: the "Agent mode" in cursor. It gave my LLM the ability to run commands (eg in a terminal) and have the results of said commands added to it's context window. As a career long TDDist, the very first command I gave it the ability to run was `mix test`. Now my lil buddy could not just write code, but it could use tests the same way I do: to have an early indication of the likelihood of my code being correct. And this also meant it could do what I do: run the test, see it fail, change the code, and iterate until the tests were passing. All of sudden the coding agents, even if mediocre compared to the current best of breed models, went from "interesting but mostly annoying toys" to capable of delivering valuable work.

If you think about it, it's pretty obvious why LLM generated code isn't useful without this. I consider myself to be a pretty top notch meat-based coding agent. And yet, whenever I write code and it happens to work the first time I am surprised to the point of deep skepticism. My instinctual reaction based on decades of experience says "I can't possibly have gotten that right the first time". Writing automated tests, in addition to other possibly even more important benefits, gives me a useful early signal on whether I got it right.

But tests are just one kind of feedback, and they are not enough. At the office, I used to pair with one of my friends and business parters who was so confident in his tests that he would ship code if the tests pass. And most of the time, his stuff worked, but not always. I am on the other hand, either plagued or gifted with self-doubt, and have seen myself multiple times write bugs in both test and implementation code that happen to perfectly offset such that the tests pass and the code is wrong. So I would always insist that we click test the feature even when the tests pass. My co-workers started referring to this as "Superchrisnelson testing". What if our bot buddies could do "superchrisnelson testing" too? Well, with things like the playwright MCP server now they can. We've had some great success with these tools in making the results of automated coding even more robust.

Another kind of feedback human coders often reach for is what you might call "exploratory coding". I don't know enough to even write a test yet, so I might try something out in the REPL of my application (which needs to have one!). Can we grant this power to robots? This is where something like [Tidewave](https://tidewave.ai) comes in. I generally install it in every Elixir/Phoenix application I'm working on. With it, I will often see Claude reach for the tool to try things out the way I would. It definitely adds another level of accuracy.

### You must be this tall to ride this ride.

All of the above are things that many teams can't do right now. There a quite a few prerequisites: some are obvious, some less so. I'll be talking about those in my next post.
