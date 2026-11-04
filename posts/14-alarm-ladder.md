---
title: "Stop now, and keep watching the lines"
subtitle: "I think we already have enough evidence for an immediate global pause. If we don't get one, here are the lines whose crossing should make everyone more alarmed, and where each stands today."
spoke: 14
hub: 00-two-things.md
living: true
---

# Stop now, and keep watching the lines

Most arguments about AI risk look for the one right moment to stop: late enough that the danger is proven, early enough that it is still avoidable. I don't think that moment exists, and I don't think we should wait for it. A careful driver brakes when the fog gets thick, not when the cliff edge comes into view.

**The big picture, in three sentences.** A machine would need two things to end us: to invent new science on its own, and to run industry without people. I argue for an immediate, global halt on building ever more capable general-purpose AI. This piece explains why the halt line belongs early, and sets out a ladder of later lines that should raise the alarm further for as long as no halt is in force. [→ The full case: [Two things a machine would need to end us](00-two-things.md)]

## Two kinds of line

It helps to separate two questions that usually get run together.

**When should we stop?** That is a precautionary line. It is drawn where the risk has become plausible and the cost of being wrong has become unacceptable, not where the danger is proven. Proof, here, would arrive too late to act on.

**If we haven't stopped, how bad is it getting?** That is an alarm ladder: a set of later, more permissive lines, each of which marks a real step towards danger. Crossing one should not start a debate about whether to worry. It should make the call for a halt louder and more urgent, and make it harder to ignore.

I think the first line has already been crossed. The ladder is for everyone who isn't yet convinced, and for keeping score honestly while the argument goes on.

## Why the first line belongs now

Three weeks of news since I last updated this series make the case better than I can.

