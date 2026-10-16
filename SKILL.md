---
name: build-in-public-post-rule
description: "Use when writing build-in-public content: progress posts, \"XYZ days\" updates, launch posts, or content/post ideas for a product. Turns your changelog (or one built from merged work) into posts, and shares only what brings business rather than noise."
---

# Build in Public: Post Rule

## When this applies

Use this whenever someone asks you to write anything promotional or "build in
public" flavoured:

- "XYZ Days" updates / progress posts
- content ideas or post ideas to promote their product
- launch or milestone posts
- a posting calendar for a founder or a SaaS

The rule below governs every one of these. It overrides the instinct to share
more, post daily, or "document everything".

## The core rule

More public ≠ more business.

Sharing everything about your build attracts copycats, people who only want to
learn from you, and people who don't care, and it rarely converts. The best
thing you can do for the business, especially when new, is to keep your mouth
shut and share only what brings you more business.

> "every-time a reel pops up on my feed with 'build in public till i hit $10,000
> or wtv thing'
>
> i know it's gonna go down in a few months
>
> i have seen this happen too many times ngl
>
> the best thing u can do for ur business is to keep ur mouth (especially if new)
>
> share only what brings u more business
>
> or else it will attract copy cats, people who wanna learn from you, people who dgaf
>
> even if u doing build in public share only:
>
> > what is gonna get u mega viral
> > ur workflows that will get u customers
> > hit your goal first while documenting from day 1 then share the parts that make sense
>
> it's worse if u are a saas founder
>
> building a business in public is super risky (speaking from personal experiences)"
>
> - Suprava

## Share only these three things

1. **What can go mega-viral**: reach plays. Top-of-funnel attention that
   actually pulls people in.
2. **The workflows that win you customers**: the how-to that makes someone
   buy, not the generic advice that makes someone copy you.
3. **The parts that make sense**: hit your goal first while documenting from
   day 1, then publish only the slice worth publishing.

## Keep private

- The full playbook, mechanics, and moat of the product
- Numbers and details that only invite copycats
- Anything that teaches a competitor more than it wins you a customer
- Daily "we shipped X" noise that neither converts nor travels

## Pick your path first

Post ideas always come from a changelog, but *where* that changelog comes from
depends on how far along the product is. Check this before you do anything
else.

**Path A: the product is already built and a changelog already exists.**
The user has shipped, meaning the product is already built or launched, and
already keeps a `changelog.md` or already generates a changelog report. Do NOT
rebuild it. Analyse the changelog you're given:

1. Read every entry in it.
2. Classify each entry and run the share test (Step 2 below).
3. Turn the survivors into posts (Step 3 below).

Because the back-catalogue is already complete, you can mine the whole thing in
one pass and hand back a batch of ready-to-post ideas, instead of a single
update. Skip Step 1 entirely, the changelog already exists.

**Path B: the product is still being built (no changelog yet).**
Use the normal workflow below: build the changelog as you ship, then mine it
for ideas.

**Path C: no changelog, and no repo to pull one from.**
The user has logged nothing and there's no codebase to mine, a solo founder, a
no-code product, an idea that hasn't shipped. Don't stall. Ask for the raw
material directly, in one short batch:

- What did you build or change recently?
- What did a customer ask for, or what did you fix for them?
- Any result worth showing, a number, a before/after, a launch?

Build the changelog from those answers (Step 1), then continue as normal.

Either way you finish at Step 3, the paths differ only in where the entries
come from.

## Changelog-driven post ideas (the workflow)

The strongest post ideas are mined from what you actually shipped, not
invented from a blank page. So every time you're asked for post ideas, work
from a changelog.

**Step 1: Build the changelog from what you actually shipped.**
Know your four inputs first: the **repos** (GitHub org + the repos holding the
product's work), the **product scope** (if a repo is shared across products, the
keywords or file paths that mark a change as relevant, and those that mean
skip), the **timezone** (how "today" and "yesterday" resolve; GitHub timestamps
are UTC, so convert them for display), and the **product name** (shown in the
summary line).

