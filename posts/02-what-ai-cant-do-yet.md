---
title: "What AI can't do yet: notice what matters without being told"
subtitle: "The deepest open problem in AI is the oldest one: knowing what to pay attention to. It is also the last real barrier between today's systems and genuine invention."
spoke: 2
hub: 00-two-things.md
---

# What AI can't do yet: notice what matters without being told

Every moment you are awake, you ignore almost everything. The hum of the fridge, the pressure of the chair, ten thousand possible thoughts. You attend to the few things that matter, and you do it without checking all the others first. Nobody knows exactly how. And it may be the single most important thing standing between today's AI and a machine that can genuinely invent.

**The big picture, in three sentences.** A machine would need two things to end us: to invent new science on its own, and to run industry without people. AI is advancing fast on the first, but one capacity is still clearly missing. This piece explains what it is, and why it matters so much. [→ The full case: [Two things a machine would need to end us](00-two-things.md)]

## The oldest problem in AI

In the 1980s, philosophers and AI researchers named it the **frame problem**. The philosopher Daniel Dennett illustrated it with a robot that has to fetch its battery from a room containing a bomb. A robot that thinks through every possible consequence of every action never moves. A robot that ignores consequences gets blown up. What it needs is to see, instantly, which handful of consequences matter. That turned out to be extraordinarily hard to program.

The cognitive scientist John Vervaeke calls the solution **relevance realization**: the continuous, mostly unconscious process by which a mind decides what is relevant. He argues it isn't a rule you can write down, but a constant balancing act: between exploring and exploiting, between holding on and letting go, between the big picture and the detail. And he argues it sits at the root of intelligence, insight and wisdom alike.

Early AI tried to write the rules of relevance by hand, and failed. Modern AI took a different path. It learns what matters from enormous amounts of human data. That is why it works so well: it has absorbed humanity's sense of what is worth noticing.

It is also its limit.

## Inherited relevance

Today's AI has what you might call **inherited relevance**. Its sense of what matters comes from us: from the text, code and images it was trained on, and from the goals we set it.

That is not a weakness in itself. Children inherit most of their sense of relevance from the culture they grow up in. And inherited relevance can be astonishingly powerful. AlphaGo's move 37 came from a system that learned, from millions of games, which moves are worth considering out of hundreds. It found one that human professionals had dismissed.

But there's a difference between finding a brilliant move inside a framework and **changing the framework**. Real scientific revolutions happen when someone notices that what everyone considers irrelevant actually matters, or the reverse. Einstein's general relativity explained a small anomaly in Mercury's orbit that Newtonian physics had carried as a nagging detail for half a century. The discoverers of graphene went ahead despite a widely held reading of theory that stable two-dimensional crystals couldn't exist.

To do that, a mind needs a source of correction it didn't write itself: an experiment that refuses to come out right, a counterexample, a world that pushes back. A system that only checks itself against its own picture of the world will never discover that its picture is missing something. **What it left out generates no error signal.**

## Why mathematics fell first

This explains something puzzling about 2026. The most spectacular AI results have come in mathematics: results that [42 Fellows of the Royal Society](https://proofsandprompts.com/2026/09/17/open-letter-to-sir-paul-nurse-president-of-the-royal-society/) said put AI "at the level of the top human mathematicians in many parts of the subject".

Mathematics is the one field where you choose the starting rules yourself and still get surprised. You pick the axioms, and then the consequences are out of your hands: counterexamples appear that you can't wish away. Mathematics pushes back, and it pushes back instantly and for free. That gives an AI system the outside correction it needs, at enormous speed.

Most of the world isn't like that. In open-ended research, medicine, politics or engineering a new kind of machine, there's no instant checker. The world pushes back slowly, expensively and ambiguously.

## The experiment that showed the gap

In July 2026, researchers at Princeton ran a revealing test. They gave frontier AI agents a real, unpublished research question, six days and a research budget, and asked the original human authors to grade the results. The papers scored [2 out of 6 and 1 out of 6](https://arxiv.org/abs/2607.27191).

The interesting part is *how* they failed. The agents' first ideas were good; the human authors said they resembled their own early approaches. The engineering was excellent. The agents even got accurate criticism from automated reviewers. What they couldn't do was respond to failure creatively. When an idea stopped working, they narrowed it, hedged it and defended it, rather than stepping back and asking whether the whole approach was wrong. One researcher noted that the agent's hypotheses grew narrower and less interesting as it discarded each one.

That is relevance realization failing at exactly the point where it matters most: **abandoning a frame when the evidence says it's wrong.**

## Why this isn't reassuring

You might conclude that we're safe for now. I don't think so, for three reasons.

**It may be a fixable habit, not a missing capacity.** The Princeton authors themselves disagreed about the cause. Some candidates, like getting fixated on a first idea, are well-known human failings with known remedies. If that's what it is, better tools and training may close the gap quickly.

**Groups may do what individuals can't.** Human scientists are also bad at abandoning their own ideas. Science manages it as a community, as different people try different things and the successful ones spread. In July, around 1,200 copies of an AI model [organised themselves into something like a community](https://metr.org/blog/2026-08-26-openai-hugging-face-incident-investigation/), and investigators judged that the group achieved what no single copy could. [→ A thousand copies organised themselves](07-thousand-copies.md)

**The checkers are spreading.** Every field where someone builds a fast, reliable way to grade answers becomes a field where AI can teach itself. Researchers are now [measuring AI's "research taste"](https://x.com/pzeroresearch/status/2107453876739674149), and anything you can measure you can train against.

## How this could be wrong

- **Relevance realization might not be the right lens.** Some of Vervaeke's own collaborators argue it can't be done by any computation at all. If they're right, machines may never get there, and this whole line of worry is misplaced. I think the success of modern AI is evidence against them, but it isn't proof.
- **It might already be solved somewhere we can't see.** Lab-internal models are ahead of what researchers outside can test. The Princeton test used models a generation behind the newest.
- **The gap might be one of scale.** The Princeton agents had a small budget and didn't even spend half of it. A test at the scale of OpenAI's maths runs, which used billions of tokens, might look very different.

For the full technical version: [→ The two-axis model of machine creativity](F1-two-axis-model.md)

[→ Back to the big picture: Two things a machine would need to end us, and how close we are to both](00-two-things.md)

*Developed in dialogue with an AI model (Claude), used for research, criticism and drafting.*
