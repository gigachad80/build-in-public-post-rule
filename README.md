# build-in-public-post-rule

A skill that turns a product changelog into **build-in-public posts**, and, just as
importantly, tells you what *not* to publish.

It exists to counter the default instinct to "document everything" and post daily. The
rule it enforces is simple: **more public does not equal more business.** Share only what
actually brings customers; keep the rest private.

## Table of contents

- [What it does](#what-it-does)
- [When it triggers](#when-it-triggers)
- [Who it's for](#who-its-for)
- [The core rule](#the-core-rule)
  - [Share only these three things](#share-only-these-three-things)
  - [Keep private](#keep-private)
- [Pick your path first](#pick-your-path-first)
- [What your changelog needs](#what-your-changelog-needs)
- [The share test](#the-share-test)
- [The workflow, step by step](#the-workflow-step-by-step)
- [Hook types](#hook-types)
- [Worked example](#worked-example)
- [How it compares to other build-in-public skills](#how-it-compares-to-other-build-in-public-skills)
  - [Which one should you choose](#which-one-should-you-choose)
- [Rules of thumb](#rules-of-thumb)
- [Files](#files)
- [Install](#install)
- [Credits](#credits)

## What it does

Given a changelog (or raw material you turn into one), the skill:

1. **Mines post ideas from what was actually shipped**, never from a blank page.
2. **Classifies each change** and runs a "share test" to decide whether it is postable.
3. **Drafts posts from the survivors** in four parts (Hook, Body, Visual, CTA), using a
   hook type matched to the entry.

It also works out *where* the changelog comes from before doing anything else (see
[Pick your path first](#pick-your-path-first)).

## When it triggers

Use it whenever the request is promotional or "build in public" flavoured:

- "XYZ Days" updates and progress posts
- Content or post ideas to promote a product
- Launch or milestone posts
- A posting calendar for a founder or a SaaS

## Who it's for

This skill is for a founder who is building in public and would rather convert than
broadcast. It fits best when there is something real to protect and something real to
ship.

**Best fit**

- **Solo and indie founders**, especially SaaS. The skill exists because the moat is easy
  to leak. If your edge is your workflow or your roadmap, it is written for you.
- **Developer-founders who ship.** Paths A and B assume a changelog or merged work to
  mine, such as a repo or GitHub activity.
- **Small teams with engineering activity but no marketing motion.** They already
  generate a changelog; they just need the few posts worth publishing pulled out of it.
- **Non-technical or no-code founders.** Path C is built for them: no repo and no
  changelog, so the skill asks for the raw material directly.

**Who benefits most**

Founders with real competitor risk, people who tried build-in-public and attracted
learners and copycats instead of customers, and builders who do not want to become
full-time content creators.

**Who should skip it**

Anyone documenting everything as a personal-brand exercise, teams that want a high-volume
daily content calendar, and anyone who wants a draft generator rather than a decision
rule. The skill actively fights all three.

**Quick test**

If you can name the thing you must keep private, and you have shipped something you could
post about, this skill is for you.

## The core rule

> More public does not equal more business.

Sharing everything attracts copycats, people who only want to learn from you, and people
who do not care, and it rarely converts. Especially for a new product, the best move is
often to stay quiet and share only what brings more business.

### Share only these three things

1. **What can go mega-viral**: reach plays and top-of-funnel attention.
2. **The workflows that win you customers**: the how-to that makes someone buy, not the
   generic advice that makes someone copy you.
3. **The parts that make sense**: hit your goal first while documenting from day 1, then
   publish only the slice worth publishing.

### Keep private

- The full playbook, mechanics, and moat of the product
- Numbers and details that only invite copycats
- Anything that teaches a competitor more than it wins you a customer
- Daily "we shipped X" noise that neither converts nor travels

## Pick your path first

Post ideas always come from a changelog, but *where* that changelog comes from depends on
how far along the product is. The skill checks this before anything else.

| Path | Situation | What the skill does |
|---|---|---|
| **Path A** | Product already built or launched, changelog exists | Skips building it; reads every entry and mines the existing back-catalogue in one pass |
| **Path B** | Product still being built, no changelog yet | Builds the changelog from merged PRs as you ship, then mines it |
| **Path C** | No changelog and no repo to pull one from | Asks you for the raw material directly, in one short batch, then builds the changelog from your answers |

**Path C** covers the solo founder, the no-code product, or the idea that has not shipped.
Instead of stalling, the skill asks three questions (what did you build or change
recently, what did a customer ask for or what did you fix for them, and any result worth
showing such as a number, a before/after, or a launch), then builds the changelog from
those answers.

All three paths finish the same way: classified entries turned into ready-to-post ideas.

## What your changelog needs

The skill reads whatever entries you give it. It does not compare against history, so a
changelog with only the latest entries is enough. You do not have to keep the old
versions for the skill to work.

Two things matter more than history:

- **Detail beats completeness.** Each entry should say what changed and why it matters,
  in plain language. "Fixed the checkout button that failed on mobile" gives the skill
  something to work with. "v1.2.3 fixed bugs" gives it almost nothing.
- **Bug fixes rarely become posts.** Fixes are classified as "Fixed", which the rule
  marks as rarely postable, and only when the story travels. Three or four routine fixes
  will likely give you one post at best, and often none. That is the rule working as
  intended, not the skill failing.

Keeping old changelogs gives you a bigger bank of ideas and helps you avoid repeating
yourself, but it is optional. The skill only needs the entries you hand it, with enough
detail to say what changed and why.

## The share test

Each entry is tagged by its changelog section, then judged:

| Changelog section | What it is | Post it? | Angle |
|---|---|---|---|
| **New** | a new capability | usually yes | launch or reach post |
| **Improved** | a better workflow | yes, if it wins customers | "here's how we did X" |
| **Fixed** | a bug fix | rarely | only if the story travels |
| **Under the hood** | internal plumbing | no | keep private |

Anything that only teaches a copycat, or leaks the moat, stays private, no matter how
good it looks.

## The workflow, step by step

**Step 1. Build the changelog from what you actually shipped.**
Know four inputs first: the **repos** (GitHub org plus product repos), the **product
scope** (keywords or paths that mark a change as relevant, and those that mean skip), the
**timezone** (GitHub timestamps are UTC, so convert for display), and the **product name**
(shown in the summary line). Entries come from **merged PRs in the date window**,
filtered to your product's scope. Write each as a user-facing entry with a plain-English
**title** (the job-to-be-done), **contributors** (who plus the PR link), and **details**
(2 to 3 sentences, no jargon). When in doubt, skip; a shorter accurate changelog beats a
padded one. Record the *why* next to the *what*, because that is where the post angle
lives.

**Step 2. Classify each entry, then run the share test.** (table above)

**Step 3. Turn survivors into posts.** Each post has four parts:

1. **Hook**: the change, framed to travel. Pick the hook type that fits the entry.
2. **Body**: the business-relevant lesson, meaning what changed and why it matters to the
   reader.
3. **Visual**: what to show, such as a screenshot, a before/after, or a short clip. Name
   the asset and say why that image earns the scroll. Text cards and caption images get
   one bold accent colour so they stand out in the feed.
4. **CTA**: one explicit next step, matched to the goal. For reach, ask for a follow. For
   a customer-winning workflow, invite the reader to try it, book a demo, or grab the
   template.

Do not pad the list. A few strong posts beat thirty daily updates.

## Hook types

Pick one that fits the entry:

| Hook | Best for | Shape |
|---|---|---|
| **Controversial** | a change that pushes against how the market works | "Everyone does X. We killed it." |
| **Bold** | New entries, big swings | a flat, confident claim, no hedging |
| **Relatable** | Improved workflows, a pain you also felt | "We used to do this by hand. Never again." |
| **Viral** | reach plays such as milestones and striking results | lead with a number, a before/after, or a surprise |
| **Visual** | anything with a screenshot or design payoff | the image leads, with one bold accent colour |

## Worked example

The skill ships with a worked example to show the whole flow end to end.

- **Changelog entry:** "Translated replies no longer disappear from chat", a user-visible
  bug where translated replies vanished mid-chat, caused by a race
  between the translation stream and the message store.
- **Share test:** it is a **Fixed** entry, which the table marks "rarely", but it clears
  the test because the story travels (a user-visible failure with a clean cause).
- **Finished post:** a *Relatable* hook ("Our users watched their own messages vanish. We
  fixed it, and here's why it happened"), a body explaining the race and the fix, a
  before/after screen recording as the visual, and a CTA aimed at builders handling
  streaming translation.

The example doubles as the rule's own stress test: most fixes stay private, but the skill
shows you how to spot the rare one that earns a post.

## How it compares to other build-in-public skills

Several build-in-public skills already exist. They mostly fall into two camps: **post
generators** that turn GitHub activity into drafts, and **channel playbooks** that teach
formatting and timing for LinkedIn and X. This skill sits in a third camp: a **decision
rule** about whether to post at all, and what to keep back.

| Skill | Focus | Best for | How it works |
|---|---|---|---|
| **build-in-public-post-rule** (this skill) | Whether and what to post, business-first restraint | Founders protecting a moat; turning a changelog into a few sharp posts | Rule plus a changelog-driven workflow, three paths (A/B/C), four-part posts with matched hooks |
| **alinaqi/maggy `build-in-public`** | Best practices for sharing engineering work publicly | Engineers and CTOs posting technical work | Channel-specific tactics for LinkedIn and X, posting times, anti-patterns, measurement |
| **jeromeetienne/skillmd_collection `build_in_public`** | Turning recent GitHub activity into posts | Developers who want quick `#buildInPublic` drafts | Uses the `gh` CLI to scan commits and releases, then drafts one to three posts |
| **vindicatenyc/build-in-public-plugin** | Generating posts from coding sessions | Claude Code users who want session-based updates | A plugin with hooks and scripts that auto-tracks sessions and drafts posts |
| **JayantChopra/stanley-mcp-playground `build-in-public`** | GitHub activity into posts through an MCP | Users who already run the Stanley MCP | MCP-driven flow that drafts per platform and can schedule into slots |

Sources: the public listings for [alinaqi/maggy](https://github.com/alinaqi/maggy),
[jeromeetienne/skillmd_collection](https://github.com/jeromeetienne/skillmd_collection),
[vindicatenyc/build-in-public-plugin](https://github.com/vindicatenyc/build-in-public-plugin),
and [JayantChopra/stanley-mcp-playground](https://github.com/JayantChopra/stanley-mcp-playground).

### Which one should you choose

- If you want a **generator** that scans your repos and hands you drafts, pick
  jeromeetienne's `build_in_public`, the vindicatenyc plugin, or the Stanley skill.
- If you want **per-channel formatting and posting-time advice** for an engineering
  audience, pick alinaqi's `build-in-public`.
- If your real problem is **deciding whether to post and what to hold back**, and you want
  a repeatable way to turn a changelog into a small number of high-conviction posts, this
  skill is the one to reach for.

You can also use them together. Run this skill first to decide *what* is worth saying,
then hand the chosen changes to a generator or a channel playbook to shape the draft.

## Rules of thumb

- Prefer fewer, sharper posts over a daily drumbeat.
- Document from day 1, but publish selectively and late.
- If a post would not bring more business, do not publish it.
- SaaS founders: be extra conservative, because the moat is easy to leak.

## Files

```
build-in-public-post-rule/
├── SKILL.md    # the skill itself: frontmatter, rule, and workflow (this is what loads)
└── README.md   # this documentation file (for humans; not read by the skill loader)
```

The skill is self-contained in `SKILL.md`; there are no scripts, references, or assets.
The README is documentation only and is not part of the loadable skill.

## Install

Drop the `build-in-public-post-rule/` folder into your skills directory. The folder name must match
the `name:` field in the SKILL.md frontmatter (`build-in-public-post-rule`) for the skill to load.

## Credits

- The core rule and its framing are adapted from a note by **Suprava Sabat**
  ([@Suprva02](https://x.com/Suprva02)) on the risks of building a business in public,
  quoted in full inside `SKILL.md`. See the
  [original post on X](https://x.com/Suprva02/status/2103794798390108391).
- The changelog method is adapted from the **changelog-report** skill, which inspired this
  workflow.