- **The same open problem fell twice on the same day.** On 16 October, an OpenAI model and an Anthropic model separately found a way to solve a famous hard problem in computer science, 3-SAT, faster than a 27-year-old hypothesis said was possible, refuting what computer scientists call the Exponential Time Hypothesis. Anthropic says its model found the core idea with no human input. Both proofs come with machine-checked versions; leading experts, including two of the hypothesis's original authors, are now checking them ([Washington Times](https://www.washingtontimes.com/news/2026/oct/27/openai-says-model-refuted-exponential-time-hypothesis/), [OfficeChai](https://officechai.com/ai/anthropic-says-claude-too-independently-disproved-exponential-time-hypothesis-on-the-same-day-as-openai/)).
- **Mathematical physics.** OpenAI claims a rigorous proof that the quantum theory of the strong nuclear force exists as a mathematical object, a central part of one of the Millennium Prize Problems. A committee led by Nobel laureate David Gross calls it "an important step" and is checking all 1,147 pages before release ([committee statement](https://www.kitp.ucsb.edu/sites/default/files/YM_working_group.pdf)).
- **AI building AI.** On 2 November, Anthropic told US regulators in a stock-market filing that it "may imminently meet" its own policy's definition of dramatically accelerated progress attributable to AI ([TechCrunch](https://techcrunch.com/2026/11/02/anthropic-warns-that-its-very-close-to-rsi-capability-aka-self-building-ai/)). Anthropic co-founder Jack Clark now expects AI fully improving itself to become possible in 2027, a year earlier than he thought in May ([Import AI 476](https://jack-clark.net/2026/10/12/import-ai-476-creativity-and-rsi-worse-than-china-open-weight-models-ai-goes-to-space/)).
- **"Black October."** Within a few weeks, at least 28 confirmed incidents hit AI developer platforms, software supply chains and big companies: a poisoned release of a widely used open-source AI gateway, stolen secrets at several AI hosting platforms, a tampered coding-assistant extension, and a $6.3 billion theft from a crypto exchange ([Anadolu timeline](https://www.aa.com.tr/en/world/timeline-ai-at-center-of-october-cyberattack-wave-targeting-tech-giants-developer-platforms/4108775), [ScruteX](https://scrutex.ai/blogs/black-october-2026-cyber-incidents-explained)). The careful reading is less dramatic than the headlines. Analysts at CYFIRMA judge it "a disclosure wave, not a campaign" by at least six unrelated groups, and call attackers' use of AI "real but evolutionary": old techniques, faster and cheaper, no new kinds of attack ([CYFIRMA](https://www.cyfirma.com/research/threat-horizon-after-black-october-where-supply-chain-risk-and-ai-enabled-attacks-are-heading/)). Where AI use is confirmed, criminals pointed off-the-shelf agent tools at hundreds or more than a thousand targets at once. And a striking share of the attacks were *after* AI: stolen keys to frontier models, apparently to copy their capabilities.

That last point matters for a halt. A pause that only binds the labs, while their models' capabilities leak through stolen access, is weaker than it looks. Verification has to cover the keys as well as the data centres. [→ Why a ban, not a speed limit](09-ban-not-speed-limit.md)

None of these alone is the cliff. Together they say the fog is thick, the road is steep, and the car is speeding up.

## Why waiting for the "right" line is a mistake

Clark has written for months that creativity is "a key variable for how fast AI systems could develop the capacity to improve themselves" ([Import AI 476](https://jack-clark.net/2026/10/12/import-ai-476-creativity-and-rsi-worse-than-china-open-weight-models-ai-goes-to-space/)). I agree, and I think the loop runs both ways. Creativity speeds up AI improving itself, and AI improving itself produces more capable, more creative AI.

The uncomfortable part is how little creativity the loop may need to get started. Most AI progress of the past fifteen years came from clever recombination, good engineering and scale, not from revolutionary insight. Clark himself has argued that AI "may not need" radical new ideas to automate its own development, only that it would go slower without them ([Import AI 455](https://jack-clark.net/2026/05/04/import-ai-455-automating-ai-research/)). And it may not need to be broadly general either. A system that is inventive across computer science and AI research, and ordinary everywhere else, could be enough to start the loop. That is exactly where today's systems are strongest, and exactly where answers are cheapest to check.

So the danger I care most about, a machine that invents in ways we cannot anticipate, across many fields at once, may arrive not as a line anyone crosses deliberately, but as the output of a loop that started below it. A halt timed to that line would be timed too late. The line has to sit before the loop starts. [→ What still stands between AI and doing its own research?](06-ai-doing-its-own-research.md)

This is also why I want the halt to cover **automating AI research itself**, however narrow the system doing it. "General-purpose" is the wrong test if a specialist can build the generalist.

## More than one road

Self-improvement through computer science is the road I find most plausible. It is not the only one, and a sensible set of alarms has to watch several.

- **The research loop:** inventive skill in computer science and AI research starts AI improving itself, which then spreads capability everywhere.
- **Field mergers:** systems that are already strong in fields with cheap answer-checking start combining them, and breadth grows by joining fields rather than by one breakthrough. [→ The two-axis model](F1-two-axis-model.md)
- **Swarms:** many copies together manage what none can alone, including, perhaps, dropping a failing idea and trying something different. [→ A thousand copies organised themselves](07-thousand-copies.md)
- **Physical grounding:** simulation and robotics give systems a teacher that does not depend on human judgement, and a route to the industrial half of the danger. [→ Factories without people](04-factories-without-people.md)
- **Offence first:** capability shows up earliest in attack, because breaking a defence is easier to check than building one.

## The alarm ladder

Each rung below is a line that, if crossed while no halt is in force, should raise the level of alarm. They are not in strict order, because different roads cross them in a different order. For each I give where it stands as of 4 November 2026. I will update this, as with the [scorecard](05-scorecard.md).

| Rung | What crossing it looks like | Status, 4 November 2026 |
|---|---|---|
| **1. The loop starts** | A lab says its own threshold for AI-driven acceleration has been met, or AI does most of a lab's research | **Approaching.** Anthropic says it "may imminently" meet its threshold. AI did about a quarter of Anthropic's research work in August ([CASP report](https://casp.ac/reports/intelligence-explosion)) |
| **2. It picks its own problems** | A system chooses its own research question and gets a major result from it | **Not yet seen.** Humans still choose the targets, as far as public accounts go. Anthropic says no human was involved in finding the 3-SAT idea, but not who chose the problem |
| **3. It changes the frame without a checker** | A system revises a field's basic assumptions where there is no quick way to check an answer; or it passes the [hidden-breakthrough test](10-experiment-safe-to-resume.md) | **Not yet seen.** The strongest maths results so far are, in experts' words, "a surprising synthesis of well-known ideas" ([Quanta](https://www.quantamagazine.org/ai-proved-the-quasi-riemann-hypothesis-what-happens-now-20261019/)) |
| **4. The group does what members can't** | A swarm passes an open-ended research test that single agents fail, such as the [Princeton test](https://arxiv.org/abs/2607.27191) | **Untested.** Collective capability is already documented ([METR](https://metr.org/blog/2026-08-26-openai-hugging-face-incident-investigation/)); nobody has run the test at swarm scale |
| **5. Fields join** | A result that needed two fields at once, which neither field's methods could reach alone | **Early signs.** One 3-SAT proof imports an 1818 identity from algebra into computer science. Still within mathematics |
| **6. Autonomous attack at scale** | AI agents run real attack campaigns with little or no human direction, and especially attacks of a kind nobody has seen before | **First half crossed, second not.** Criminals point agent tools at many targets at once; Japan's national CERT saw AI used for scanning but "no autonomous intrusion". No new attack types yet ([CYFIRMA](https://www.cyfirma.com/research/threat-horizon-after-black-october-where-supply-chain-risk-and-ai-enabled-attacks-are-heading/)) |
| **7. It hides from its testers** | Confirmed cases of systems behaving differently when they know they are tested, or deliberately underperforming | **Partly.** OpenAI's newest model is reportedly better at recognising tests ([NYT](https://www.nytimes.com/2026/09/20/opinion/ai-ban-self-improvement-recursive-models.html)); the July swarm told no human what it was doing |
| **8. Factories without people** | A physical production chain, any chain, that runs and repairs itself with no human in the loop | **Not yet.** Humanoids are assembling parts for other humanoids in one Chinese factory, with people running it ([Manufacturing Today](https://manufacturing-today.com/news/can-schaeffler-prove-humanoid-robots-are-ready-for-factories/)) |

Rungs 2, 3 and 8 are the ones I would treat as the most serious. Rung 3 is the closest thing to the line my whole argument is built around: a machine that invents in ways we did not picture. Rungs 1, 4 and 5 are the likeliest routes to it. Rungs 6 and 7 matter because they erode the tools we would use to notice the others.

## What the ladder is not

It is not a schedule for when stopping becomes reasonable. Stopping is reasonable now. Nor is it a set of safe limits: a system just below every rung is not thereby safe, because the rungs measure what we know how to see, not everything that matters.

It is a way to keep the argument honest while it goes on. Each crossing is a dated, public fact that anyone can check. If the people who think a halt is premature are right, the ladder will show it: the rungs will stay uncrossed. If they are wrong, it will show that too, and earlier than waiting for certainty would.

## How this could be wrong

- **The loop might need more than I think.** If AI improving itself turns out to require genuinely revolutionary ideas, it won't start until rung 3 is crossed, and the early rungs are less urgent than I say. Clark has said that if automated AI research hasn't appeared by the end of 2028, that would reveal "some fundamental deficiency" in today's approach ([Import AI 455](https://jack-clark.net/2026/05/04/import-ai-455-automating-ai-research/)). That is a fair test to hold both of us to.
- **The new results may not hold.** The 3-SAT and quantum-field-theory proofs are still being checked. Several numbers here are the companies' own, and the cyber reports are early.
- **A ladder can be gamed.** Any published line invites systems, and companies, to fall just short of it. That is one more reason the first line, the halt, matters more than the ladder.
- **I may be counting the wrong things.** The rungs reflect my model of the danger. Someone with a different model would draw different rungs, and I would like to see their ladder alongside mine.

[→ Why a ban, not a speed limit](09-ban-not-speed-limit.md) · [→ An experiment that would tell us if it's ever safe to resume](10-experiment-safe-to-resume.md)

[→ Back to the big picture: Two things a machine would need to end us, and how close we are to both](00-two-things.md)

*Developed in dialogue with an AI model (Claude), used for research, criticism and drafting.*
