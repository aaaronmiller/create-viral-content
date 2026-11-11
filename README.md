# create-viral-content

<p align="center">
  <img src="https://img.shields.io/github/stars/aaaronmiller/create-viral-content?style=for-the-badge&color=f59e0b" alt="Stars">
  <img src="https://img.shields.io/badge/Agent%20Skill-v3.0.0-8b5cf6?style=for-the-badge" alt="Agent Skill v3.0.0">
  <img src="https://img.shields.io/badge/Platforms-Reddit%20%C2%B7%20X%20%C2%B7%20LinkedIn%20%C2%B7%20YouTube%20%C2%B7%20TikTok-0ea5e9?style=for-the-badge" alt="Platforms">
</p>

An Agent Skill that turns a draft or a brief into social content that spreads
and reads as written by a person with a point of view. It covers hooks,
platform rules, titles and thumbnails, AI-tell removal, adversarial
refinement and AI-disclosure rules, updated for the platform changes of
June to November 2026.

## Install

The skill is a folder named `create-viral-content` containing `SKILL.md` and
`references/`. Every platform below needs the folder name to stay exactly
`create-viral-content`.

**claude.ai (web and desktop).** Download `create-viral-content.zip` from the
[latest release](https://github.com/aaaronmiller/create-viral-content/releases/latest)
and upload it under Settings, Capabilities, Skills. To build the zip
yourself instead, its single top-level folder must be `create-viral-content`:
```bash
git clone https://github.com/aaaronmiller/create-viral-content
cd create-viral-content && git archive --prefix=create-viral-content/ -o ../create-viral-content.zip HEAD
```
Do not upload GitHub's "Download ZIP" archive: it wraps the files in
`create-viral-content-main/`, and the folder name must match the skill name.

**Claude Code.**
```bash
git clone https://github.com/aaaronmiller/create-viral-content ~/.claude/skills/create-viral-content
```

**Codex, Gemini CLI, opencode, Qwen Code, Cursor, Kilo** (shared user-level
skills folder):
```bash
git clone https://github.com/aaaronmiller/create-viral-content ~/.agents/skills/create-viral-content
```

**Antigravity:** clone into `~/.gemini/config/skills/create-viral-content`.

**Claude API and OpenAI API:** upload the same zip as a skill bundle.

## Use

```
Write a LinkedIn post about [topic]. I ran [experiment] for [time] and
[result]. Audience: [who].
```

```
Give me 10 YouTube title and thumbnail-text variants for a video about
[topic]. The video shows [what it delivers].
```

The skill runs an eight-step workflow: pin the brief and the author's own
stake, check platform rules, draft hooks, draft the body, remove AI tells,
run five refinement passes, package variants, and check disclosure.

## Files

| File | Purpose |
|---|---|
| `SKILL.md` | Workflow, platform rules, hooks, titles, top AI tells, ethics and disclosure |
| `references/platform-updates-2026.md` | Dated 2026 ranking, anti-AI and disclosure changes with sources |
| `references/ai-tells.md` | 100+ AI tells, including current-model tells (2026) |
| `references/platform-templates.md` | Templates for Reddit, X, LinkedIn, YouTube, TikTok, Instagram, email |
| `references/refinement-protocol.md` | Adversarial passes for text and thumbnails |
| `references/viral-titles.md`, `references/title-formulas.md` | Title psychology and 50+ formulas |
| `references/viral-thumbnails.md`, `references/thumbnail-checklist.md` | Thumbnail design and checklist |
| `references/research-statistics.md` | Research data, with 2026 studies that supersede older rules |
| `references/humanize-integration.md` | Hand-off to the humanize-writing skill |
| `references/cross-platform-adaptation.md` | One piece across several platforms |
| `references/trend-intelligence.md` | Finding a topic when you have none |
| `references/feedback-loop.md` | Tracking results over time |
| `CHANGELOG.md` | Version history |
| `marketplace.json` | Marketplace manifest |

## Optional companion

[humanize-writing](https://github.com/aaaronmiller/custom-skills/tree/main/humanize-writing)
adds a voice-polish pass. Without it, the skill uses its built-in checklist.

## Ethics

Use it to sharpen your own ideas. It refuses astroturfing, misinformation,
impersonation, fake reviews and invented personal experiences, and it tells
you which AI-disclosure rule applies (including EU AI Act Article 50 for
public-interest content from 2026-08-02).

## Version

| Field | Value |
|---|---|
| Version | 3.0.0 |
| Updated | 2026-11-10 |
| Author | ice-ninja |
| License | MIT |
| Format | Agent Skills (SKILL.md with name, description, license, metadata) |

Issues and suggestions: open an issue on this repository.
