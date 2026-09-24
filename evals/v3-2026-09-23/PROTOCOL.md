# Test v3, 23 September 2026: the skill against a plain prompt

**Question.** On two niches no earlier test had used, which answer gives a creator more posts they
would make this week, with less invented: the skill, or the same model told to try hard?

**Niches.** Two constructed creators, written for the test. Neither is a real person.

- cake decorating: *"I decorate celebration cakes at home — buttercream piping, vintage-style heart
  cakes and the odd sculpted cake — and post the process for other home bakers who want their cakes
  to look bakery-made. Instagram and Pinterest, stills, carousels and short process reels."*
- leathercraft: *"I hand-stitch small leather goods — wallets, card holders, key fobs — at a bench
  in my garage, and post the process for beginners learning the craft and for people who might buy
  one. Instagram and Pinterest, stills, carousels and a few short reels."*

**Arms, per niche.** Both on Claude Opus 5.5 through the `claude` command-line tool, a fresh
session in an empty folder, web search and web fetch as the only tools.

- **skill**: an earlier, unpublished draft of the skill (the version before 1.1), in this frame:

  ```text
  You have the skill folder below open in your agent. Follow it.

  Today is 23 September 2026.

  ===== SKILL.md ===== … ===== THE-METHOD.md ===== … ===== THE-BRIEF.md ===== …

  ===== the person you are working for =====

  They have already answered the skill's opening question. Their answer:

  > <the creator's words>

  Do the work and write the brief. Use your web search and web fetch tools. You have no other
  tools, no keys, no database and no access to anything of the skill publisher's. Everything you
  cite must be something you opened.
  ```

  If an answer came back under 1,500 characters, the harness replied once, as a buyer would, and
  let the session continue. Neither skill run needed it.

- **plain prompt**, word for word:

  ```text
  Today is 23 September 2026.

  You are helping one creator work out what to post next. Take this seriously and spend real
  effort on it: use your web search and web fetch tools extensively, open a lot of pages, and come
  back with a thorough, specific brief rather than a quick answer. Aim for something substantial —
  comparable to an hour of a good strategist's work.

  Here is the creator, in their own words:

  > <the creator's words>

  Give them what to post next, with whatever supporting research, references and reasoning you
  think makes it useful. You have no tools beyond web search and web fetch.
  ```

**Grading.** Every answer was blinded before a grader saw it: the publisher's name, the skill's own
section names and any model or vendor name were replaced with neutral words, so a grader could not
tell which arm wrote it. The answers were shuffled with a recorded seed (`c0b3b92362cd165c`). Two
graders, Claude Opus 5.5 and Claude Sonnet 5, each read every answer in its own fresh session with
no tools. The grader prompt is `GRADER.md`, byte for byte. Its rubric was written blind for an
earlier round by GPT-6 Astra, a model from another company, and it pays nothing for honesty: an
honest "I couldn't find this" scores zero, and a fabrication costs a point.

**The main number** is Net: the posts a grader counted as fully settled and worth making this week,
minus the unsourced figures and constructed-looking links it found.

**Pre-registration.** The plan, the arms, the grader prompt and every script's hash were committed
before any output existed (plan sha256 `35ccd669859b252507e5d8e9c599925a5bd24213128f9aecc0b389ffcc00eb0b`).
That plan also covered a third arm, an internal prototype, and a buyer panel. Neither is part of
this package, and the decision rule it registered compared the prototype against these two arms,
so it is not restated here. What it fixed for the two arms here: the niches, the frame and prompt
above, the hosts, the two graders, the blinding, and Net as the main number.

**Result** (`SCORES.md`): skill Net 2.0, plain prompt −0.5. Invented numbers per answer: skill 0.3,
plain prompt 2.5. The plain prompt scored higher on the rubric (88 against 85) and filled every
section it promised; the skill's section on well-made, little-seen work was empty in both briefs,
because a text-only browser cannot judge a picture. Version 1.1 asks the creator for screenshots
for that reason.

**Limits.** Two niches, one host model, two graders from one company, one run per cell. The
graders and the host are the same model family, so the Sonnet grader's column is the check that
matters; it keeps the order (skill 1.5, plain prompt 0.5). A second round (test v4) re-checked the
published 1.1.1 text on two more niches.
