# Director Lite

**A free creative director for your niche.** Tell it what you make. It reads what your niche is
publishing this month, finds what's working in other niches, and hands you a brief you can make
this week, down to the cover and every slide.

## What you get back

Here is part of a real brief, lightly trimmed. It was written for someone who makes carousels about
AI coding agents for technical founders:

> **Working elsewhere: a ceramics studio's glaze tests.** Each glaze experiment is documented as a
> repeatable test: the result, how the glaze was mixed and applied, the firing program, smooth and
> textured versions.
>
> **Your version: "Agent Lab #014."** Task, model, context files, permissions, tools, how it was
> checked, the outcome, and what changed on the next run. Slides: setup, run, failure, adjustment,
> second run, conclusion.

Anyone testing coding agents fights the same problem a potter does: too many things changing at
once. The skill saw that and turned a glaze log into a weekly series.

Every brief gives you:

- one post to make first, briefed to the cover, the slides and a written opening line
- ideas that already work in other niches, rewritten for yours, with the real page beside each and
  a note on how much is known about how it did there
- what's moving in your niche right now, each point dated, and a line on whose conversation it is
- well-made work worth studying, and what to take from it
- the words and topics that keep coming up, each with where it came from
- a numbered source list, so every claim traces back to a page you can open

## Why not just ask your AI for content ideas?

We tried exactly that, blind. Same model, same creator, one answer with this skill and one from a
plain "try hard, give me your best ideas" prompt. The graders didn't know which was which.

With the skill, the briefs had more posts a creator would actually make that week, and far fewer
invented numbers: 0.3 per brief against 2.5 for the plain prompt. It cites a page for every claim,
and when it can't find something it writes "unknown" instead of making it up.

Every release gets the same blind test before it ships. Version 1.2, the one here, went up against
1.1.1 on the same two niches. Graders found about four posts per brief they'd make that week, up
from about two and a half, and not one invented statistic in any brief. Most of the gain came from
hooks: 1.2 writes the opening line out instead of describing its shape.

The prompts, the rubric, every score and every brief are in [evals/](evals/).

## Works best on

Claude (Opus or Sonnet) and GPT-5.6 Sol, with web search on. That's where our tests showed the
difference. It needs to browse, because the whole point is reading what's live this month. On Gemini,
switch on Google Search grounding first.

## Get sharper briefs

**Give it your eyes.** Most AI browsers read a page's text and can't see the pictures. When it asks,
send five to ten screenshots of covers, some yours and some from your niche that you rate. If your
assistant reads images, the craft notes get noticeably better.

**Tell it what you're working with.** The goal, the format, the photos or products you have, how
much time you've got. Or just say "assume" and it will pick sensible defaults and tell you which.

**Pick a depth.** Standard reads about 25 pages and suits most weeks. Say "quick" for a dozen-page
top-up in a niche you've briefed before, or "deep" for about 40 when you're pitching a new client.
In our tests a standard brief took the model five to eleven minutes of real reading.

## Install

The skill is the `niche-director-lite/` folder. Keep its three files together.

**Claude Code**

```bash
git clone https://github.com/RabHanz/meliura-director-lite.git
mkdir -p ~/.claude/skills
cp -r meliura-director-lite/niche-director-lite ~/.claude/skills/
```

Then say: *"Use niche-director-lite. I make …"*

**Claude apps (claude.ai and desktop).** Zip the `niche-director-lite` folder and upload it under
Skills in your settings.

**Codex CLI.** Copy the folder into `~/.codex/skills/`.

**Any other assistant that can browse.** Paste the three files into a new chat, `SKILL.md` first,
then tell it your niche.

## Want it to see every cover?

[Meliura Director](https://meliura.com) is the hosted version. It looks at the covers themselves,
scores the craft separately from the reach, and keeps your brief fresh every Monday.

## New in 1.2

- Choose quick, standard or deep. Standard is the default and reads about 25 pages.
- Every idea borrowed from another niche says what's known about how it did there: seen in use,
  reported popular, beat its author's usual posts, or a measured result.
- Coverage is counted in independent sources, and the brief tells you when they were narrow.
- Reach keeps a raw count apart from how a post did against its author's other posts.
- Each hook comes written out as a line, with a blank wherever your own number belongs.
- A numbered source list, and a last check of every claim against it before the brief is handed
  over.
- An optional line about your goal, format, materials and time. Say "assume" to skip it.

## Licence

[PolyForm Internal Use License 1.0.0](LICENSE). Use it for your own work and your clients'. Don't
resell it, rebrand it or republish it.

Versions up to 1.1.1 were released under the MIT licence, and those copies keep it.

Made by [Meliura](https://meliura.com).
