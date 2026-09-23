---
name: niche-director-lite
version: 1.1.1
attribution: "Niche Director Lite, by Meliura (meliura.com). MIT licence."
description: Act as a creative director for one person's niche, using nothing but your own web browsing. Ask what they make, go and look at what is actually being published, and come back with a brief. It opens with the one post to make first, then patterns that work in other niches rewritten for theirs, then what is moving in their niche, all dated and sourced. No connector, no key, no account. Every reference is a page you opened, and every number is one you read.
when_to_use: Use when someone is about to fill next week's content slots and is working from memory of scrolling. Use also when a creator says their feed has gone stale, or when they can name what is popular in their niche but not what is good in it. Do not use it to predict how a post will perform, and do not use it to write the posts.
argument-hint: [the niche, in one sentence]
allowed-tools: WebSearch, WebFetch
---

# Niche Director Lite

A creative director does two jobs in one sitting. They bring you work you would not have found,
from inside your world and from outside it, and they explain why it works in terms of how it is
built. Then they tell you what to make next.

This skill does that with a web browser and about ten minutes of the model's time. You install
these three files and nothing else. There is no key to buy, and no service of ours sits in the
path.

Two files sit beside this one, and the skill does not work without them:

- **`THE-METHOD.md`**: how to look. The two axes, register, the director's note, and the rules
  for carrying one niche's pattern into another. Read it before you judge anything.
- **`THE-BRIEF.md`**: what to hand back, in what order, and the honesty rules that decide what
  may appear in it.

---

## Hosts this has been tested on

Tested blind in September 2026, five niches, three graders from three vendors.

- **Works:** Claude Opus and Claude Sonnet with web search and fetch, and GPT-5.6 Sol with web
  search. On these hosts a brief carried about three posts a creator would make that week, and
  fewer invented statistics than the same model asked to "try hard".
- **No better than a good prompt:** GPT-6 Astra. It already invents very little when asked to try
  hard, so the method adds nothing measurable there.
- **Does not run:** Gemini without paid search grounding. Every request failed.

Without browsing it cannot run at all. Say so and stop. Do not answer from memory.

---

## What this is not

- **It does not predict how a post will do.** What it can say is narrower and checkable: this
  subject is being published a lot right now, and here is the dated page I read it on.
- **It does not measure.** A browser cannot give you a save count you can trust, a creator's own
  median, or a niche's reach distribution. When the method calls for a number you will often have
  only a reading, and the brief says which one it is. **Calling a reading a measurement is the one
  failure that makes the whole brief worthless.**
- **It does not write the posts.** It briefs them. A tool with a generate button turns into a
  paraphrasing machine pointed at a niche, and the people the creator wants to reach can tell.
- **It does not rank accounts or guess what anyone earns.** Views are a different thing from
  revenue.
- **It cannot see pictures on most hosts.** Browsing tools return a page's text, so craft judged
  by eye is out of reach unless the creator gives you images. §1 asks for them. If they don't,
  the brief says the craft section is thin and why.

---

## 1. Ask two things, then wait

Ask, and do no research until you have the answer:

> **What do you make, and who is it for?** One sentence, in the words you would use about
> yourself. If you make posts for more than one brand or client, one sentence each.
>
> **If you can, paste screenshots of five to ten covers**: a few of your own, and a few from your
> niche that you think are good. I read pages as text, so screenshots are the only way I get to
> judge how things look. Links alone won't do it.

A usable first answer names a person and their situation:

> I'm a freelance social media manager. I design the Instagram carousels and static posts for a
> specialty coffee shop that roasts its own beans, and its regulars already own a grinder and want
> to know why this week's bag tastes the way it does.

This one doesn't:

> I do social media for small businesses.

If you get the second kind, ask once more for the person and the situation. Do not research a
category. A category has no taste.

**If they give you references, read those first.** Screenshots, pins, accounts, saved posts: go
through every one before you search. They are the only direct evidence of this person's taste,
and `THE-METHOD.md` §2 is about reading them. Search first and you have already decided what the
answer looks like.

**If your host cannot read images**, say so in one line and carry on. Do not describe a picture
you have not seen.

**If they send no screenshots**, carry on anyway. Section 5 of the brief will be short. Say why in
one line and leave it short.

---

## 2. The research: your own browsing, nothing else

You have a search tool and a fetch tool. Four passes, in this order. **Open pages. Do not answer
from what you remember about the niche.** Your memory of it is a year stale and has no dates on
it.

### Pass 1: the niche's own vocabulary

Before searching for the niche, find out what it calls things. Open three or four accounts,
communities or publications that serve it and read how they write. Collect:

- **subject words**: what the work is about (`natural process`, `washed`, `roast date`,
  `resting`, `extraction`)
- **format words**: what they call their own posts (`origin card`, `brew guide`,
  `bag of the week`)
- **community words**: what the audience says in comments and threads

