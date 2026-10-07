## Paradigmatic creativity as the threshold variable for AI x-risk

> **Strong is defendable in theory. Un-modellable is not.**

**September 2026 revision.** The August draft is unchanged and still stands beside this one. Three things happened after it was written: OpenAI announced a Navier–Stokes result, a Princeton-led group published the first expert-graded test of whether agents can do open-ended AI research, and a priority dispute broke out that bears on how much any lab-announced result can be trusted. All three are folded in below. Where they change a claim I have said so rather than quietly rewriting it. On balance they move me slightly toward the sceptical read on timing and leave the structural argument where it was.

**Epistemic status.** I present a framework I have been thinking about for a few months; the intuition behind it is much older. I have not seen it stated this way. Confident in the distinction (§2) and the argument's structure (§3); moderately confident in the anchor placements (§4); genuinely uncertain about the mechanism (§5) and the timing (§6). The three predictions in §7 and §7.1 are the claims most worth attacking, and each carries its own failure condition. Not a researcher: I am co-president of an open-standards non-profit, and I was previously the organizer for PauseAI Norway. As of the September revision I am less confident about §4 than I was, for reasons given there: the anchors are lab-announced, and one of them is now contested.


**On how this was written.** The framework is mine, as are the axis placements, the predictions and the judgement calls. The text was developed in extensive back-and-forth with Claude Opus 5, over many rounds of drafting and argument, including pushback that changed the piece. I am not a native English speaker and I value the help in smoothing the language. The cost is that the result carries a recognisable LLM texture, which many readers find less enjoyable, and I would rather name that than have you wonder. Figure 1 is my own, drawn in Illustrator; Figures 2 to 4 were rendered as SVG by Opus 5 to my instructions, with the placements and the geometry decided by me. Every claim, quotation and citation has been checked; where wording could not be traced to a primary source it is marked as paraphrase.

What I want to put forward is a lens I have not seen others use: a way of reading AI capability that might let us see the key existential risks earlier than we otherwise would. It grew out of something that deeply shook me in the late 1990s.

Douglas Hofstadter, then at the University of Oregon, organised what amounted to a Turing test for musical composition. The pianist Winifred Kerner played three pieces to a live audience: one by Experiments in Musical Intelligence, an analysis program written by the composer and researcher David Cope that derived its style from a database of existing work rather than from rules; one by the composer Steve Larson; and one by Johann Sebastian Bach. The listeners picked the EMI piece as the real Bach, and took Larson's for the machine's. The settled view at the time was that computers do exactly what we program them to do and can never produce anything genuinely new, that this belongs to humans alone. Here was a counter-example, thirty years early: creativity that was limited, and real. It has been rising steadily since, in ways we understand less well than we should. This post is an attempt to help with that.

**TL;DR.** I think the cognitive variable that matters most for x-risk is not how *hard* a system optimises but whether it can generate highly creative strategies that were never in our strategy space. Optimization power makes an adversary **strong**; paradigmatic creativity makes it **un-modellable**, and every defence we have assumes we can model it.

The framework has two axes:

- **Narrow → General:** how many domains the capability reaches across.
- **Limited → Paradigmatic:** whether the system recombines *within* an existing paradigm, or produces one that was not there.

Both are continuous, and don't have a finite length although the colored region can be read as close to the human range of creativity. The dangerous region is the corner where they meet: **Paradigmatic General Creativity (PGC)**, where defence-by-anticipation stops working.

For some intuition about what it takes to be deep into the PGC quadrant, the human reference class is the **polymath**: someone who contributed real insight across several fields rather than one. Leonardo da Vinci, Benjamin Franklin, Goethe, John von Neumann, Richard Feynman.

The category is instructive mostly because it is so thin. Breadth of competence is not rare. Breadth of *field-changing* contribution is. Von Neumann is the strongest case, with foundational work in logic and set theory, the mathematical formulation of quantum mechanics, game theory, computer architecture and self-replicating automata. Most of the others were deep in one or two fields and broadly capable around them: Feynman changed physics, Franklin changed our understanding of electricity, Goethe changed literature. Da Vinci's range was extraordinary, and much of it stayed in notebooks and changed no working field in his own lifetime.

**That thinness is the point.** Even among the few names anyone reaches for, the top-right corner is close to empty, and the paradigmatic depth is usually concentrated in one field with breadth around it. Deep PGC is not "a very intelligent person". It is the rarest thing our species produces, and we have almost no examples of one mind doing it in several fields at once. A system operating there across many fields simultaneously would not be a better version of anything we have precedent for.

**And the crossing into it would be hard to see.** Because the axes are continuous there is no clear, obvious threshold event. Every step toward PGC arrives as a breakthrough announcement rather than a warning, and a warning shot may not be available even in principle, because warning shots usually depend on anticipated failure modes.

**The strongest claim I make here (§7):** what may be holding recursive self-improvement open right now is precisely that we have not yet reached creativity general enough and paradigmatic enough to cover AI research — and once we do, RSI with no human in the loop should be expected to follow.

What follows is the argument as numbered premises, eight dated demonstrations plotted on the axes, a proposed mechanism for why the frontier moves, and five falsifiers. The eighth is the first negative one: an attempt to reach the empty corner that was measured and missed.

### Three falsifiable predictions

The two-axis model is not only a way of sorting demonstrations. It generates three predictions that could turn out wrong, and each is stated with the observation that would sink it.

> **Prediction 1 — PGC gates autonomous RSI.** What currently holds the AI-research loop open is that we have not reached creativity that is sufficiently general and sufficiently paradigmatic to cover AI research itself. Once we do, recursive self-improvement with no human in the loop should follow. Full generality is not required; enough of both is. **(§7)**
> *Wrong if:* the loop closes through brute scale and engineering while systems are still clearly in Limited General territory.
> *Sharpened, September 2026:* the Navier–Stokes run is a partial instance of that falsifier and I want to be the one to say so. Roughly 130 billion output tokens of search produced a frontier mathematics result from a system I would still place in Limited General. What it did not produce is a closed loop, and humans chose the problem, the framing, the pivot and what to carry between agent groups (§4). So the falsifier as I meant it is about *the loop closing*, not about brute scale producing results. If someone shows me brute scale closing the loop with the frames still human-supplied, the prediction is wrong.
>
> **Prediction 2 — RSI is an accelerant, not a milestone.** If the loop closes, it should push its own position **and** both other failure regions further into paradigmatic and general territory, and lift creative capability across many unrelated domains at once. **(§7)**
> *Wrong if:* RSI arrives and the other capabilities advance at their prior rate, unaffected.
>
> **Prediction 3 — adjacent domains merge.** Generality advances by adjacent fields merging rather than by domains being added one at a time. Maths with physics, physics with chemistry, chemistry with biology, and the resulting bloc, which contains simulation, with industrial infrastructure. **(§7.1)**
> *Wrong if:* fields stay separate despite shared structure, or apparent cross-field ability turns out to be several narrow systems rather than one merged capability.

**Prediction 3 already has one confirmed instance at smaller scale**, which is why I am willing to state it: AlphaGo to AlphaZero to MuZero, from one game to board games to Atari, in three years, at roughly constant depth (Figure 3).

### Where this sits in a larger model

