# Test v4, 24 September 2026: the published 1.1.1 on two new niches

**Question.** Rewording can move how a skill performs, and the numbers we had came from the
earlier draft. Does the text published as 1.1.1 hold test v3's result, improve on it, or regress?

**Niches.** Two constructed creators, never used by an earlier test. Neither is a real person.

- fly tying: *"I tie trout flies at my kitchen table, traditional wet flies and a few modern nymph
  patterns, and post step-by-step photos for anglers who want to start tying their own. Instagram
  and Pinterest, stills, carousels and a few short reels."*
- a bouldering gym's social media manager: *"I'm a freelance social media manager. I design the
  Instagram carousels and static posts for an independent bouldering gym, for members who climb a
  couple of times a week and for people nearby who have never tried it. Stills and carousels, plus
  the odd reel the gym films itself."* This one is shaped like the skill's own example (a social
  media manager for a coffee shop), so it doubles as a check that the example isn't copied.

**Arms.** The skill only, the three 1.1.1 files in v3's frame word for word (see the v3 protocol),
on two hosts: Claude Opus 5.5 and Claude Sonnet 5. No plain-prompt control this time; v3 measured
it. Same command-line harness, same tools, same stall rule; no run stalled.

**Grading.** v3's grader prompt byte for byte (`GRADER.md`, identical to v3's), the same two
graders, a fresh session per answer, no tools, shuffled with seed `d57dcee680081aa9`.

**Pre-registered decision rule**, on the mean Net over both niches, both hosts and both graders,
and mean invented numbers F:

- **regresses** if Net < 1.5 (below v3's weaker niche) or F > 0.8
- **improves** if Net ≥ 2.5 (v3's better niche) and F ≤ 0.3
- **holds** otherwise

Any rubric line more than half a point below v3's is named as a regression on that line. The plan,
the prompts and the scripts were committed before any output existed (plan sha256
`e21aa16785d31248201909482910ebe9c44cedd19439ff739decd62e37dbac6f`).

**Result** (`SCORES.md`): **holds.** Net 1.8 as graded, F 0.5, rubric 86, coverage 85% (v3: 70%).
No rubric line fell more than 0.25. The coffee example did not leak into either gym brief.

**One grading error, found after the fact, and ours.** The blinding step replaced every brand name
on its list wherever it appeared, including inside URLs. One of those brands publishes a blog the
skill cited, so two real links reached the graders as `https://www.the publisher.ai/…`. Both
graders scored them as constructed, which is the whole of v4's F. The run's own fetch log shows both pages were opened and returned content. The
blinding now leaves URLs alone. The affected answer (D002) was re-blinded with the fix and graded
again by both graders on 24 September. Neither flagged anything, and v4's mean moves to Net 2.4
with no invented numbers. `SCORES.md` shows both readings, and `grades/` keeps both sets of ballots.

**Limits.** Two niches, one run per cell, graders from one company, no control arm.