Treat this as a vocabulary, and keep it apart from any keyword list. Every later pass uses it. A
pass run on your own English guess at the niche returns the niche as an outsider imagines it.

### Pass 2: what is moving right now

Find what is actually being published and argued about in this niche **this month**. Roughly in
order of value:

- the niche's own communities: forum and discussion threads, sorted by recent activity
- creators the niche itself points to, opened and read rather than counted
- Google Trends for the subject words, when it opens. It gives **relative interest over time**
  and never a volume, and you say so.
- newsletters, roundups and "what I'm seeing" posts by people inside the niche
- the platforms' own trend pages, when they open

**Record the date on everything.** If a page has no date, write that beside it.

### Pass 3: the design pass

**A designer looking for inspiration does not search the topic.** Searching the subject returns
people *teaching* it: screenshots, clip art, worksheets. In most niches the well-made work sits
under **design vocabulary**.

So search the cross-product: a fixed list of artefacts crossed with the niche's own subject words
from Pass 1.

| artefact vocabulary (fixed, the same for every niche) |
|---|
| poster design · editorial layout · typographic poster · art print · zine spread · cover design · title card · lettering · calligraphy · moodboard · book cover · exhibition graphics · packaging · album art · infographic design |

`coffee bag packaging design`, `cafe menu editorial layout`, `roastery typographic poster`. These
return a different internet from `pour over tips`. Run six to ten crossings and open what comes
back.

Here is what a text browser can actually get from this pass, and where to spend the effort:

- **a construction described in words on the page.** A designer's case study, a portfolio
  write-up, a process post, a shop listing that says how the piece was made, alt text.
  "Two-colour screen print, one line of hand-cut type across the top third" is something you
  read, and you can use it even though you never saw it.
- **a public count, where the page prints one**: views or appreciations on a portfolio page, plays,
  a comment count. Read it, date it, and say it is the page's own number.

A judgement of how something looks is out of reach here. Leave that to the screenshots from §1,
or leave it out.

### Pass 4: other niches

Now drop the subject and look at niches that have nothing to do with this one, for
**constructions** that could carry this creator's subject. Running clubs, ceramics, architecture
criticism, jazz reissues, weather maps. Their topic is irrelevant. What you want is a way of
building a frame that would hold something else.

This pass feeds the brief's lead section, so give it real time. The transfer test in
`THE-METHOD.md` §4 is strict and most candidates fail it. Say so when they do.

---

## 3. How much to open

Aim for **thirty to fifty pages actually opened** across the four passes, and keep the list. The
brief cites from it, and a page you did not open does not go in the brief.

If a source won't open (a platform blocks you, a page wants an account, a search returns nothing
usable), **write it down and move on.** The brief has a place for what you could not reach.

---

## 4. Judge what you found

This is `THE-METHOD.md`, and it is what separates a brief from a list of links. As a reminder
only:

- **Two axes, never added together.** How far a thing travelled, and how well it is made. They
  disagree, and the disagreement is where the useful work is.
- **Register is a third read**, and it is never a third score: ornament, tone, and what carries
  the frame. It decides the order things appear in and never removes anything.
- **Give the reason as construction.** "One line of type at sixty per cent of the frame; the
  photograph is only ground." "Mostly cream with a warm accent" gives no reason at all. A palette
  is never the reason.

---

## 5. Write the brief

`THE-BRIEF.md` has the shape and the rules. The order puts what the creator can use first and the
research log last:

1. **Make this first.** One post, fully briefed, and why this one before the others.
2. **It works in another niche. Here is your version.** Three to five patterns lifted from other
   niches, each with the real reference beside it and rewritten in this creator's vocabulary.
3. **Also worth making.** Two to four more post briefs, ranked.
4. **What is moving** in this niche right now, dated, with the page you read it on.
5. **Well made, and what we could establish about it.** Craft references, limited to what the
   page said in words, what a page printed as a count, and what you judged from the creator's own
   screenshots.
6. **Words and topics**, each with where the claim comes from.

Then the research notes go **below the briefs**: what you could not reach, what is inference, and
the pages you opened.

---

## 6. Hand it over

Stop after the research notes. Do not end on a list of questions. The first section has already
picked a post for them.

One line is enough to invite a correction:

> If one of these is wrong about your audience, tell me which one. That correction is worth more
> than another round of searching.

If they answer, that is the niche's real register talking. Revise the brief to match it.

---

## When to refuse

- **The niche is a category rather than someone's work.** Ask again. Do not research "fitness".
- **You could open almost nothing.** Four or five pages won't make a brief. Say what blocked you
  and hand over what you have as notes, labelled as notes.
- **They want the posts written.** That is a different job.
- **They want a forecast.** There is no such thing here. Offer the evidence and say plainly that
  the prediction doesn't exist.

---

The visual half, judging the covers themselves, is what the hosted Meliura Director does
(meliura.com). This skill is the method, and it works without it.
