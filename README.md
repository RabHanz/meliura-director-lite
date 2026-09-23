# Director Lite

**A free creative director for your niche.** Tell it what you make. It reads what your niche is
publishing this month, finds what's working in other niches, and hands you a brief you can shoot
this week, down to the cover and every slide.

## What you get back

Here is part of a real brief, written for a freelance social media manager who runs the Instagram
for a bouldering gym:

> **Working elsewhere: the chess daily puzzle.** One position shown from the solver's side, a
> two-word instruction, the answer held back. Difficulty climbs through the week.
>
> **Your version: "Yellow to move."** A photo from where a climber stands at the start, looking up
> at the first holds. One short instruction across the bottom. Slide 2: the first two moves, marked.
> Slide 3: the crux. Slide 4: where to find it on the floor. Run it as a weekly ladder, one colour
> harder each post.

Climbers already call routes problems. The skill spotted that a chess puzzle works the same way and
turned it into a series the gym can post every week.

Every brief gives you:

- one post to make first, briefed to the cover, the slides and the opening line
- ideas that already work in other niches, rewritten for yours, with the real post beside each
- what's moving in your niche right now, each point dated and linked to the page it came from
- well-made work worth studying, and what to take from it
- the words and topics that keep coming up, each with where it came from

## Why not just ask your AI for content ideas?

We tried exactly that, blind. Same models, same niches, one arm with this skill and one with a
plain "give me your best ideas, try hard" prompt. Graders from three AI companies scored the results
without knowing which was which.

With the skill, the briefs had more posts a creator would actually make that week, and about eight
times fewer invented numbers (0.3 per brief against 2.5). It cites a page for every claim, and when it
can't find something it writes "unknown" instead of filling the gap. A brief
takes the model five to thirteen minutes of real reading.

## Works best on

Claude (Opus or Sonnet) and GPT-5.6 Sol, with web search on. That's where our tests showed the
difference. It needs to browse, because the whole point is reading what's live this month. On Gemini,
switch on Google Search grounding first.

## Get sharper briefs

Most AI browsers read a page's text, and they can't see the pictures. So give it your eyes: when it
asks, send five to ten screenshots of covers, some yours and some from your niche that you rate. If
your assistant reads images, the craft notes get noticeably better. It will tell you plainly when a
section had nothing to go on.

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

## New in 1.1

- The brief opens with the one post to make first.
- Ideas from other niches come straight after, with the reference beside each one.
- The craft section now works from your screenshots, so it rarely comes back empty.
- Opening lines never put a made-up statistic in your mouth.

## Licence

MIT. Use it, change it, share it.

Made by [Meliura](https://meliura.com).
