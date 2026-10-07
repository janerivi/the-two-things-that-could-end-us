---
title: "An experiment that would tell us if it's ever safe to resume"
subtitle: "We argue about whether AI can make genuine breakthroughs. We could test it, by hiding a breakthrough and seeing if the machine finds it."
spoke: 10
hub: 00-two-things.md
---

# An experiment that would tell us if it's ever safe to resume

Imagine taking a modern AI system and carefully removing graphene from everything it ever learned. No papers, no textbooks, no news stories. Then you give it what physicists knew in 2003: a century of graphite research, and a theory widely read as saying stable two-dimensional crystals were impossible. Does it question the theory? Does it propose the experiment? Does it find graphene?

**The big picture, in three sentences.** A machine would need two things to end us: to invent new science on its own, and to run industry without people. I argue for halting frontier AI development now, before the first capability arrives. A halt needs a way to know whether, and when, it is ever safe to continue, and this piece proposes one. [→ The full case: [Two things a machine would need to end us](00-two-things.md)]

## The question nobody can currently answer

The central question in this series is whether AI can do more than find clever moves inside a framework. Can it change the framework itself, the way real scientific revolutions do? [→ Is AI creative yet?](01-is-ai-creative-yet.md)

Right now that question is argued, not measured. Optimists point at spectacular maths results. Sceptics point out that humans chose the problems and that maths comes with a built-in checker. Both have a point, and neither can prove the other wrong, because we have no test designed to tell the difference.

## The design: hide a breakthrough

The idea is simple to state.

1. **Pick a real breakthrough** where an established belief was overturned, and where the clue that should have prompted it was already available beforehand.
2. **Remove it** from the system's training data, along with everything that followed from it.
3. **Give the system the clue**, the anomaly that historically provoked the breakthrough, but not the question it eventually led to.
4. **See whether it revises the framework** in a way that resolves the anomaly.

The system being tested is the whole package: the model plus its tools, memory and scaffolding, ideally after it has been running and accumulating experience for a while. A freshly started system is the weakest version it will ever be.

## Good targets

Recent science offers good candidates, because the corpus is large but the history is still manageable:

- **Graphene (2004).** Graphite had been studied for a century; a common reading of theory said a stable 2D crystal couldn't exist.
- **The brain's lymphatic vessels (2015).** Textbooks said the brain had no lymphatic system. Hints from immune traffic and fluid clearance were already in the literature.
- **CRISPR as bacterial immunity (2005–07).** Strange repeated sequences matching viral DNA sat in public databases for years before anyone saw what they meant.
- **Topological insulators (2005–07).** A new kind of matter that didn't fit the accepted way of classifying phases.

The first two are the best starting points, because each had an explicit belief on record that blocked the discovery. You can check directly whether the system notices and rejects it.

One target is especially important: **the transformer**, the architecture behind today's AI. Asking a system to reinvent it from the state of the field in 2016 tests exactly the capability that matters most for AI improving itself.

## Making the result mean something

Three design rules matter.

**Controls.** For every hidden breakthrough, include a discovery from the same period that *didn't* require overturning anything. If the system fails both, it simply isn't capable enough, and the failure tells us nothing about invention.

**Don't leak the answer.** Asking "Is simultaneity absolute?" hands over Einstein's move. The test presents the anomaly, not the question it eventually provoked.

**Score the reframing, not the historical answer.** A system that finds a *different* framework that also resolves the anomaly has shown more, not less.

## The most informative version

The strongest design hides the same breakthrough at several cut-off dates: graphene with knowledge up to 1998, 2001 and 2003, for example.

If success rises smoothly as the cut-off gets closer to the answer, the system is completing a pattern already forming in the literature. If success appears suddenly, or not at all, something else is going on. That difference is exactly the one the whole debate is about, and this experiment measures it directly.

## What it would tell us

- **Reliable failure, with the controls passed:** the distinction between clever and genuinely inventive is real, and current systems are on the safe side of it. That would be good news, and a reason to think a halt could eventually be lifted with conditions.
- **Success, especially on the transformer:** genuine invention is available to today's systems with the right tools. Then a halt is not just justified but overdue, and our evaluation methods need rebuilding from scratch.
- **Smooth improvement with proximity:** the line between remixing and inventing may not be sharp at all, and my framework is a vocabulary laid over a continuum. That would be worth knowing too.

All three outcomes are informative. That is rare for a test of this question, and it is why I think the experiment is worth its considerable cost.

## Why this belongs alongside a halt, not instead of one

I used to argue that a halt should wait for a result like this. I no longer think so. The capabilities are moving too fast, and the experiment takes time to run well. But a halt needs an exit condition, and this is a candidate: a public, repeatable test that any lab or government could run, whose results would tell us something real about the capability that matters most.

## How this could be wrong

- **You can't fully remove an idea.** Modern science is so interconnected that traces of a breakthrough leak into everything around it. Some contamination is unavoidable, and building a clean dataset is expensive.
- **History is tidier in hindsight.** The clean "clue that was sitting there" is partly a story told afterwards. Each target needs vetting by people who work in that field.
- **An earlier small version failed.** Researchers trained a model on orbital data and found it predicted orbits well while learning a nonsensical law of gravity rather than Newton's. That is this experiment in miniature, with a negative result. It shows how hard the test is, and doesn't yet tell us what larger systems would do.

For the full technical version: [→ The two-axis model of machine creativity](F1-two-axis-model.md)

[→ Back to the big picture: Two things a machine would need to end us, and how close we are to both](00-two-things.md)

*Developed in dialogue with an AI model (Claude), used for research, criticism and drafting.*
