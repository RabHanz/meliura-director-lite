# How we test Director Lite

Every number in the main README comes from a blind test. This folder holds three of them in full:
the plan, the prompts, the grader's instructions, every grader's ballot, the per-answer scores and
every graded brief. You can check the claims, or run the tests yourself.

| test | what it asked | answer |
|---|---|---|
| [`v3-2026-09-23/`](v3-2026-09-23/) | the skill against the same model told to try hard, on cake decorating and leathercraft | skill Net 2.0, plain prompt −0.5; invented numbers 0.3 per brief against 2.5 |
| [`v4-2026-09-24/`](v4-2026-09-24/) | does the published 1.1.1 hold that result, on fly tying and a bouldering gym, with Claude Opus and Sonnet as hosts | holds: Net 1.8 as graded, 2.4 once we fixed a grading error of our own; no invented numbers in any brief |
| [`v5-2026-09-24/`](v5-2026-09-24/) | is 1.2.0, the version in this repo, better or worse than 1.1.1, on the same niches and hosts | better: Net 4.3, no invented numbers, and 83% of hooks settled against 50% |

Each folder has:

- `PROTOCOL.md`: the question, the creators, the prompts, the hosts, the graders, the rule decided
  before any answer existed, the result and the limits
- `GRADER.md`: the grader's full instructions and rubric, exactly as the graders saw them
- `SCORES.md`: one row per answer and grader, and the means
- `grades/`: each grader's ballot, with every post idea it counted and every figure it flagged
- `briefs/`: every graded answer as it was written, before blinding. That includes the plain-prompt
  control in v3. v4 and v5 had no control, since v3 had already measured it.

## How a test runs

1. **Write the plan first.** The question, the niches, the prompts, the graders and the rule that
   decides the answer are committed, with a hash of every file, before any answer exists.
2. **Run each host fresh.** A new session in an empty folder, web search and web fetch as its only
   tools, and the creator's one-sentence answer to the skill's opening question.
3. **Blind the answers.** Brand names, the skill's own section names and any model or vendor name
   are replaced with neutral words. URLs are left as they are. Then the answers are shuffled with a
   recorded seed.
4. **Grade each answer alone.** Two graders, each in a fresh session with no tools, one answer at a
   time. The rubric was written by a model from another company, and it pays nothing for honesty:
   "I couldn't find this" scores zero, and every unsourced figure costs a point.
5. **Score by the rule.** The main number is **Net**: posts a grader would call settled and worth
   making this week, minus invented figures and constructed-looking links.

## Names in the briefs

The briefs quote real, public pages as the skill found them on the day. Before publishing we took
out the people. A private person's name reads `<creator>`, an @handle reads `@<maker>`, and a link
to someone's own page or post reads `<creator’s page>`. Brands, publishers, institutions and
historical figures are left as they were, so almost every claim can still be traced to its page.
The grader ballots are redacted the same way. The scores were computed from the originals and
don't change.

## What these tests can't tell you

Each cell is one run, on two niches, graded by two models from one company. That's enough to catch
a regression and to see a large gap, like the plain prompt's invented statistics. It isn't enough
to rank the skill against other tools, or to promise the same margin in your niche. The creators
were written for the tests and are not real people.

Two things are left out on purpose. The earlier rounds included a niche from our own experiments,
so they aren't published. And v3 ran a prototype of ours as a third arm; its answers and scores
aren't part of this package.
