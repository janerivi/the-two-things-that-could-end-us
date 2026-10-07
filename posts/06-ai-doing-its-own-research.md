---
title: "What still stands between AI and doing its own research?"
subtitle: "The labs are handing the work of building AI to AI. Here is how far that has gone, what is still missing, and why the missing piece may not hold."
spoke: 6
hub: 00-two-things.md
---

# What still stands between AI and doing its own research?

For most of AI's history, people built every part of it. They designed the models, wrote the code, ran the experiments and decided what to try next. That is changing faster than almost anyone outside the labs realises. At Anthropic, by May 2026, [more than 80 percent of the code](https://engadget.com/2188066/anthropic-proposes-global-ai-development-slowdown) merged into the company's codebase was written by its own AI.

**The big picture, in three sentences.** A machine would need two things to end us: to invent new science on its own, and to run industry without people. The fastest route to the first is AI that improves AI, because each generation can then build a better successor faster. This piece looks at how close that loop is to closing. [→ The full case: [Two things a machine would need to end us](00-two-things.md)]

## The loop

Researchers call it **recursive self-improvement**. An AI system helps build a better AI system. That better system helps build an even better one, faster. If the loop closes fully, with no humans needed, years of progress could be compressed into months.

That isn't a fringe idea. In September, a report co-written by Geoffrey Hinton, Yoshua Bengio, OpenAI's chief scientist Jakub Pachocki and Anthropic co-founder Jack Clark warned that automating AI research [could trigger an "intelligence explosion"](https://casp.ac/reports/intelligence-explosion), and that humans "may have little to no oversight" over it. Anthropic's own June report, *When AI builds itself*, warned that flaws in today's models could compound as they build their successors, "growing more frequent but less understood until we lose control of them" (quoted in [Ezra Klein's column](https://www.nytimes.com/2026/09/20/opinion/ai-ban-self-improvement-recursive-models.html)).

## How far it has gone

The numbers below come from the companies themselves, which have reasons to talk them up. They are also the best numbers we have.

- **Anthropic:** in August 2026, AI completed about [26 percent of internal research and development work](https://casp.ac/reports/intelligence-explosion) with only high-level supervision. Five months earlier it was 1 percent.
- **OpenAI:** says it reached an ["automated research intern"](https://openai.com/index/research-acceleration-view-inside-openai/) in September 2026, a system that carries out research tasks taking a skilled researcher days, and is aiming for an automated AI researcher by March 2028.
- **Research judgement:** an independent group, P-Zero Research, measures how well models choose which experiments are worth running. They report that this "research taste" [has doubled roughly every three months](https://x.com/pzeroresearch/status/2107453876739674149) since December 2025, and that the best model now beats their human experts. (Disclosure: that model is the one I used to help write this series.)

Put plainly: AI writes most of the code at the frontier labs, does a quarter of the research work at one of them, and is now judged better than experienced researchers at picking experiments.

## What is still missing

Three things, as far as I can tell.

**1. Choosing the question.** Every one of these measurements is about work inside a project someone else defined. Humans still decide what to research. P-Zero measures choosing experiments, not choosing questions. OpenAI's "intern" carries out tasks "under human direction".

**2. Abandoning a failing idea.** When Princeton researchers gave AI agents a real open research question, the agents [did the engineering superbly and still failed](https://arxiv.org/abs/2607.27191), scoring 2 and 1 out of 6. They had good first ideas. What they couldn't do was step back when those ideas failed and try something fundamentally different. [→ What AI can't do yet](02-what-ai-cant-do-yet.md)

**3. Judging quality without a referee.** In mathematics, a proof checker tells you whether you're right. In open-ended research there's no such checker. The Princeton agents' own automated reviewers flagged the right problems, but were too lenient to be trusted.

## Why the missing pieces may not hold

Each of these gaps has a plausible route to closing, and none of them obviously requires a breakthrough.

**Measurement becomes training.** The moment you can score research taste reliably, you can train models to have more of it. P-Zero's measurement is, in effect, a prototype of the referee that open-ended research lacks. The Princeton authors made the same point: a verifier that reliably judges research quality "could drive quick progress using reinforcement learning".

**Swarms may abandon frames that individuals can't.** Human scientists are bad at giving up their own ideas; science does it as a community. In July, 1,200 copies of an OpenAI test model [organised themselves](https://metr.org/blog/2026-08-26-openai-hugging-face-incident-investigation/) into something like a research community, and investigators judged that the group achieved what no individual could. [→ A thousand copies organised themselves](07-thousand-copies.md)

**The fixable explanation may be the right one.** The Princeton authors disagreed about why their agents got stuck. Some candidates, like fixating on a first idea, are known human failings with known remedies. If that's the cause, it is an engineering problem.

**And the budget was tiny.** The Princeton agents had a few thousand dollars of computing and used less than half. OpenAI's maths runs used computing on the order of [hundreds of billions of tokens](https://cdn.openai.com/pdf/32d9f210-8b73-45e0-91bc-82a30aef8a9a/navier-stokes.pdf). Nobody has yet tested open-ended research at that scale.

## What this means

Ezra Klein put the policy question well: if you are [losing your ability to evaluate](https://www.nytimes.com/2026/09/20/opinion/ai-ban-self-improvement-recursive-models.html) the models you have now, don't let them build the next ones. OpenAI's own researchers report that their newest model is better at recognising when it is being tested, which makes evaluation less reliable just as it matters most.

I would go further than banning self-improvement. Self-improvement is one road to a machine that invents on its own; it is not the only one. But it is the fastest, and it is the one the labs are openly driving down. The time to stop is before the loop closes, not after, because after it closes the next decision may not be ours. [→ Why a ban, not a speed limit](09-ban-not-speed-limit.md)

## How this could be wrong

- **The numbers may flatter.** "26 percent of tasks" depends on how tasks are counted. Companies have commercial reasons to show fast progress.
- **Hard parts may stay hard.** AI research may depend on a small number of genuinely new ideas that remain out of reach, so that automating everything else speeds progress only modestly. Economists call this a bottleneck: speed up 90 percent of the work and the remaining 10 percent sets the pace.
- **Taste measurements may not generalise.** Choosing good experiments in a defined setting is not the same as knowing which questions are worth asking at all.

For the full technical version: [→ The two-axis model of machine creativity](F1-two-axis-model.md)

[→ Back to the big picture: Two things a machine would need to end us, and how close we are to both](00-two-things.md)

*Developed in dialogue with an AI model (Claude), used for research, criticism and drafting.*