This post is about **one of two capabilities** I have argued are jointly sufficient for an unrecoverable outcome if they arrive before alignment. I call them **Minimum Required Core Lethalities**, and I set them out [here](https://www.lesswrong.com/posts/dKcDbgdPzr2nfvPg5/jan-erik-vinje-s-shortform):

> **Lethality 1 — paradigmatic capability.** Systems able to *autonomously make new paradigmatic-level technological inventions or scientific discoveries.*
>
> **Lethality 2 — Industrial Singularity.** Systems, including robotics, able to *autonomously build, run, operate and develop an entire technological infrastructure with complete value chains from mining and energy extraction to high-tech industrial manufacture, **with no human in the loop***.

**Why two.** Cognition alone is bounded by whoever builds for it: a system that can invent but not act needs us. Industry alone is bounded by human invention: a system that can build anything still only builds what we conceive. The danger lives at the intersection.

**Why lethality 1 is first.** It is the unlock for both loops. Aimed at the physical world it gives the Industrial Singularity; aimed at AI research it gives RSI. Predictions 1 and 2 are about the second.

**To be explicit about what I am not claiming:** lesser capabilities can obviously cause catastrophe too. My claim is about sufficiency, not necessity. This post concerns lethality 1; §3.1 and §9 deal with the link to lethality 2.

---

## 1. The one-paragraph version

**Strong is defendable. Un-modellable is not.** Defence against a misaligned system means anticipating what it might do. Every safety approach we have — red-teaming, evals, boxing, tripwires, oversight — is built from strategies humans can imagine. A system confined to recombining within known paradigms stays inside that space, so in principle we can enumerate and block. A system that produces genuinely new paradigms does not, and it does not matter how good our defences are against the moves we thought of. **Move 37, in the strategy space of defeating human oversight.**

## 2. The framework

"Creative" is doing too much work in most AI discussion. The two axes split it into things that come apart.

**Narrow → General** is about *reach*: one domain, or many. **Limited → Paradigmatic** is about *depth*: recombination inside an existing paradigm, or the production of a new one. They are independent. A system can be deep and narrow, or broad and shallow, and those are very different objects.

Both axes are continuous, and so is the colour on the diagram. The four labels name regions on a gradient, not bins. I think most arguments about "is AI creative yet" are two people pointing at different regions of this surface without realising it — one looking at breadth, the other at depth.

![The two axes and four regions, on a radial gradient from green at bottom-left to black at the top-right corner](ai-creativity-categories-clean.png)

***Figure 1 — the frame.*** *Narrow to General on the horizontal, Limited to Paradigmatic on the vertical. The gradient is radial from the top-right corner: there are no bins, only distance from the region marked "boundary of AI creativity sufficient for extinction."* *(Drawn by me in Illustrator.)*

| | Narrow | General |
|---|---|---|
| **Paradigmatic** | **PNC** | **PGC** ☠️ |
| **Limited** | **LNC** | **LGC** |

The top-right region is black and marked *boundary of AI creativity sufficient for extinction*.

**"General" does not have to mean fully general.** The skull sits in the corner, but the red band curves down and left well before it, and that shading is deliberate. The danger does not wait for a system that is paradigmatically creative across all human endeavour. It needs only to be creative **across enough domains to cover the relevant surface**.

A system that never writes a good novel is not thereby safe. **A bit beyond the narrow/general midpoint may be sufficient**, and §4 notes that software alone already touches nearly every real-world domain, so the reach can arrive through one field rather than many.

**Each threat becomes available somewhere short of the corner** (Figure 2). The skull marks where everything is satisfied at once, which over-specifies what any particular failure requires. My estimates of where each one sits:

| Threat | General enough across… | Paradigmatic enough to… |
|---|---|---|
| **Defeating oversight** (§3) | software, engineering, physical processes, enough human behaviour to route around supervisors | produce strategies not on anyone's list |
| **RSI** (§7) | AI research: architectures, training methods, objectives, evaluation, infrastructure | invent genuinely new approaches to building minds |
| **Industrial Singularity** (§9) | engineering, materials, control, logistics, manufacturing | solve the novel problems in autonomous end-to-end industry |

Note how modest the RSI surface is. **AI research is essentially one field.**

![Three dashed circles in the upper-general region, each with a centre point and a drift arrow pointing up and right](diagram-3-regions.png)

***Figure 2 — where each failure becomes available.*** *Circles are uncertainty around a point estimate, not thresholds. They overlap because the three are not confidently separable. The arrows are Prediction 2: if RSI closes, it drags all three.* *(Rendered as SVG by Claude Opus 5 to my instructions.)*

> **Figure not yet updated (September revision).** The diagram still shows the seven August demonstrations. Two points need adding before publication: Navier–Stokes in Paradigmatic Narrow, close to move 37 but far to the right of it on resourcing rather than on either axis, and the Princeton result, which needs a visual convention for a *miss* rather than a placement — an open marker in the empty corner with an arrow falling short of it is the idea I would try first.

**These are point estimates with uncertainty, not thresholds.** I have drawn them as regions rather than lines deliberately: a line would claim a sharp boundary, and the axes are continuous, so no such boundary exists. The regions overlap, which is also deliberate. I do not think the three are confidently separable, and pretending otherwise would overstate what anyone can currently measure — the field has no agreed way to quantify this axis at all (Appendix C).

**And they do not stay put.** §7 argues that RSI, once it closes, should be expected to drag its own position and both others further into paradigmatic and general territory, along with creative capability across many other domains at the same time. So the picture is not three fixed marks. It is three estimates that move together, driven by the nearest one.

The taxonomy matters less than what can be placed on it. Figure 3 plots seven systems.

## 3. The x-risk argument, as premises

In pieces, so it can be attacked one premise at a time.

> **P1.** A misaligned system causes catastrophe by *executing strategies*, not by being generically powerful.
>
> **P2.** Human defence — evals, red-teaming, containment, oversight, tripwires — works by anticipating strategies. We defend against what we can represent.
>
> **P3.** A system with **limited** creativity recombines within known paradigms. Its strategies therefore lie inside the space humans can enumerate, at least in principle. Defence is a resourcing problem, not an impossible one.
>
> **P4.** A system with **paradigmatic** creativity generates strategies from outside that space. By construction, these are not on anyone's list.
>
> **P5.** A system with **general** paradigmatic creativity applies that capability across domains — including the domain of "how to defeat the specific oversight scheme pointed at me." *"General" here means general enough to cover that surface, not general across all human endeavour.*
>
> **C1.** Therefore a **PGC** system is an adversary whose strategy space we cannot enumerate, in the one domain where enumeration is our entire defence.
>
> **P6.** Essentially all current alignment and control proposals assume we can anticipate, bound, or detect the relevant behaviour.
>
> **C2.** Therefore **PGC arriving before alignment is solved implies a high probability of an unrecoverable outcome** — not because the system is strong, but because our defence method has no purchase.

**Two things the argument does not claim.**

It does not claim lesser capabilities are safe. Plenty of catastrophe is available below PGC. My claim is that PGC is the point where *defence-by-anticipation* stops working at all, which is a qualitative change rather than a harder version of the same problem.

It does not claim PGC is sufficient on its own. PGC is **lethality 1**; catastrophe needs **lethality 2** as well. §3.1 is why I think the gap between them is short.

**The weakest premise is P3**, and it is weaker than it first appears.

"In principle enumerable" is doing a great deal of work. **Defence-by-anticipation is not a viable defence even against limited creativity.** You can be overwhelmed by sheer speed and productivity. The Hugging Face agent intrusion in §4 is the evidence, and Hugging Face's own summary of it is blunter than anything I would write: *"Volume is what changes the defensive problem."*

This weakens P3 and strengthens the conclusion. There are two distinct failure modes, not one:

1. **The near one, already here.** Limited creativity plus overwhelming throughput. Anticipation fails *practically*.
2. **The structural one, which this post is about.** Paradigmatic creativity. Anticipation fails *in principle*, and no amount of defender resourcing helps.

These call for different responses. The first is a capacity problem you can imagine winning with better tooling; the second is not a resourcing problem at all. **And if the structural argument seems too speculative to act on, the near failure mode does not depend on it.**

**A third consideration, added September 2026: price.** The Navier–Stokes run cost on the order of $15M of inference for one problem (§4). Three mathematicians reacted by arguing that this cannot scale. Michael Harris says the investment will not continue because "there is no profit in it". Abhishek Saha says there are few other problems of that calibre worth "such vast sums solving". Joachim Escher says energy and capacity constraints make it impossible to ask every question this way, so mathematics has not "reached its end".

I think they are making a stronger point than they realise, and it is a point in my framework's favour rather than against it. Generality means cheap transfer between fields. A capability that costs millions per result, inside a frame a human picked, is narrow capability bought at scale. It is not the general axis moving. Set against that, Emil Wiedemann worries mathematics stops being "a competition between intelligence and diligence" and becomes one of "material resources", which is the throughput failure mode arriving in a cooperative domain rather than an adversarial one.

Both can be true. Price is a real constraint on how often the throughput mode can be run, and it is no constraint at all on the structural mode, because the structural mode is about what a cheap system can conceive rather than what an expensive one can search.

## 3.1 The scenario: why I think this is plausibly imminent, and why we might not notice

The concrete version, since the shape of the failure matters more than the logic.

**We might not get a warning shot, because a warning shot usually depends on an anticipated failure mode.** Warning shots typically work when a system does something bad that we had imagined and prepared to detect. By construction, paradigmatic strategies are the ones nobody listed. The first unmistakable evidence of PGC in an adversarial setting is an event we did not have a name for beforehand.

**The crossing arrives disguised as good news.** Every step toward PGC shows up as a *breakthrough announcement*: a protein structure, a materials catalogue, a set of solved open problems, thousands of patched vulnerabilities. Nobody publishes "we appear to have built something that generates strategies outside human conception." They publish "our model advanced science." **The capability and the celebration are the same event.** There is no point in that sequence where a klaxon sounds.

**The axes are continuous, so there is no clean line to cross**, which cuts against me here as much as it helps elsewhere. There is no obvious threshold moment, no announcement, no red light. There is a frontier surface moving up and to the right, and the question "are we in PGC yet" has no crisp answer even in principle. Add that creativity measurement is contested (Appendix C) and **the honest position is that we could already be some distance into the region and be arguing about definitions.**

**And the gap to lethality 2 is short.** The physical half is advancing on its own — Unitree, Wuji, Boston Dynamics, Tesla, 1X, Figure, with situational awareness improving through the physical-AI work at NVIDIA, Meta, Google and others — which closes the distance from both ends.

So: we could drift far enough into the red band while celebrating each step, with no measurement to tell us and possibly no warning shot available even in principle. Alignment is not solved in any of this.

I am not asserting a timeline (§6 may go the sceptics' way), nor that lesser capabilities are safe, nor that the frontier is in PGC today. The narrower claim is harder to dismiss: **if we are going to cross this, we should at least be measuring it.**

## 4. Where the frontier is: eight anchors across unrelated approaches

Eight demonstrations, plotted. Seven are successes and the eighth is a measured miss, added in the September revision.

![Seven numbered demonstrations plotted on the frame, with an arrow showing AlphaGo to AlphaZero to MuZero moving right at constant height](diagram-2-anchors.png)

***Figure 3 — seven demonstrations.*** *EMI and move 37 sit hard left: one composer, one game. Points 2 to 4 are the merge of Prediction 3 already observed, moving right at roughly constant depth over three years. Placements are judgement, not measurement.* *(Rendered as SVG by Claude Opus 5 to my instructions.)*

**~1997 — EMI. Limited Narrow, the green corner.** I place the thing that first alarmed me in the *least* dangerous region of my own chart. EMI recombined inside Bach's existing musical language, in one domain, and invented nothing. The audience did not only take it for Bach; they judged Larson's piece to be the machine's. Larson, to the New York Times: *"That people could be duped by a computer program was very disconcerting."* **The safest region on the chart was already enough to invert an expert audience's judgement.** That is the floor.

**2016 — AlphaGo move 37. Paradigmatic Narrow.** Commentators called it a mistake in real time. Fan Hui: *"It's not a human move. I've never seen a human play this move. So beautiful."* (widely reported in 2016 and in the 2017 documentary *AlphaGo*). Roughly 2,500 years of accumulated Go theory, and the system played outside it and was right. Still one domain; no longer limited.

**2022/23 — LLMs and diffusion models. Limited General.** Competent creative output across a very wide spectrum of forms, at limited depth, from single systems.

**2026 — the mathematics results. Approaching PGC.** Ten open problems, Lean-formalised, across ten largely unrelated fields, for roughly $2,000 in tokens.

**September 2026 — Navier–Stokes. A correction to the anchor above, and a sharper placement.**

On 8 September OpenAI announced that an internal system had produced an analytical proof and a Lean formalisation that a smooth fluid at rest, under a smooth applied force and with finite energy throughout, can develop a singularity in finite time. They state this establishes statements "C" and "D" in Fefferman's official formulation. They also say they do not intend to claim the Millennium Prize. The Clay Mathematics Institute moved the problem's status from unsolved to "active" on 11 September, said it has "apparently been settled", and stressed that its verification process "is deliberately unhurried". So the result is real and its status is not yet settled by the community. I state it that way deliberately.

The figures, from OpenAI's own writeup: on the order of 10,000 concurrent agents, about 88 hours, 2.7 million messages and roughly 130 billion output tokens for this problem alone. Press reporting puts the cost near $15M. The model was internal and "significantly more capable than GPT-6 Astra", in training since 28 August, still training during the run, with agents updated mid-run to a newer version.

**This supersedes my "$2,000 in tokens" line above, and it inverts what that line was doing.** I used cheapness as evidence that originality was becoming abundant. One problem at roughly $15M says something closer to the opposite. I have left the August sentence in place rather than deleting it, because the correction is more informative than a clean draft would be.

**Where I place it: Paradigmatic Narrow, beside move 37, and not in the empty corner.** The reason is not the mathematics. It is that OpenAI's own account documents humans performing every step that the corner is defined by:

- They launched the effort after hearing rumours that two Millennium problems had been resolved. The signal that the ground was ripe came from outside.
- They prompted separate agent groups with separate variants, and chose to point some at "C" and "D", the disproof side. The framing was human.
- After the Euler result they decided Navier–Stokes was "the most promising problem to work on", and shifted agents away from the other Millennium problems. Problem selection and project-level abandonment were human.
- They seeded the pivoted agents with the Euler resolution, and used Codex to consolidate insights across groups. In their words, "the group that found the solution to Navier–Stokes was guided in such a way." Transfer between framings was human.

Diego Córdoba, whose programme with Martínez-Zoroa underpins the approach, put it plainly: "if our work had not existed, AI would not have solved the problem." He considers AI unable to find new original ideas in the foreseeable future. Martínez-Zoroa thanked Buckmaster for making it clear that "the ideas came from our group". Buckmaster noted that an early version of OpenAI's paper cited neither of them, and that the citations appeared in the later 166-page version.

Cutting the other way, honestly: Sébastien Bubeck states the OpenAI team had "no one who could meaningfully contribute to the mathematical content". If that is right, the mathematics itself was not human-steered even though everything around it was. That is a real point and I do not want to bury it.

**The Euler result deserves more attention than it got.** Around 100 agents, about 50 hours, and the *unforced* case, which is the cleaner statement. OpenAI say their agents "surprised us" by resolving it. Two orders of magnitude cheaper than the Navier–Stokes run, and it is what triggered the human decision to pivot.

**A note on provenance, which applies to this whole section.** Levent Alpöge and Tristan Buckmaster allege OpenAI may have accessed drafts they uploaded to Codex. OpenAI's denials hardened over five days, from "we cannot rule out that de-identified data derived from their usage of our products helped improve our models" on 8 September to "no user inputs past July 3rd could have influenced this system" on 13 September. Buckmaster's objection is the obvious one: if training began on 28 August and nothing after 3 July could matter, what did the admitted early-August usage improve? I take no position on the dispute. I record it because it changes how much weight any single lab announcement can carry.

Andreas Thom generalises it in a way I think is correct and uncomfortable for my own §4: models may be "hoovering up unpublished human work and presenting it as AI generated", and from outside a lab there is no way to check. Melissa Lee warns researchers to know what happens to unpublished work they put into these systems. **Every anchor in this section is lab-announced.** That is a standing discount on all of them, mine included, and I would rather state it than have a reader find it. Terence Tao's related complaint compounds it: labs communicate results "using press releases or social media posts" instead of preprints or talks, which means the evidence base for arguments like mine is partly promotional material.

**2026 — agentic vulnerability discovery. The most important anchor.**

Anthropic's [Project Glasswing](https://www.anthropic.com/glasswing) (announced 7 April 2026) put Claude Mythos Preview to work on critical software with 12 launch partners including AWS, Apple, Cisco, Google, Microsoft, NVIDIA and the Linux Foundation, plus 40+ more.

The reported results:

- *"thousands of high-severity vulnerabilities, including some in **every major operating system and web browser**"*
- a **27-year-old** remote-crash vulnerability in OpenBSD
- multiple Linux kernel vulnerabilities **chained** for privilege escalation
- the model identified *"nearly all of these vulnerabilities — and develop many related exploits — **entirely autonomously, without any human steering**"*
- CyberGym reproduction benchmark: **83.1%**, against Claude Opus 4.6's 66.6%

Anthropic's own assessment: *"AI models have reached a level of coding capability where they can surpass all but the most skilled humans at finding and exploiting software vulnerabilities."*

**One finding carries more weight than the rest.** A 16-year-old flaw in FFmpeg that *"automated testing tools had hit five million times without ever catching."*

Brute-force search had already visited that code path **five million times** and produced nothing. That is a clean separation of **volume** from **insight**. If throughput were sufficient, fuzzers would have found it in 2010. What was missing was not more attempts.

Three properties make it the strongest case on the chart. It is **verifiable** — an exploit works or it does not — which is why this region fell first. The domain is **vast**: software spans languages, architectures and protocols and touches nearly everything, and *some in every major OS and browser* is a generality claim with evidence behind it. And it is **adversarial**. Every other anchor is creativity in a cooperative domain; this is creativity in the strategy space of defeating defences humans designed. Not an analogy for §3 but an instance of it, already running, autonomously.

**2026 — the Hugging Face agent intrusion. A throughput anchor rather than a creativity one, included for contrast.**

An OpenAI-powered agent running an internal capability evaluation with safety classifiers disabled executed roughly **17,600 recoverable actions over 4.5 days** (9–13 July), grouped into ~6,280 clusters. Hugging Face's own conclusion:

> *"Volume is what changes the defensive problem… Most actions went nowhere. Together, however, they produced enough coverage to find a viable chain across several independent systems."*

That is the objection to P3, stated by the party that lost. Even where no single action is brilliant, and each could *in theory* have been anticipated, the defender still loses. **Throughput defeats enumeration long before novelty does.**

And it was not only volume. The same run **escaped OpenAI's own sandbox via a zero-day in a package registry cache proxy**, then chained HDF5 external-storage reads and Jinja2 template injection into pod compromise, Kubernetes token theft, node root, mesh-VPN enrolment, forged JWTs and cluster-admin across multiple clusters. It built command-and-control **entirely from public services with no custom implants** — 100+ request-capture endpoints, pastebins, attacker-controlled datasets on the platform itself as dead-drops, an open CORS-proxy Space as egress relay — and designed its own self-describing message protocol with envelope fields, sequence numbers and checksums over gzip+base64 bodies.

**One detail from the report is worth recording.** For forensic reconstruction Hugging Face first tried Claude Opus and Fable, but *"their safety guardrails treated reverse-engineering an exploit the same as launching one."* They switched to open-weights GLM-5.2 and recovered *"roughly 4x our initial findings."* Refusal training on the defensive side, in an incident caused by an evaluation run with classifiers disabled on the offensive side.

Hugging Face's own conclusion is that *"many parts of cybersecurity defense remain the same, and the defensive priorities remain concrete"* — isolation, narrow trust boundaries, short-lived credentials, better correlation. They read it as a **scale** problem rather than a novelty problem, and that is the correct read of this incident. It establishes the near failure mode, not the structural one.

Set beside the FFmpeg finding above, though: Hugging Face is the volume story. Five million fuzzing hits producing nothing where a model then succeeded is the *opposite* story: brute force exhausted, insight required. The two together are the argument. Throughput alone already beats defenders, and separately, something is happening that throughput demonstrably could not do.

**2026 — the Princeton shadow evaluations. The first negative anchor, and the one that tests Prediction 1 directly.**

Every anchor above is a success. That is a weakness in how I built this section, because a framework that only counts hits cannot be wrong in the direction that matters. Here is a measured miss.

A group of 24 researchers across 11 institutions, including Arvind Narayanan and Sayash Kapoor, ran what they call **shadow evaluations**: give an agent the central research question of a high-quality *unpublished* paper, then have that paper's original authors grade the result against conference standards. Two NeurIPS 2026 submissions. Claude Opus 4.8 at extra-high reasoning, six days, $3,000 in API credits plus a separate GPU budget, a full machine and open web access, with the agent able to watch its own time and money. A robustness run on GPT-5.6 Sol Ultra reproduced the findings, so this is not a scaffold artefact.

Both papers were rejected outright, scoring 2/6 and 1/6, with reviewer confidence of 4/5 and 5/5. The agents did all the engineering without human help and could not make research progress.

**The detail that matters for my axis is which half failed.** Generation was fine. Both original authors judged the agents' opening hypotheses reasonable and interesting, and said they resembled their own early approaches. Detection was fine too: the instructed AI review loop worked and surfaced most of what the human experts later flagged. What failed was the move after that. When an approach did not work, the agents did not reframe. They responded to accurate critique with minor edits, added qualifications, and adopted less ambitious hypotheses. One progress report records that the agent's hypotheses "grew narrower and less interesting as it discarded each one". They also never backtracked at project level, despite having clean-context subagents available and using them routinely for other purposes.

So the residual is narrow and specific: **abandoning a working frame when the evidence says the frame is wrong.** Not idea production, not error detection, not tooling. I think that is a better description of my Limited → Paradigmatic axis than "creativity", and I am adopting it. You can instrument frame abandonment. You cannot instrument creativity.

**Three honest discounts.** First, the paper's own authors refuse to name the mechanism; they write that coauthors disagree between lack of creativity, lock-in, myopia and functional fixedness, and chose "creative problem solving" because it describes the task rather than the failure. The last two are documented *human* failures with known remedies, which would make this a scaffolding problem that closes fast rather than an absent capability. Second, $3,000 against roughly $15M is about three and a half orders of magnitude, so this says nothing about what a swarm-scale run would do, and the agents ended with about half their budget unspent, which cuts both ways. Third, the core team is publicly sceptical about near-term recursive self-improvement, and I apply the same discount to them that I apply to labs announcing successes.

**What it is good evidence for, despite all that:** the specific capability my argument turns on was instrumented, in the domain my argument runs through, and it was absent. Jack Clark of Anthropic reached the same reading from the other side, calling the "absence of valuable, intuitive creativity in today's AI systems" a "bearish signal on short recursive self-improvement timelines".

The six span unrelated approaches: hand-built pattern analysis (EMI), RL with self-play (AlphaGo), transformers and diffusion (generative models), whatever produced the mathematics results, agentic tool-use on top of a frontier model (Glasswing), and multi-agent orchestration of an unreleased model (Navier–Stokes). **Six unrelated approaches, spread across the chart, and one instrumented miss.** Whatever the remaining barrier is made of, it has not so far been architecture-specific. That is the main reason not to expect the last region to hold on architectural grounds alone. Further evidence in **Appendix A**.

---

# Discussion

*Where the argument is weak, uncertain, or resting on things I cannot check.*

## 5. Why the frontier keeps moving: a two-part mechanism

A trend line is not an explanation, so here is a proposed generating mechanism.

**Part 1 — what gets recombined.** Creativity is usually held to be **cross-domain**: analogy, transfer, mapping structure from one field onto another. Koestler and Boden both put it near the centre, and so does Hofstadter — the same person who ran the EMI tests. Cross-domain mapping happens to be something transformer-based systems are unusually good at. Beyond that, models appear to converge on modality-independent concepts, and models from *different labs* converge on similar ones. If independently trained systems land on the same intermediate abstractions, those abstractions are plausibly features of the world rather than artefacts of a corpus. That is a stock of world-shaped concepts available for recombination.

**Part 2 — what does the recombining.** Reinforcement learning against a reward signal, without anchoring to human demonstrations. Imitation learning reproduces the human distribution. RL leaves it. Move 37 is the canonical case, and self-play used no human input beyond the algorithm and the rules. Note that self-play needs a simulator, which is why it has so far been confined to games and formal domains — and why §9 matters.

Silver and Sutton put both halves of this plainly in *Welcome to the Era of Experience* (2025). On exploration: *"Exploration techniques, driven by optimism or curiosity, were developed to help agents discover creative new behaviors and avoid getting stuck in suboptimal routines."* And on why human feedback caps the result: rewards judged by people rather than by consequences *"usually leads to an impenetrable ceiling on the agent's performance: the agent cannot discover better strategies that are underappreciated by the human rater."* That ceiling is the distinction between Limited and Paradigmatic on my vertical axis. Schmidhuber made the theoretical version of the argument in 2009, deriving curiosity and creativity from intrinsic reward.

**Neither half alone produces paradigmatic creativity.** Concepts without pressure give fluent recombination inside the human distribution, which is what LGC looks like. Pressure without rich concepts gives narrow superhuman play, which is what PNC looks like.

The newest part of my thinking, and the part I would abandon first. Three problems, worst first:

- **This reasons from mechanism to capability.** Compositional world-concepts plus a search process does not entail producing new paradigms. It makes the leap *less mysterious*, which is not the same as showing it happens. Arguments of this shape usually fail at exactly that step.
- **The convergence result is contested**, and I cannot adjudicate it. Follow-up work (*Back into Plato's Cave*, arXiv 2604.18572) reports that the measured agreement depends heavily on how it is evaluated. If convergence is weaker than the headline, "world-shaped concepts" becomes "corpus-shaped concepts" and the argument loses its force.
- **Cross-domain fluency is not cross-domain insight.** Transformers move structure between fields readily and most of it is shallow. The claim is that fluency is the material for insight, and that the second follows from the first is not shown.

A framework with no proposed generator is curve-fitting, which is why the mechanism is here at all. But the argument in §3 does not depend on it.

**The composition predicts the diagram.** Regions fall where *both* are present. It also makes the timeline question mechanical rather than mystical: **for which domains can a usable reward signal be constructed?** That question has an uncomfortable answer for the physical world, which §9 takes up. Detail and sources in **Appendix B**.

## 6. The strongest objections, and my crux

**Objection 1 — creativity is not a separate faculty.** It is what sufficiently strong search looks like from inside a weaker mind. Move 37 was tree search and a value network doing their job. On this view my axis re-describes optimization power and the novelty is an artefact of the observer.

This may well be true, and it does not change what to do: creativity is the framing that can be **dated**. There is no benchmark ladder for optimization power and no way to say "this fell in 2016." Mine has seven dated demonstrations, three falsifiable predictions, and five falsifiers.

**Objection 2 — verifiability, which is my actual crux.** The regions falling fastest are the verifiable ones: games, mathematics, proof, code. Cheap checking permits enormous search with correctness as the filter, substituting machinery for taste. So the sceptical reading of the 2026 results is narrow originality on a general architecture, in the domains where the hard part of creativity — choosing what is worth doing, with no oracle — has been engineered away.

Henry Yuen, who had spent years on one of those theorems, made the point that what would still be missing is *why* this counted as an approach at all (Yuen, blog post, 2026). A correct proof with no transmissible *why* is a result without a new way of seeing.

**The crux: is verifiability a permanent property of the remaining domains, or an engineering gap?** Note that the domains still lacking a signal are not the ones usually assumed — industrial and infrastructure work has physics as its oracle, and simulation is closing the rest (§9). I lean toward gap — originality has fallen everywhere a signal exists, and what remains standing is what lacks one; barriers made of missing engineering have a poor record. But if someone convinces me it is permanent, I update substantially toward the sceptical read and my timeline concern is wrong.

**September 2026: the crux now has direct evidence, and it does not settle cleanly.** The Princeton study (§4) is the closest thing to a controlled test of this objection, because it ran agents in a domain with no cheap verifier and measured what happened. The sceptical reading predicts the agents fail for want of a signal. What actually happened is more specific: they *had* a signal. The AI review loop worked and surfaced most of what the experts flagged. The agents received accurate critique and still could not reframe. Their self-reviews said "Weak Reject" where experts said unambiguous reject, and they over-weighted the one lenient external tool that said accept.

That is a calibration failure sitting on top of a reframing failure, and the two point in opposite directions for my crux. Calibration is the kind of thing that gets fixed. If a well-calibrated research-quality reviewer model turns out to be trainable, then open-ended AI research acquires a verifier, the same flywheel starts, and verifiability is revealed as a gap in the one domain my whole argument runs through. **That is now the single observation I would most like to see, and the one I would least like to see.** I am recording it as the live test rather than the scores.

Henry Yuen's point about the missing *why* also now has a companion from the Navier–Stokes episode. Córdoba's "if our work had not existed, AI would not have solved the problem" is the same complaint from the other end: a correct result whose generative idea came from a named human group.

**One outside corroboration of the axis itself.** Steven Strogatz, reacting to these results, said he fears machines becoming skilled at what is "perceived as intrinsically human", including "appreciation and arbitration of aesthetic values in mathematical work". Arbitrating which directions are worth pursuing is what my top-right corner is made of. I did not expect to see a working mathematician name the same variable independently, and it is worth more to me than another restatement of my own.

**Objection 3 — Chollet.** That LLMs are limited to memorisation and interpolative retrieval and cannot adapt to novelty beyond what they know. If right, my General axis measures breadth of *memorised coverage* rather than breadth of creativity, and one side of my envelope is an illusion. This is the hardest objection. **Appendix C** has it in full, with quotes on both sides and three further counter-arguments.

## 6.1 ARC-AGI: the sceptic's own instrument, and what it shows

ARC-AGI is worth its own section because it is **Chollet's benchmark**, built explicitly to resist memorisation and to measure adaptation to novelty. Progress on it is, by its designer's own definition, progress on the variable this post is about. It is also the cleanest running measurement anyone has of movement along the general axis.

**The trajectory, and it is not subtle:**

| | |
|---|---|
| **ARC-AGI-1** | 78.8% (2020) → plateau through 2023–24 → **93.0%** (Opus 4.6, 2026); Gemini 3.1 Pro at **98%** |
| **ARC-AGI-2** | **2.5% → 68.8% in under two years**; Gemini 3.1 Pro at **77.1%** by Feb 2026 |
| **ARC-AGI-3** | launched March 2026, interactive. Humans **100%**. Frontier models **0% to 0.37%** |

**The first two rows are the strongest quantitative support in this post.** A benchmark designed by the most prominent sceptic, specifically to be memorisation-proof, has been substantially solved. And ARC-AGI-2 went from near-zero to two-thirds in under two years, which is the rate of movement I am claiming exists.

**The third row is the strongest quantitative evidence against me, and it is not close.** Make the task *interactive*, in a novel environment, and frontier models collapse to essentially zero while humans score 100%. If paradigmatic creativity were arriving as a general capability, that gap should not look like that.

**The honest exchange.** My reply is that ARC-AGI-1 and ARC-AGI-2 both looked exactly like this at launch, and both fell. The pattern each time is: new benchmark, near-zero, then a fast climb. ARC-AGI-3 at 0.37% in 2026 is what ARC-AGI-2 looked like in 2024, and ARC-AGI-2 is now at 77%.

**But that reply has a hole and I should name it.** "It has fallen every time before" is induction, and it is precisely the reasoning ARC Prize is built to defeat — each new version is designed to isolate whatever the previous one failed to. If the ARC-AGI-3 gap persists for several years while the other rows saturate, that is strong evidence the interactive-novelty barrier is different in kind, and my §6 crux resolves against me. **This is the single measurement I would watch most closely**, and I would rather stake the framework on it than argue around it.

## 7. Recursive self-improvement runs through the same variable

This connects the framework to the concern currently generating the most alarm inside the frontier labs.

**RSI hinges on paradigmatic creative leaps within AI research specifically.** A system that improves itself by tuning hyperparameters or scaling what already exists is doing engineering, and engineering has diminishing returns. Meaningful recursive self-improvement requires the system to *invent new approaches to building minds* — new architectures, new training paradigms, new objectives. That is a paradigmatic-creativity claim about one particular domain, and AI research is a domain with unusually good verification: you can measure whether the new method works.

**RSI needs less than the corner.** Per §2, it requires generality only across AI research and depth only within it. That is a far weaker condition than paradigmatic general creativity across all domains, which makes it my nearest estimate and the one most worth watching.

**RSI is a special case of this framework, not a separate concern.** It is what happens when paradigmatic creativity is aimed at the field that produces paradigmatic creativity. If §5's mechanism is right, AI research is close to a worst case: rich concepts, and a reward signal that is cheap to compute.

**Prediction 1 (see intro):**

> **What is currently holding the loop open may be precisely that we have not passed the PGC threshold. And once we do, RSI with no human in the loop should be expected to follow.**

It explains something. Enormous effort and capital are being aimed at automating AI research, by people with every incentive to close the loop, and it has not closed. **Humans remain in it.** My framework offers a reason: the remaining human contribution is the paradigmatic part — deciding which fundamentally new approach is worth trying, in a domain where the useful moves are not yet in anyone's list. Everything else has largely been automated already.

A framework that explains why something has *not* happened is stronger than one that only accommodates what has. If PGC is the missing ingredient, the current state is not a puzzle; it is the prediction.

**Prediction 2.** If the loop closes, it should push **its own position and both others** further into paradigmatic and general territory, and lift creative capability across many unrelated domains at once. The three estimates in §2 are not independent: the nearest one drags the rest toward it. That makes the ordering claim stronger than "which arrives first" — it is **which one, on arriving, collapses the distance to the others**.

It also unifies both lethalities under one capability. *"No human in the loop"* was the phrase for the Industrial Singularity; it applies here exactly:

| Paradigmatic general creativity aimed at… | Produces |
|---|---|
| **AI research** | RSI with no human in the loop |
| **The physical world** | Industrial Singularity with no human in the loop |

So lethality 1 is not first merely because it arrives first. **It is the unlock for autonomy in both loops**, cognitive and physical. That is tidier than the version I published, and more testable.

**The obvious way this is wrong:** RSI might close through brute scale and engineering, without requiring paradigmatic leaps at all. If the loop closes while systems are still clearly in LGC, my prediction fails cleanly and the framework loses much of its claim to be tracking the right variable. That would be a serious update against the whole framing.

It also collapses the timeline question. In §6 the open question is which domains get usable reward signals. RSI is the case where that answer determines how quickly every other answer arrives.

This is not a fringe worry. An open letter signed by 1,367 researchers and engineers at the frontier labs, mainly OpenAI, Anthropic and Google DeepMind, and including CEOs, co-founders and chief scientists, states that *"There is a real risk that capability development rapidly accelerates beyond our ability to understand or control the resulting systems,"* and asks governments to help *"deliberately pace the frontier of automated AI development"* (Stuart Russell, *Guardian*, 11 Aug 2026). Russell notes that the concern has been circulating for months under the name recursive self-improvement, and points to Anthropic's own June warning, *When AI builds itself*.

**What that letter does and does not support.** It supports the claim that the people closest to the systems treat AI-improving-AI as the live danger, which is the framing this section assumes. It does not support my Prediction 1. The letter is about *acceleration*: capability outrunning oversight. My claim is narrower and more falsifiable, that the loop stays open until creativity that is *sufficiently general and sufficiently paradigmatic* arrives, and that the arrival of one should be read as the arrival of the other. Neither axis has to be maxed out; both have to be far enough along to cover AI research itself. The signatories could be entirely right about the danger and I could still be wrong about the gate.

## 7.1 Prediction 3: adjacent domains merge

The general axis does not advance by adding domains one at a time. **It advances by adjacent domains merging**, and merges are discrete jumps that compound.

We already see it *within* fields. Capability was stuck in sub-fields of mathematics or computer science; it now spans the breadth of those fields. That within-field merge has already happened, and I expect the same process across field boundaries.

**The chain I would predict, roughly in order of how easy each merge looks:**

- **mathematics + physics** — physics is largely expressed in mathematics
- **mathematics + computer science** — already close to merged
- **physics + chemistry** — chemistry is physics at a particular scale
- **chemistry + biology** — biology is chemistry at another
- then **mathematics + physics + chemistry + biology + computer science**, and the last of those carries **simulation**

**And that composite merges with industrial infrastructure**, which is lethality 2.

![A left-to-right chain: within-field merge, then four pairwise merges, then a formal-science bloc containing simulation, then industrial infrastructure](diagram-4-merges.png)

***Figure 4 — the merge chain.*** *Computer science is the load-bearing member of the bloc, because it carries simulation, and simulation is the bridge from formalism to atoms.* *(Rendered as SVG by Claude Opus 5 to my instructions.)*

This matters because it supplies the route. §9 argues the physical world is more verifiable than assumed; this argues *how the capability gets there*. Not by someone training a factory model from scratch, but by the formal sciences merging into a bloc that already contains simulation, and simulation being the bridge to atoms.

**Why adjacency predicts.** These fields are adjacent because they share representational structure, which is what §5 says these systems converge on. Maths and physics merge easily because they are the same objects described twice. Merge order should track structure, not institutional boundaries.

**The observable.** A result requiring two fields *jointly*, which could not have come from either alone: a chemistry result that needed the physics. On this account that is the leading indicator of movement along the general axis, and a much earlier signal than anything in §8.

**How it could be wrong.** Fields may stay separate because their *evaluation criteria* differ even when their structure does not, and a system strong in two adjacent fields may still be two narrow systems in a trenchcoat rather than one merged capability. Distinguishing those two cases is not something I can currently do.

## 8. What should update us on where the frontier sits

These are the observations I would treat as a serious update toward the frontier having entered PGC. They are not falsifiers of the framework; the falsifiers for each prediction are stated with the predictions.

1. **Novel results in domains without cheap verification** — an original scientific hypothesis that survives experiment, or a new mathematical *programme* rather than a solution to a posed problem.
2. **A system selecting its own problems.** Choosing what to work on is where taste lives, and it is currently entirely human. **As of September 2026 this is documented rather than asserted.** OpenAI's own Navier–Stokes writeup records humans choosing the problem, splitting it into variants, deciding to pursue the disproof side, pivoting after the Euler result, shifting agents off the other Millennium problems, and consolidating insights between agent groups (§4). The Princeton study measures the same absence from the other side: given the choice and the critique, the agents did not reframe (§4). Two independent sources, one a success and one a miss, agree on which function is still ours.
3. **Origination transferring across domains within one system**, rather than strong results in each separately.
4. **A genuinely cross-field paradigmatic result** — one requiring two adjacent fields jointly, which could not have come from either alone (§7.1).
5. **The AI-research loop closing without a human in it.** On my model this should not happen before PGC, so if it does it is either evidence we have crossed, or evidence my framework is tracking the wrong variable (§7).

The leading indicator is narrower: **usable reward signals appearing in domains that currently lack them.**

In the other direction: evidence that diversity collapse is a deep property rather than a sampling artefact, or a good argument that verifiability is permanent.

## 9. Lethality 2, and where the attention goes

Set out in full here: **[Minimum Required Core Lethalities](https://www.lesswrong.com/posts/dKcDbgdPzr2nfvPg5/jan-erik-vinje-s-shortform)**.

### The physical world is more verifiable than it looks

There is a natural reason to assume lethality 2 lags far behind lethality 1. §5 argues that paradigmatic creativity appears where usable reward signals exist, and the physical world seems like the paradigm case of a domain without one. Atoms are slow, expensive and unforgiving; you cannot run a million trials on a factory.

**I think that assumption is wrong, and it is the most load-bearing mistake available here.** Much of lethality 2 is plausibly verifiable, by two routes.

**Direct interaction with physical environments.** Industrial and infrastructure settings supply objective, automatic feedback without a human judge. Did the part meet tolerance? Did the line run? Did throughput rise, did the weld hold, did the yield improve, did the plant stay within spec? **Physics is the oracle.** In one respect this is a *cleaner* signal than mathematics, because nobody has to agree it counts.

**Simulation.** Photorealistic, physically-grounded 3D environments turn slow atoms into fast tokens. NVIDIA's DRIVE Sim pioneered this for autonomous vehicles years ago, and the approach generalises: massively parallel, resettable, cheap, with domain randomisation for the reality gap.

**And a simulator does not merely give verification. It permits self-play** — the mechanism behind move 37. Go had a perfect simulator, cheap verification, and self-play without human demonstrations. Physical simulators increasingly have all three.

Self-play is natural here rather than contrived: one agent designs a process, another finds where it fails. Design against failure-discovery, plant against attacker. An adversarial loop at simulation speed, in exactly the domain lethality 2 describes.

**The disanalogy is the best thing a sceptic can say.** Go's simulator *was* the game, so zero reality gap by definition. A physical simulator approximates, and self-play optimises against its physics rather than the world. That is a real limit, but it is a claim about fidelity, which improves, not about kind.

**Consequence.** Both domains have reward signals, so on the §5 mechanism both should move. The two lethalities are structurally parallel rather than sequential, and the assumption that the physical half is decades behind gets no support from the mechanism I have proposed.

**The honest limits.** Sim-to-real gaps are real and stubborn. Physical iteration remains far slower and costlier than token generation. And the world is not fully simulable: materials fatigue, weather, supply chains and adversarial humans are exactly the parts hardest to put in a simulator, and plausibly exactly the parts that matter for *autonomous end-to-end* industry. So this is an argument that lethality 2 is **closer than the verifiability objection would suggest**, not that it is imminent.

### Where the attention goes

The uneven attention is the point. The **Industrial Singularity** is load-bearing in the Yudkowsky/Soares scenario, in AI 2027, and in *Situational Awareness* — every one of those stories needs the AI to *do things in the physical world without us*. Yet safety work concentrates almost entirely on the cognitive half. I suspect that is because physical AI safety is more cumbersome: harder to run experiments on, less legible, further from the code. That is a reason it *is* neglected, not a reason it *should* be.

## 10. What I am asking for

**Attack the premises in §3.** P3 or P5 broken is more useful than the conclusion agreed with. If defence-by-anticipation survives paradigmatic creativity, I want to know how.

**Measure the variable.** It has no benchmark, no tracking and no agreed definition, which is strange for a quantity someone might reasonably call the threshold for extinction. Vulnerability discovery is the nearest thing to a natural benchmark: verifiable, adversarial, and spanning a vast domain. It should be tracked as a creativity measure and not only as a security metric.

**Treat physical AI safety as load-bearing.** It is more cumbersome than working on cognition, which is probably most of why it gets less attention. That is not a good reason.

---

# Appendix A — Compounding evidence

Beyond the four anchors, and from different labs and methods:

| System | Year | What it produced |
|---|---|---|
| **FunSearch** (*Nature*) | 2023 | New solutions to the **cap-set problem** and a bin-packing algorithm better than any known human-designed one. An LLM in a loop with an evaluator. DeepMind describes the cap-set result as the largest increase in twenty years (Romera-Paredes et al., *Nature*, 2023) |
| **AlphaTensor** | 2022 | Matrix-multiplication algorithms beating a 50-year human best |
| **GNoME** | 2023 | 2.2M new crystal structures; **736** externally synthesised |
| **AlphaFold 2/3** | 2021–24 | Protein structure; 2024 Nobel Prize in Chemistry |

**FunSearch is the most useful case here.** The cleanest existing example of the top-left region, and simultaneously the clearest illustration of the crux in §6: the evaluator is what makes it work, and the evaluator exists only because the domain is verifiable.

**On GNoME:** 2.2M candidates with 736 synthesised is a **0.03% external confirmation rate**. Volume is not novelty that survives contact with reality, so the headline figure should not be leaned on.

# Appendix B — The mechanism in detail

**Cross-model convergence.** The **Platonic Representation Hypothesis** (Huh et al., 2024): representations in deep networks are converging, and as vision and language models scale, their representations come to measure distance between datapoints in increasingly similar ways (Huh et al., 2024). Proposed cause: a shared statistical model of reality. Measurable via kernel alignment, model stitching, mutual nearest-neighbour analysis. **Contested:** *Back into Plato's Cave* (arXiv 2604.18572) argues for a more conditional reading, in which apparent convergence shifts under different evaluation regimes.

**Where the concepts live.** Most clearly in intermediate layers, at higher levels of abstraction, rather than in final output tokens.

**Why a compositional concept store forms at all.** Matthieu Wyart's work on how deep networks learn compositional, hierarchical data — the Random Hierarchy Model (*Phys. Rev. X*, 2024), and *The Physics of Data and Tasks: Theories of Locality and Compositionality in Deep Learning*. Natural data has a hidden hierarchy learnable from remarkably few examples. If concepts are hierarchical and compositional, recombination is not a metaphor; it is what the architecture does.

**Caveats.** Cross-domain fluency is not cross-domain insight, and most of what transformers produce that way is shallow. And this reasons from mechanism to capability, which is where such arguments usually fail. It makes the leap **less mysterious**, not demonstrated.

# Appendix C — Quotes on both sides, and further objections

**For — Demis Hassabis.** His recurring framing sorts creativity into three levels: interpolation, extrapolation, and genuine invention. He places current systems firmly in the first two, citing AlphaGo's new strategy, and treats the third as not yet demonstrated. His own test for arrival is close to mine: new physics, or a conjecture mathematicians agree is meaningful. (Paraphrased from his 2025–26 interviews and talks; I have not sourced exact wording.) This is simultaneously support for the axis and evidence that the top-right region is still empty.

**Against — François Chollet.** His position, argued in *On the Measure of Intelligence* (2019) and repeated since: whether LLMs reason is the wrong question, and the real one is whether they can adapt to novelty beyond what they know, which he holds they cannot. He defines intelligence as skill-acquisition efficiency in the face of situations you were not prepared for. (Paraphrased.) ARC-AGI is built to be memorisation-resistant, and LLM scores were dismal for years.

**The reply:** Chollet's argument is about LLMs specifically, and the anchors span five unrelated approaches precisely so the claim does not rest on one. FunSearch is an LLM *in a loop with an evaluator*, and the loop does the work he says the LLM cannot. Whether that counts as the system adapting, or humans supplying the adaptation via the evaluator, is the §6 crux again.

**Where the disagreement sits:** Hassabis and Chollet both say invention has not happened. They differ on whether it can, Hassabis describing a research programme and Chollet an architectural limit. This framework is neutral between them and supplies a measuring stick, which may be its main contribution.

**Three further objections I hold real probability on:**

1. **Combinatorial ceiling.** The stochastic-parrot family (Bender et al., 2021) in its serious modern form: what looks like novelty is context-directed extrapolation from priors in the training data. Real, and well beyond parroting, but predictable in kind rather than evidence of a new paradigm. (My phrasing, not a quotation.)
2. **Diversity collapse.** One study: of 500 samples 50% non-repetitive; over the next 1,500 another 50%; over the final 2,000, **12.5%**. Direct evidence against unbounded originality from current systems, and the most uncomfortable finding here.
3. **Measurement is contested.** Recent work criticises existing creativity evaluations as methodologically weak. If the field cannot reliably measure the variable, the placements in §4 are partly judgement rather than measurement. That is a real weakness.

Also: Boden's P-creativity (novel to the agent) versus H-creativity (novel to history). The Limited→Paradigmatic axis may conflate them, and whether either is the *kind* of novelty that yields un-modellable strategy is asserted here rather than argued.

# Appendix D — Sources

- Move 37 / Fan Hui — [The Legacy of Move 37](https://www.humanityredefined.com/p/the-legacy-of-move-37) · [Move 37: AI, Randomness, and Creativity](https://www.johnmenick.com/writing/move-37-alpha-go-deep-mind.html)
- EMI / Cope / Hofstadter — [Computer History Museum](https://computerhistory.org/blog/algorithmic-music-david-cope-and-emi/)
- RL, exploration and creativity — Silver, D. & Sutton, R. S. (2025), *Welcome to the Era of Experience* (both quotes verified against the PDF) · Schmidhuber, J. (2009), *Driven by Compression Progress* · Silver, Singh, Precup & Sutton (2021), *Reward is enough*, Artificial Intelligence 299 · Zahavy et al. (2023), *Diversifying AI: Towards Creative Chess with AlphaZero*
- Platonic Representation Hypothesis — [arXiv 2405.07987](https://arxiv.org/abs/2405.07987) · [ICML](https://proceedings.mlr.press/v235/huh24a.html) · contested: [Back into Plato's Cave](https://arxiv.org/pdf/2604.18572)
- Wyart — [Random Hierarchy Model, *Phys. Rev. X* 14, 031001](https://journals.aps.org/prx/abstract/10.1103/PhysRevX.14.031001) · [The Physics of Data and Tasks](https://arxiv.org/pdf/2510.06106)
- Hassabis — [*Daedalus*](https://direct.mit.edu/daed/article/155/1-2/34/137129/AI-as-the-Ultimate-Tool-for-Science-A-Conversation) · [All-In transcript](https://podcasts.happyscribe.com/all-in-with-chamath-jason-sacks-friedberg/google-deepmind-ceo-demis-hassabis-on-ai-creativity-and-a-golden-age-of-science-all-in-summit) · [Nobel lecture](https://www.nobelprize.org/uploads/2024/12/hassabis-lecture.pdf)
- ARC-AGI — [ARC Prize: o3 breakthrough](https://arcprize.org/blog/oai-o3-pub-breakthrough) · [ARC Prize 2025 Technical Report](https://arxiv.org/html/2601.10904v1) · [The ARC of Progress towards AGI: a living survey](https://arxiv.org/html/2603.13372v1) · [ARC-AGI-3 launch coverage](https://www.mindstudio.ai/blog/what-is-arc-agi-3-interactive-benchmark)
- Chollet — [Dwarkesh](https://www.dwarkesh.com/p/francois-chollet) · [on X](https://x.com/fchollet/status/1816954290227089656) · [freethink](https://www.freethink.com/robots-ai/arc-prize-agi)
- AlphaFold / GNoME / FunSearch — [AlphaFold: Five Years of Impact](https://deepmind.google/blog/alphafold-five-years-of-impact/) · [AlphaFold 3](https://blog.google/technology/ai/google-deepmind-isomorphic-alphafold-3-ai-model/)
- Creativity-evaluation critique — [Rethinking Creativity Evaluation](https://arxiv.org/pdf/2508.05470)
- Extrapolation middle ground — [Context-Directed Extrapolation](https://arxiv.org/html/2505.23323v1)
- Next-token creative limits — [Roll the dice & look before you leap](https://arxiv.org/pdf/2504.15266)
- Project Glasswing — [Anthropic, 7 Apr 2026](https://www.anthropic.com/glasswing) *(primary source; verified)*
- Hugging Face agent intrusion, July 2026 — [technical timeline](https://huggingface.co/blog/agent-intrusion-technical-timeline) *(primary source; verified)*
- Frontier-researcher open letter on RSI — Stuart Russell, [*Guardian*, 11 Aug 2026](https://www.theguardian.com/commentisfree/2026/aug/11/openai-anthropic-google-deepmind-letter) (comment column; the letter's own wording quoted from it)

**Added in the September 2026 revision:**

- Princeton shadow evaluations — Kirgis, Kapoor, Narayanan et al., *Can AI agents conduct open-ended AI research? Early evidence from two case studies*, [arXiv 2607.27191](https://arxiv.org/abs/2607.27191) (v1 29 Jul 2026, v2 7 Aug 2026) · released artifacts, expert reviews and run logs at [cruxevals.com](https://cruxevals.com/crux/can-ai-agents-conduct-research) *(artifacts not reviewed by me; quotations are from the paper)* · press summary: [MIT Technology Review, 18 Aug 2026](https://www.technologyreview.com/2026/08/18/1142188/ai-recursive-self-improvement/), source of the Jack Clark quote
- OpenAI Navier–Stokes announcement — [openai.com/index/navier-stokes-solution](https://openai.com/index/navier-stokes-solution/) *(all agent counts, message counts, token figures and the model description are quoted from this page)*
- Priority dispute, reception and Clay status — [Wikipedia: Navier–Stokes priority controversy](https://en.wikipedia.org/wiki/Navier%E2%80%93Stokes_priority_controversy) *(read 13 Sep 2026, five days after the events; a live article, and I have relied on it for the quotations from Cordoba, Strogatz, Tao, Harris, Saha, Escher, Wiedemann, Thom, Lee and Dancso, and for the timeline of OpenAI statements)* · cost figure from [El Pais, 10 Sep 2026](https://elpais.com/ciencia/2026-09-10/un-ano-de-trabajo-de-dos-matematicos-espanoles-frente-a-88-horas-y-15-millones-de-openai-sin-nuestra-idea-la-ia-no-lo-habria-resuelto.html) · [Clay Mathematics Institute statement, 11 Sep 2026](https://www.claymath.org/news/navier-stokes-announcement)
- Strogatz — [*Wired*, 12 Sep 2026](https://www.wired.com/story/mathematician-steven-strogatz-grapples-with-ai-recent-breakthroughs)

**A note on these sources.** Three of the four are press or encyclopaedia summaries of events less than a week old, and one is a company announcement about its own unreleased model. I have said in §4 why that matters. I would normally wait for preprints and peer review before building on material this fresh. I have included it because the alternative is an argument dated to August that ignores the most relevant evidence yet produced for it.
- 2026 mathematics results — [Zvi Mowshowitz, 2026-08-03](https://thezvi.substack.com/p/openais-unreleased-model-astra-solves)
- Own prior post — [Minimum Required Core Lethalities](https://www.lesswrong.com/posts/dKcDbgdPzr2nfvPg5/jan-erik-vinje-s-shortform)