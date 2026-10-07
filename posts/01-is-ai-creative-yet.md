---
title: "Is AI creative yet? Two people asking that are usually measuring different things"
subtitle: "AI creativity has two dimensions, not one. Mixing them up is why the argument never ends, and why we keep missing where the danger is."
spoke: 1
hub: 00-two-things.md
---

# Is AI creative yet? Two people asking that are usually measuring different things

Ask a room whether AI is creative and you'll get a fight. One person points at a model that writes poems, code, business plans and bedtime stories on demand. Another says none of it is really new, just a remix of what humans already made. They are both right, because they are talking about different things.

**The big picture, in three sentences.** A machine would need two things to end us: to invent genuinely new science on its own, and to run industry without people. This piece is about the first of those, and about a simple way of measuring how close AI is to it. [→ The full case: [Two things a machine would need to end us](00-two-things.md)]

## Two questions hiding inside one

"Is AI creative?" is really two questions.

**How wide?** How many different fields can a system work in? A chess engine works in one. A modern language model works in almost every field humans write about. Call this **reach**.

**How deep?** Can the system only find clever moves inside the rules it was given, or can it change what counts as important? Can it notice that the way everyone frames a problem is wrong, and reframe it? Call this **depth**.

These are independent. A system can be very wide and very shallow, or very deep in one narrow field. Put them on two axes and you get a map.

![Figure 1](../figures/fig1-two-axes.png)

*The map. Reach runs left to right, from narrow to general. Depth runs bottom to top, from limited to paradigmatic. The colour shows distance from the top-right corner, where a system would be both deeply inventive and broadly capable.*

The word "paradigmatic" comes from the historian of science Thomas Kuhn. Most science, he argued, is puzzle-solving inside an accepted framework. Every so often the framework itself is replaced: Newton by Einstein, a fixed Earth by plate tectonics. Those replacements are what he called paradigm shifts. Depth, on this map, is the capacity to make that kind of move.

## The four corners

- **Bottom left: limited and narrow.** Clever within one field and its existing rules. A chess engine, or David Cope's 1990s program EMI, which composed music in Bach's style convincingly enough that an audience took it for the real thing.
- **Top left: paradigmatic and narrow.** Changes how experts see one field. AlphaGo's famous move 37 against Lee Sedol in 2016 looked like a mistake to professionals and turned out to change how humans play Go.
- **Bottom right: limited and general.** Competent across almost everything, but rarely deeper than the best existing human ideas. This is where large language models arrived in 2022–23.
- **Top right: paradigmatic and general.** Able to reframe problems in many fields at once. Nothing is there yet.

## Why the top-right corner is the dangerous one

Every safety measure we have works by imagining what a system might do and preparing for it. Safety tests, red teams, monitoring, kill switches: all of them depend on our picture of the possibilities.

That works against a system that is merely strong. A very strong chess engine is still playing chess. It fails against a system that can change the game: one that sees a problem in a way none of its overseers imagined. And it fails worst when that system can do so in many fields at once, because then there are many directions in which the surprise can come.

That is why the danger grows towards the top-right corner. It is also why the band of colour curves down before the corner: a system doesn't need to be inventive in literally everything. Software alone touches almost every part of modern life.

## Where AI is now

Here are the main data points, plotted as of October 2026.

![Figure 2](../figures/fig4-anchors-2026-10.png)

*Anchors as of October 2026. Placements are judgement, not measurement.*

The pattern is striking. For 30 years AI has been spreading to the right, from one game to many games to almost every field, while getting deeper in each. In 2026 the points rose sharply:

- In September, mathematicians working with AI, and separately OpenAI, produced [proofs about fluid equations](https://cims.nyu.edu/~tristanb/statement.pdf) of a kind the official Millennium Prize problem statement accepts.
- In October, OpenAI published [722 mathematical manuscripts](https://openai.com/index/sharing-ai-progress-in-mathematics/) from one internal model, across more fields than any human mathematician has worked in.
- AI-driven security research found flaws that millions of automated tests had missed.

But notice what hasn't happened. In every case, humans still chose the problems. And every one of these fields has a cheap way of checking answers: a proof checks out, an exploit works, a test passes. When researchers at Princeton gave AI agents a genuinely open research question with no such checker, the agents [did the engineering well and still failed](https://arxiv.org/abs/2607.27191): when their first idea didn't work, they couldn't let go of it and try something fundamentally different.

That is the clearest thing still missing. No AI has reached the corner yet, and it is a lot less far away than it was a year ago. One human arguably did: John von Neumann, who did field-changing work in logic, quantum mechanics, game theory and computing. Humanity coped with one von Neumann. An AI that reached the same point could be copied a million times, what Anthropic's chief executive has called "a country of geniuses in a datacenter".

## So: is AI creative yet?

Yes, widely, and increasingly deeply inside fields where answers can be checked. Not yet in the way that matters most: choosing its own problems, and abandoning a frame that has failed.

Asking "is it creative?" is like asking "is it big?" without saying whether you mean tall or wide. The useful question is where on the map a system sits, and how fast it is moving. On both counts the answer this year is: closer, and faster, than almost anyone expected.

## How this could be wrong

- **The placements are judgement.** Nobody yet has an agreed way to measure depth. The map is partly an argument that we need one.
- **"Paradigmatic" may not be a real threshold.** The cognitive scientist Geraint Wiggins showed that changing the rules can itself be described as searching a bigger space of rules. If so, depth might be a smooth slope with no steep part. I think the danger rises steeply anyway, but that is an argument, not a measurement.
- **Volume might substitute for depth.** If enough attempts in a field with a good checker can find anything a deep thinker would, then the corner matters less than I claim, and the danger is already nearer.

For the full technical version, with the mechanism and the research behind it: [→ The two-axis model of machine creativity](F1-two-axis-model.md)

[→ Back to the big picture: Two things a machine would need to end us, and how close we are to both](00-two-things.md)

*Developed in dialogue with an AI model (Claude), used for research, criticism and drafting.*
