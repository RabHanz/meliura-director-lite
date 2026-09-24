# Test v5, 24 September 2026: version 1.2.0, the version in this repo

**Question.** 1.2.0 changed the method in ten places: a note on how each borrowed idea did in its
own niche, sources counted by independence, a depth choice, raw reach kept apart from
author-relative reach, taste claims treated as things to check, an optional line about the goal
and materials, a numbered source list, a last check of every claim, and a written hook line. Did
all that make it better, or worse?

**Niches.** v4's two constructed creators, word for word (see the v4 protocol): fly tying, and a
bouldering gym's social media manager. Neither is a real person.

**Arms.** The skill only, the three 1.2.0 files in v3's frame word for word, with the day's date,
on Claude Opus 5.5 and Claude Sonnet 5. The prompt says nothing about depth, so the skill ran at
its default, standard. No plain-prompt control; v3 measured it. Same harness, same tools, same
stall rule; no run stalled.

**Grading.** v3's grader prompt byte for byte (`GRADER.md`), the same two graders, a fresh
session per answer, no tools, shuffled with seed `71b4f7629edac9c9`. The blinding leaves URLs
alone from this round on (see the v4 protocol for why).

**Pre-registered decision rule**, against v4 with its grading error fixed (Net 2.4, invented
numbers 0), on the mean over both niches, both hosts and both graders:

- **regresses** if Net < 1.8, or invented numbers F > 0.5, or coverage < 75%
- **improves** if Net ≥ 2.8 and F ≤ 0.25
- **holds** otherwise

Any rubric line more than half a point below v4's is named as a regression on that line. The plan,
the prompts and the scripts were committed before any output existed (plan sha256
`879a47e12f1bb3d4167bd0c215b00663b1b4495e703c22e06e55b5a642df2629`).

**Result** (`SCORES.md`): **improves.** Net 4.3 against v4's 2.4, no invented numbers in any of
the eight ballots, rubric 89 against 87, coverage 88% against 84%. The graders counted 83% of hooks
as settled, against 50% in v4, which is most of the gain: v4 described each hook's shape, and 1.2.0
writes the line. No rubric line fell more than 0.25. Each brief carried every new element, and each
one's final check says what it cut, mostly numbers seen only in search results. A standard brief
read 32 to 44 pages and took 5 to 11 minutes.

**What the graders still didn't like:** length spent on research notes, a "no saves seen" line
repeated under each reference when the creator sent no screenshots, and hooks with a blank for the
creator's own number, which some graders read as unfinished.

**Limits.** Two niches, one run per cell, graders from one company, no control arm.
