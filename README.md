# Niche Director Lite

A free skill that makes your AI assistant act as a creative director for one niche.

You tell it what you make and who it's for. It goes and reads what is actually being published in
your niche this month, looks at how other niches build their posts, and hands back a brief:

1. **One post to make first**, briefed down to the cover, the slides and the hook.
2. **Patterns that work in other niches, rewritten for yours**, each with the real reference
   beside it.
3. **A few more posts** worth making, ranked.
4. **What is moving** in your niche right now, each line dated, with the page it came from.
5. **Well-made work**, with how each piece is built and what to take from it.
6. **Words and topics**, each with where the claim comes from.

Every reference is a page it opened, and every number is one it read. When it doesn't know
something, it writes "unknown" instead of guessing.

It does not write your posts, predict how they will do, or rank accounts.

## Where it works

We tested it blind in September 2026 on five niches, with three graders from three different AI
vendors.

| host | result |
|---|---|
| Claude Opus, Claude Sonnet (with web search and fetch) | works |
| GPT-5.6 Sol (with web search) | works |
| GPT-6 Astra | runs, but no better than asking it to try hard |
| Gemini without paid search grounding | does not run |

On the hosts where it works, a brief carried about three posts a creator would actually make that
week, and fewer made-up statistics than the same model given a plain "try hard" prompt. A brief
takes six to thirteen minutes of the model's time.

**It needs browsing.** Without web search it will say so and stop.

**It mostly can't see pictures.** Browsing tools read pages as text, so on most hosts the model
can't judge how a cover looks. It will ask you for screenshots of five to ten covers, some of
yours and some from your niche that you think are good. If you send them and your host reads
images, the craft section gets much better. If you don't, that section stays short and says why.

## Install

The skill is the `niche-director-lite/` folder: `SKILL.md` plus the two files it reads,
`THE-METHOD.md` and `THE-BRIEF.md`. Keep all three together.

**Claude Code**

```bash
git clone https://github.com/RabHanz/meliura-director-lite.git
mkdir -p ~/.claude/skills
cp -r meliura-director-lite/niche-director-lite ~/.claude/skills/
```

Then ask: *"Use niche-director-lite. I make …"*

**Claude apps (claude.ai, desktop)**: zip the `niche-director-lite` folder and upload it as a
skill in your settings, where your plan offers skills.

**Codex CLI**: copy the folder into `~/.codex/skills/`.

**Anything else with browsing**: paste the three files into the conversation, `SKILL.md` first,
and tell it your niche.

## What changed in 1.1

- The brief now opens with a single post to make first, instead of ending on questions.
- Patterns from other niches, rewritten for yours, come second, straight after that pick.
- The "beautiful, not yet travelled" section came back empty in most test runs, because a text
  browser can't see images. It is now built from what the model can actually establish: your
  screenshots, the maker's own description of the work, or a count printed on the page.
- The research log moved below the briefs.
- Hooks can no longer put a made-up number in your mouth.

## Licence

MIT. Use it, change it, share it.

---

By [Meliura](https://meliura.com). The hosted Meliura Director does the visual half: it looks at
the covers themselves.