Entries come from **merged PRs in the date window**. Pull them across the
tracked repos, filter to your product's scope, and write each change as a
user-facing entry. Don't write it as a marketing doc. "When in doubt, skip", a
shorter accurate changelog beats a padded one. Each entry has three parts:

- **Title**: one line from the user's job-to-be-done: what problem did this
  solve, or what can someone now do? Plain English, not technical.
- **Contributors**: who shipped it, plus the PR link.
- **Details**: 2-3 sentences on what changed and why it matters. No jargon,
  no class names, no file paths.

Record the *why* next to the *what*, that's where the post angle lives. Keep
it factual and internal; the changelog is your idea bank, not the post itself.
(If you already generate a changelog report from GitHub activity, that report
*is* the changelog, mine it directly.)

**Step 2: Classify each entry, then run the share test.**
Tag each entry by its changelog section, then decide whether it's postable:

| Changelog section | What it is | Post it? | Angle |
|---|---|---|---|
| New | a new capability | usually yes | launch / reach post |
| Improved | a better workflow | yes, if it wins customers | "here's how we did X" |
| Fixed | a bug fix | rarely | only if the story travels |
| Under the hood | internal plumbing | no | keep private |

Anything that only teaches a copycat, or leaks the moat, stays private, no
matter how good it looks.

**Step 3: Turn survivors into posts.**
For each keeper, draft one post in four parts:

1. **Hook**: the change, framed to travel. Choose the hook type that fits the
   entry (see below).
2. **Body**: the business-relevant lesson: what changed, and why it matters to
   the reader.
3. **Visual**: what to show: a screenshot, a before/after, a short clip. Name
   the asset and say why that image earns the scroll. Where the post carries a
   text card or caption image, give it one bold accent colour so it stands out
   in the feed instead of blending in.
4. **CTA**: one explicit next step, matched to the post's goal: reach →
   follow; a customer-winning workflow → try it, book a demo, or grab the
   template.

Do not pad the list, a few strong posts beat thirty daily updates.

**Hook types: pick one that fits the entry**

| Hook | Best for | Shape |
|---|---|---|
| **Controversial** | a change that pushes against how the market works | "Everyone does X. We killed it." |
| **Bold** | New entries, big swings | a flat, confident claim, no hedging, no "we think" |
| **Relatable** | Improved workflows, a pain you also felt | "We used to do this by hand. Never again." |
| **Viral** | reach plays, milestones, striking results | lead with a number, a before/after, or a surprise |
| **Visual** | anything with a screenshot or design payoff | the image leads; a short line sets it up, one bold accent colour per hook |

## Worked example

**Changelog entry (from Step 1):**

> **Title:** Translated replies no longer disappear from chat
> **Contributors:** by contributor · #955
> **Details:** Translated replies were silently
> disappearing from chat. The text now streams correctly on every turn and
> survives a reload, on web and mobile.

**Finished post (from Step 3):**

- **Hook (Relatable):** "Our users watched their own messages vanish. We fixed
  it, here's why it happened."
- **Body:** For weeks, replies translated into other languages were
  disappearing mid-chat. It came down to a race between the translation stream
  and the message store, the store kept winning. We reordered it so the text
  lands before the screen clears, and it now holds on every turn and survives a
  reload, on web and mobile.
- **Visual:** A before/after screen recording, the message vanishing, then
  staying. Caption card in one bold accent colour.
- **CTA:** "Building for a multilingual audience? We wrote up how we handled
  streaming translation, link in the comments."

Note: this is a **Fixed** entry, which the table marks "rarely". It clears the
share test because the story travels, a user-visible failure with a clean
cause. Most fixes still stay private; this one earns its post.

## Rules of thumb

- Prefer fewer, sharper posts over a daily drumbeat.
- Document from day 1, but publish selectively and late.
- If a post wouldn't bring more business, don't publish it.
- SaaS founders: be extra conservative, the moat is easy to leak.

