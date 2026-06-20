# Engagement Feedback Loop & Self-Improvement

> **Progressive Disclosure:** This module activates AFTER content has been published. It requires a local tracking file to function. If no tracking file exists, this module can be skipped.

## Storage Convention

All engagement data lives in a single directory:

```
~/viral-content-log/
├── posts.json          # All published posts + metadata
├── scorecards/         # Per-post engagement reports
│   └── YYYY-MM-DD-{slug}.md
└── trends.json         # Observed trends from performance
```

### posts.json Schema

```json
[
  {
    "id": "2026-06-20-reddit-deliberative-refinement",
    "date": "2026-06-20T14:30:00Z",
    "platform": "reddit",
    "subreddit": "MachineLearning",
    "title": "Deliberative refinement is the 2026 prompt technique that matters most",
    "url": "https://reddit.com/r/...",
    "hook_pattern": "prediction-stakes",
    "content_snippet": "First 100 chars...",
    "engagement": {
      "upvotes": 0,
      "comments": 0,
      "awards": 0,
      "crossposts": 0
    },
    "checked": {
      "1h": null,
      "24h": null,
      "7d": null,
      "30d": null
    }
  }
]
```

## When to Run the Feedback Loop

1. **After posting** — log the post to `posts.json` immediately
2. **24 hours later** — check engagement, update the entry
3. **7 days later** — final engagement snapshot
4. **Monthly** — run self-improvement analysis (see below)

## Engagement Scoring

### Platform-Specific Metrics

| Platform | Primary Metric | Good | Great | Viral |
|----------|---------------|------|-------|-------|
| Reddit | Upvotes | 50+ | 500+ | 2000+ |
| Reddit | Comment ratio | 5% | 15% | 30%+ |
| Twitter/X | Impressions | 1K | 10K | 100K+ |
| Twitter/X | Engagement rate | 2% | 5% | 10%+ |
| LinkedIn | Reactions | 20 | 100 | 500+ |
| LinkedIn | Comments | 5 | 20 | 50+ |
| YouTube | Views (48h) | 500 | 5K | 50K+ |
| YouTube | CTR | 3% | 6% | 10%+ |
| TikTok | Views | 1K | 50K | 500K+ |
| TikTok | Share rate | 1% | 3% | 8%+ |

### Composite Viral Score

```
Viral Score = (normalized_primary_metric * 0.4) 
            + (engagement_rate * 0.3) 
            + (velocity_factor * 0.2) 
            + (longevity_factor * 0.1)
```

Score 0-10. Posts scoring 7+ are "viral" for your account size.

## Self-Improvement Analysis

> Run monthly or after every 10 posts, whichever comes first.

### Step 1: Aggregate Performance

Read all entries from `posts.json` and compute:

- **Average viral score** per platform
- **Best-performing hook pattern** (prediction-stakes vs tribal-identity vs before-after)
- **Best-performing platform** (highest average engagement)
- **Best day/time** to post
- **Topic clusters** that over/under-perform

### Step 2: Pattern Extraction

For the top 20% of posts (viral score 7+), identify:

- What hook pattern did they use?
- What platform were they on?
- What time of day were they posted?
- What was the topic category?
- What title formula was used?

For the bottom 20% (viral score < 3), identify:

- What anti-patterns appear?
- Were certain platforms consistently weaker?
- Did certain hook patterns fail?

### Step 3: Strategy Update

Generate a "Strategy Brief" with findings:

```
## Monthly Viral Content Brief — [MONTH YEAR]

### What Worked
- Hook pattern X outperformed Y by Z%
- Platform A is your strongest channel
- Topics in category B consistently go viral

### What Didn't
- Hook pattern Z underperformed across all platforms
- Platform C is not worth the effort for your niche
- Posts under N words performed better than long-form

### Next Month's Strategy
- Primary hook: [pattern]
- Primary platform: [platform]
- Content ratio: X% original takes, Y% trend-riding, Z% engagement-bait
- Posting schedule: [days/times]
```

### Step 4: Skill Update

If patterns emerge that aren't covered in the main SKILL.md:

- Add new hook patterns to `references/title-formulas.md`
- Add new AI tells to `references/ai-tells.md`
- Update platform calibration in the main body
- Add new research findings to `references/research-statistics.md`

## Quick-Start: First-Time Setup

If `~/viral-content-log/` doesn't exist:

```bash
mkdir -p ~/viral-content-log/scorecards
echo '[]' > ~/viral-content-log/posts.json
echo '{}' > ~/viral-content-log/trends.json
```

Then log your first post using the schema above.
