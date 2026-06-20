# Cross-Platform Adaptation Framework

> **Progressive Disclosure:** Use this module when the user wants ONE piece of content adapted to multiple platforms. If they only need one platform, skip this entirely.

## The Topology Question: Star vs Mesh

### Star Topology (Recommended for Most Cases)

One piece of content → adapted to each platform independently.

```
                    ┌─────────────┐
                    │  Original   │
                    │  Content    │
                    └──────┬──────┘
                           │
           ┌───────────────┼───────────────┐
           │               │               │
           ▼               ▼               ▼
      ┌─────────┐    ┌─────────┐    ┌─────────┐
      │ Reddit  │    │ Twitter │    │ LinkedIn│
      │ (long)  │    │(thread) │    │ (post)  │
      └─────────┘    └─────────┘    └─────────┘
           │               │               │
           ▼               ▼               ▼
      ┌─────────┐    ┌─────────┐    ┌─────────┐
      │ YouTube │    │ TikTok  │    │Newsletter│
      │(comment)│    │ (hook)  │    │(subject)│
      └─────────┘    └─────────┘    └─────────┘
```

**When to use:** You have one strong take and want maximum reach.
**Each platform gets its own version.** No cross-linking needed.
**Why:** Each platform's algorithm rewards native content. A Reddit post that says "also on Twitter" feels like spam.

### Mesh Topology (Recommended for Ecosystem Play)

Platforms reference each other to create a discovery loop.

```
      ┌─────────┐ ←────────→ ┌─────────┐
      │ Reddit  │   "see my  │ Twitter │
      │ (full)  │    thread" │(thread) │
      └────┬────┘            └────┬────┘
           │                      │
           │    ┌─────────┐       │
           └──→ │ GitHub  │ ←─────┘
                │ (code)  │
                └────┬────┘
                     │
                ┌────▼────┐
                │ YouTube │
                │ (demo)  │
                └─────────┘
```

**When to use:** You have a project/product and want to drive traffic between platforms.
**Each platform teases the others.** "Full code on GitHub" → "Discussion on Reddit" → "Demo on YouTube."
**Why:** Creates a discovery loop. Reddit readers find your GitHub, GitHub stars see your YouTube, YouTube viewers join your Twitter.

### Decision Matrix

| Situation | Topology | Cross-Link? |
|-----------|----------|-------------|
| One strong opinion/take | Star | No |
| Project launch | Mesh | Yes |
| Trend commentary | Star | No |
| Tutorial/educational | Mesh | Yes |
| Personal story | Star | Maybe (link to one other) |
| Product update | Mesh | Yes |
| Meme/hot take | Star | No |
| Community building | Mesh | Yes |

## Cross-Linking Rules (Mesh Topology)

### What to Link

| From | To | Natural Link Phrase |
|------|-----|-------------------|
| Reddit | GitHub | "Full code and data at [github]" |
| Twitter | Reddit | "Discussion thread on r/[sub]" |
| YouTube | GitHub | "Source in comments" |
| GitHub | YouTube | "Demo video in README" |
| LinkedIn | Twitter | "Follow for more @[handle]" |
| TikTok | Instagram | "Full version on IG" |
| Newsletter | Reddit | "Community discussion at [link]" |

### What NOT to Link

| From | To | Why |
|------|-----|-----|
| Reddit | Twitter | Different audiences, feels like farming |
| Twitter | LinkedIn | Tone mismatch (casual vs professional) |
| TikTok | GitHub | Zero audience overlap |
| LinkedIn | TikTok | Professional credibility risk |
| Newsletter | TikTok | Different consumption patterns |

### The "One Link Rule"

Each piece of content should have **at most one outbound link**. More than one feels like spam. Pick the platform where your target audience lives.

## Platform Adaptation Patterns

### Original → Reddit

- Title: Use curiosity-gap or contrarian formula
- Body: 200-400 words, conversational, bold headers
- Ending: TL;DR that's quotable, invite specific discussion
- Tone: Casual expert

### Original → Twitter/X Thread

- Tweet 1: Hook (standalone viral potential)
- Tweets 2-5: One insight per tweet, no numbering
- Final tweet: Payoff or quotable closer
- Tone: Punchy, fragmentary OK

### Original → LinkedIn

- Opening: Personal story or contrarian statement
- Body: Professional lesson with specific example
- Ending: Invite specific perspectives (not "what do you think?")
- Tone: Professional but warm

### Original → YouTube Comment

- First line: Bold claim (stop the scroll)
- Middle: 2-3 sentences of mechanic
- End: Quotable closer or question
- Length: Under 500 chars

### Original → TikTok Script

- Hook: First 1-3 seconds (curiosity, problem, or result)
- Body: 15-30 seconds of value
- CTA: Follow for part 2, or quotable last line
- Caption: 5-10 words + hashtags at end

### Original → Instagram Reels

- First frame: Visual hook (text overlay)
- Pattern interrupt: Unexpected visual in first 2 seconds
- Carousel: Hook → Value → Quotable last slide
- Caption: Keywords in first 3 words

### Original → Email Subject Line

- Length: 30-50 characters
- Pattern: Curiosity, personal, or value
- Preview text: Complement, don't repeat

## The Content Waterfall (Star Topology)

For maximum reach from one piece of content:

```
Day 0:  Write original (blog post or long-form)
Day 1:  Reddit post (summary + discussion prompt)
Day 1:  Twitter thread (key insights, link to Reddit for discussion)
Day 2:  LinkedIn post (personal angle on the topic)
Day 3:  YouTube comment (on related video, 500 chars)
Day 4:  TikTok (60-second version of the core insight)
Day 5:  Newsletter (round-up including this topic)
```

**Key rule:** Each platform gets a NATIVE version. Never copy-paste.

## Cross-Platform Voice Calibration

| Platform | Formality | Sentence Length | Emoji | Links |
|----------|-----------|-----------------|-------|-------|
| Reddit | Casual expert | 10-20 words | Rarely | 1 max |
| Twitter | Punchy | 5-15 words | Sometimes | 0-1 |
| LinkedIn | Professional | 15-25 words | Never | 0-1 |
| YouTube | Conversational | 10-20 words | Sometimes | 0 |
| TikTok | Casual | 5-10 words | Often | 0 |
| Instagram | Casual-polished | 10-15 words | Often | 0 (bio only) |
| Email | Personal | 15-25 words | Never | 1-2 |
| Hacker News | Technical | 15-30 words | Never | 1 max |
