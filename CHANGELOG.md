# Changelog

## [3.0.0] - 2026-11-10

### Fixed
- Malformed YAML frontmatter that made the claude.ai zip upload fail with
  "malformed YAML frontmatter in SKILL.md" (issue #2): the description was a
  closed double-quoted string followed by an indented continuation line.
- Frontmatter reduced to the portable keys (`name`, `description`,
  `license`, `metadata`); non-standard top-level keys (`inputs`, `outputs`,
  `tags`, `grade`, `source`) removed or moved under `metadata`.
- Reference list used absolute paths from the author's machine; it now uses
  relative `references/` paths.

### Changed (grading report, issue #1)
- Added a table of contents to SKILL.md and to every reference file over
  100 lines.
- Replaced the "core principle" loop with a numbered eight-step workflow.
- Imperative voice throughout.
- AI-tell section trimmed to the top five with a pointer to the full catalog.
- Explicit reference file table with contents and when to load each file.
- SKILL.md shortened from 478 to about 260 lines.

### Added (June to November 2026 changes)
- `references/platform-updates-2026.md`: dated ranking, anti-AI and
  disclosure changes for LinkedIn, X, YouTube, Instagram, Threads, Reddit,
  TikTok, Bluesky and email, with sources and confidence tags.
- `references/ai-tells.md`: "Current-Model Tells (2026)" table; em dash
  downweighted as a historical tell.
- `references/research-statistics.md`: "2026 Updates" with 2026 thumbnail
  and title studies.
- Disclosure guidance for EU AI Act Article 50 (from 2026-08-02) and other
  2026 labeling rules.

### Corrected
- "Shocked face = highest CTR" replaced: 2026 studies find neutral faces
  dominate breakout thumbnails.
- "11 words / 65 characters" limited to text headlines: 2026 YouTube data
  shows longer specific titles break out more.

## [2.1] - 2026-06-20

### Changed
- Standardized bundled documentation under `references/`.

### Fixed
- Updated marketplace and feedback-loop paths to use `references/`.
