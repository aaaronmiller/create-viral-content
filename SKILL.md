---
name: create-viral-content
description: "Create and refine viral social content: Reddit posts, X threads, LinkedIn posts, YouTube titles and thumbnails, TikTok and Reels scripts, Instagram carousels, Threads and Bluesky posts, email subject lines and blog headlines. Use when the user wants content to spread, earn engagement, or read as human to a skeptical audience, and whenever drafting any public-facing post, hook, title or caption even if the word viral never appears. Triggers: 'make this viral', 'social media post', 'catchy headline', 'hook', 'title ideas', 'thumbnail', 'engagement', 'shareable', 'go viral', 'attention-grabbing', 'scroll-stopping', 'hot take', 'more engaging', 'subreddit', 'thread', 'sounds like AI', 'AI slop'. Covers 2026 platform ranking changes, current AI-tell removal and AI-disclosure rules."
license: MIT
metadata:
  author: ice-ninja
  version: "3.0.0"
  updated: "2026-11-10"
  tags: "social, writing, marketing, ai-tells"
---

# Create Viral Content

Turn a draft or a brief into a post that earns shares, comments and action,
and that reads as written by a person with a point of view.

## Contents

- [Workflow](#workflow)
- [What platforms reward in 2026](#what-platforms-reward-in-2026)
- [Hooks, body and closer](#hooks-body-and-closer)
- [Platform rules](#platform-rules)
- [Titles and thumbnails](#titles-and-thumbnails)
- [AI tells: the top five](#ai-tells-the-top-five)
- [Refinement passes](#refinement-passes)
- [Ethics and disclosure](#ethics-and-disclosure)
- [Example](#example)
- [Reference files](#reference-files)

## Workflow

Run these steps in order for every request. Skip a step only when the
request makes it irrelevant (for example, no thumbnail for a Reddit post).

1. **Pin the brief.** Identify platform, audience, goal and the author's own
   stake: a claim, a number, an event or an experience only they have. If
   none is given, ask for one; without it, platforms now classify the post
   as slop.
2. **Check platform rules.** Read the platform section below and, for
   LinkedIn, X, YouTube, Instagram, Threads, Reddit or email, the matching
   section of `references/platform-updates-2026.md`. For Reddit, check the
   target subreddit's AI rule first.
3. **Draft the hook.** Generate at least five hooks from the patterns below
   and pick the strongest by the title score.
4. **Draft the body and closer** using the structure below and the matching
   template in `references/platform-templates.md`.
5. **Remove AI tells.** Apply the top five below, then scan against the
   "Current-Model Tells (2026)" table in `references/ai-tells.md`.
6. **Run the refinement passes.** Attack the draft from five perspectives
   and revise after each.
7. **Package.** For video, write two or three title and thumbnail variants
   that make different promises (YouTube tests pick by watch time).
8. **Check disclosure.** Apply the disclosure rules below before handing
   the draft back, and say which one applies.

Deliver the final draft, the alternates considered, and one line on why the
chosen hook wins.

## What platforms reward in 2026

These changes override older advice. Details and sources:
`references/platform-updates-2026.md`.

- **Perspective beats polish.** LinkedIn's slop classifiers (from
  2026-07-30) cut out-of-network reach for fluent posts with no identifiable
  stance; classified slop gets about 40% fewer views.
- **Keyword-comment bait is dead.** "Comment GUIDE and I'll DM you" lost
  about half its LinkedIn reach from 2026-07-27. A plain question is fine.
- **Links cost reach.** About 16-21% on LinkedIn, including "link in the
  comments"; near-zero median engagement for non-Premium link posts on X.
  Put substance first and the link last, or in a reply.
- **Originality is enforced on video.** YouTube demonetizes templated AI
  content and AI personas on health or finance; Shorts cuts reach for
  re-uploads, and narrating someone else's footage does not count.
- **Mutuals and communities win replies.** X boosts mutual-follow replies;
  Bluesky ranks replies by social proximity; Threads reports which
  community drove each post.
- **Posting time barely matters on LinkedIn** (±2% of final reach). Do not
  spend effort on it.

## Hooks, body and closer

### Hook (first line, first two seconds)

Pick one pattern and fill it with the author's real material.

- **Prediction + stakes:** "I think [concept] is the [year] [category] that
  [outcome]." A personal conviction, a timeframe and a consequence.
- **Tribal split:** "[Technique] separates [group] from [everyone else]."
  The reader picks a side.
- **Before/after compression:** "What used to take [old cost] now takes
  [new cost]." A concrete, shareable gain.
- **Specific result:** "I tried [thing] for [time]. [Number] changed." The
  number must be real.

### Body

Order: **what** it is (one or two sentences), **how** it works with a
concrete example, **why now**, then the **payoff** the reader can use.
Explain the thing before arguing why it matters. Give at least one concrete
example per abstract claim.

### Closer (last 10%)

End on a statement, not a request:

```
BAD:  "Try it. Change my mind."  /  "Comment GUIDE and I'll send it."
GOOD: "Your next [action] shouldn't [old way]. It should [new way]."
```

A specific question that invites a real answer is acceptable; generic
"what do you think?" is not.

## Platform rules

| Platform | Length | Do | Avoid |
|---|---|---|---|
| Reddit | 200-400 words | Casual-expert voice, quotable TL;DR, match the subreddit (r/MachineLearning: conservative claims; r/LocalLLaMA: self-hosting angle) | AI-sounding replies (98% of replies are human-written, so tells stand out), posting before reading the subreddit's AI rule |
| Hacker News | Short | "Show HN:" format, understate | Hype words |
| X | under 280 chars per post | Standalone hook post, substance before link, replies inside the author's niche | "1/" numbering, bare link posts |
| LinkedIn | 150-300 words | First-person claim or lived detail, plain-question or statement closer | Keyword-comment CTAs, link in post or comments when reach matters, hashtag stuffing |
| YouTube comment | about 500 chars | Bold claim first, mechanic in two sentences, quotable closer | Formatting |
| TikTok | Caption 5-10 words | Keyword in the first three words, hook in 1-3 seconds, sound-off friendly text | Unlabeled realistic AI visuals |
| Instagram Reels | Text overlay in 2 s | First-frame hook, optimize for sends to a friend; Reels may trail a long video | Watermarked reposts, minor-crop reposts |
| Carousel | 5-10 slides | Slide 1 curiosity gap, middle slides deliver, last slide quotable | Assuming carousels still beat photos (the lead shrank to about 9%) |
| Threads | Short | First line written as a headline (posts appear in Google Discover), UTM links | Relying on native link stats (removed) |
| Email subject | 30-50 chars | Personalized curiosity; pitch in preheader and first sentence because AI inbox summaries read them | ALL CAPS urgency, fake "quick question", emoji overload |

Full templates: `references/platform-templates.md`. Adapting one piece to
several platforms: `references/cross-platform-adaptation.md`.

## Titles and thumbnails

Titles decide most of a video's or article's performance. Generate 25 or
more, then score each 0-3 on curiosity, specificity and emotion; ship only
7 or above.

- **Length:** for text headlines, about 11 words or 65 characters still
  works. For YouTube, 2026 data (507k videos) shows longer, specific titles
  break out more (over 75 characters: 35.9% vs under 30: 26.1%).
- **Numbers:** specific beats round ($1,247 over $1,000); odd beats even.
- **Negative superlatives** outperform positive ones on clicks; use them
  only when true.
- **Thumbnail:** a face with a calm or neutral expression (shocked faces are
  only 5-11% of 2026 breakouts), 4-6 words that add to the title rather than
  repeat it, at most three elements, legible at 120 px wide.
- **Variants:** make each variant a different promise the video keeps.

Formulas and scoring: `references/viral-titles.md`,
`references/title-formulas.md`. Thumbnail design:
`references/viral-thumbnails.md`, `references/thumbnail-checklist.md`.

## AI tells: the top five

Current models dropped the famous tells (em dashes fell 99% in Opus 5.5), so
check for these first. Score clusters, not single hits.

1. **Importance flagging:** "this matters", "why X matters", "matters most".
2. **"More than" contrast:** "is more than a X, it...", "rather than
   simply", "not only... but also".
3. **Forward-looking transitions:** "looking ahead", "adds another layer",
   "in practice", "here's the thing".
4. **Enthusiasm and helpfulness:** "excited to share", "game-changer",
   "can help you", "makes it easier", "genuinely".
5. **Perspective-free polish:** fluent sentences of uniform length with no
   stance, number or lived detail. Fix it by adding the author's own claim
   and varying sentence length.

Complete catalog with older tells, platform-specific tells and video and
thumbnail tells: `references/ai-tells.md`. For a voice polish pass, use the
humanize-writing skill if installed (`references/humanize-integration.md`).

Never promise that a rewrite evades AI detectors; detector vendors now
target "humanized" text. Substance and the author's real voice are what
both readers and platform classifiers reward.

## Refinement passes

Attack the draft once per pass and revise before the next. Details and
thumbnail-specific passes: `references/refinement-protocol.md`.

1. **Skeptic:** Why should I care? What is actually new?
2. **Expert:** Is every claim accurate? What would an expert nitpick?
3. **Scroller:** Would I stop for this first line?
4. **Competitor:** How is this different from the last ten similar posts?
5. **Editor:** What can go without losing meaning? Cut about 20%.

Stop when a full pass produces no change.

## Ethics and disclosure

Use this skill to sharpen the author's own ideas. Refuse astroturfing,
coordinated inauthentic behavior, misinformation, impersonation, fake
reviews or testimonials, and invented personal experiences.

Disclosure, as of November 2026:

- **Paid or sponsored content:** always disclose.
- **EU audiences, public-interest topics** (politics, health, economics):
  EU AI Act Article 50 applies from 2026-08-02. Either a named person edits
  substantively and takes editorial responsibility, or the post carries an
  AI label.
- **Realistic AI images, audio or video:** label them (YouTube, TikTok,
  India, South Korea; New York for ads with synthetic performers).
- **LinkedIn:** disclose substantial AI involvement when it is not apparent.
- **Reddit:** follow the subreddit's rule.

State in the hand-back which rule applies. Full table:
`references/platform-updates-2026.md`.

## Example

**Before (reads as AI):**

```
I'm excited to share a revolutionary productivity hack that will change
your workflow forever. Here's the thing: most people waste hours on email.
Let's dive into how inbox zero can transform your day. First, batch
process. Second, use templates. Finally, schedule check-ins. What do you
think?
```

**After (human, specific):**

```
Email before noon is self-sabotage. I tested it for 3 weeks: no inbox
until 2pm. My deep-work hours went from 2 to 4+. That 7:47am Slack ping?
Not your fire. Morning brain builds. Afternoon brain reacts. Flip the
order and you stop playing defense. Two inbox windows, 2pm and 5pm,
handle everything that matters.
```

What changed: enthusiasm, transition and list-scaffold tells removed;
engagement bait replaced by a statement; real numbers added (3 weeks, 2 to
4+ hours, 7:47am); sentence length varied from 3 to 12 words; conviction
opener instead of an announcement.

## Reference files

Load only what the current step needs.

| File | Contents | Load when |
|---|---|---|
| `references/platform-updates-2026.md` | Dated 2026 ranking, anti-AI and disclosure changes with sources | Steps 2 and 8, always for public posts |
| `references/ai-tells.md` | 100+ tells: current-model table, classic tells, platform, video and thumbnail tells | Step 5 |
| `references/platform-templates.md` | Templates and examples for 8 platforms | Step 4 |
| `references/refinement-protocol.md` | Adversarial passes for text and thumbnails | Step 6 |
| `references/viral-titles.md` | Title psychology, formulas and scoring | Titles |
| `references/title-formulas.md` | 50+ title formulas with examples | Titles |
| `references/viral-thumbnails.md` | Thumbnail psychology, design and AI prompts | Thumbnails |
| `references/thumbnail-checklist.md` | Quick thumbnail checklist | Thumbnails |
| `references/research-statistics.md` | Research data, including 2026 studies that supersede older rules | Justifying a choice |
| `references/humanize-integration.md` | Handing off to the humanize-writing skill | Step 5 voice pass |
| `references/cross-platform-adaptation.md` | One piece adapted to several platforms | Multi-platform requests |
| `references/trend-intelligence.md` | Finding a topic when the user has none | No topic given |
| `references/feedback-loop.md` | Tracking engagement over time | User wants to learn from results |
