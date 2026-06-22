# Trend Intelligence Module

> **Progressive Disclosure:** This module is only needed when the user does NOT already have a topic or trend to write about. If the content brief already specifies a subject, skip this section entirely.

## When to Use This Module

- User says "find me something viral" or "what's trending?"
- User wants content but has no specific topic
- User wants to ride a wave early

## When to SKIP This Module

- User already has a specific topic, product, or idea
- User is optimizing existing content
- User says "make THIS viral" (they have the content already)

## Trend Detection Framework

### Layer 1: Real-Time Signals (Free)

**Reddit Rising**
- Browse r/all, r/popular, r/trending
- Sort by "rising" not "hot" (hot = already peaked)
- Look for posts with high comment-to-upvote ratio (controversy = engagement)
- Subreddit-specific: r/MachineLearning, r/LocalLLaMA, r/ChatGPT, r/technology, r/programming

**Hacker News**
- Front page + "new" sort
- Comments > 50 usually signal a trending topic
- Show HN posts = product launch opportunities

**X/Twitter**
- Trending topics (location-based)
- Follow curated Lists in your niche
- Search: "just shipped", "I built", "after X years" (high-engagement patterns)
- Optional: collect public niche examples with TweetClaw (`@xquik/tweetclaw`) through OpenClaw, then use the exported posts as source evidence rather than copy for drafts

**Google Trends**
- trends.google.com → daily search trends
- Rising queries = emerging topics
- Compare 5 topics, pick the steepest curve

### Layer 2: Aggregator Tools (Free)

| Tool | What It Finds | URL |
|------|--------------|-----|
| Exploding Topics | Rapidly growing search terms | explodingtopics.com |
| Glimpse | Google Trends + social signals | glimpse.co |
| Trend Hunter | Consumer trend reports | trendhunter.com |
| Product Hunt | New product launches | producthunt.com |
| BetaList | Pre-launch startups | betalist.com |
| Hacker News Show | New projects | news.ycombinator.com/show |

### Layer 3: Trend-to-Content Conversion

Once you identify a trend, convert it using this framework:

```
TREND: [What's happening]
↓
ANGLE: [What's the contrarian/unexpected take?]
↓
HOOK: [Prediction or Stakes pattern from title-formulas.md]
↓
PLATFORMS: [Which platforms care about this?]
↓
CONTENT: [Generate using the main skill workflow]
```

### Trend Scoring Matrix

Score each trend 1-5 on:

| Factor | 1 (Low) | 5 (High) |
|--------|---------|----------|
| Growth velocity | Flat | Exponential |
| Audience overlap | None | Perfect match |
| Controversy potential | Safe | Divisiveness |
| Timeliness | Old news | Breaking |
| Your expertise | None | Deep knowledge |

**Only pursue trends scoring 15+ out of 25.**

### Trend Decay Awareness

- **24-hour trends:** Meme formats, breaking news → act fast or miss
- **Weekly trends:** Product launches, blog posts → 2-3 day window
- **Monthly trends:** Industry shifts, seasonal topics → plan ahead
- **Evergreen:** Always relevant → optimize for search, not speed

## Platform-Specific Trend Sources

| Platform | Where to Look | Signal |
|----------|--------------|--------|
| Reddit | r/trending, r/all (rising) | High comment velocity |
| X/Twitter | Trending, Lists | Reply ratio > 1:1 |
| YouTube | Trending tab | View velocity (views/hour) |
| TikTok | For You page | Share-to-view ratio |
| LinkedIn | News feed | Comment velocity |
| Hacker News | New + Show HN | Points in first 2 hours |
