# speech-paper-daily-skill

Daily speech paper digest skill for [Claude Code](https://claude.ai/claude-code).

## Overview

- Automatically fetches newly submitted speech/audio papers from arXiv `cs.SD` and `eess.AS` categories each day
- Deep-reads each paper in the voice of a brutally honest senior reviewer, outputting technical approach, experimental results summary, and a 10-point rating
- Covers two main tracks: **Speech Foundation Models** (TTS, ASR, codec, Speech LLM, speech generation) and **Speech Front-End** (speech enhancement, noise suppression, beamforming, source separation, dereverberation)
- Saves the digest as a local markdown report to `~/paper-digest/YYYY-MM-DD.md`

## Installation

Copy `skill.md` into your Claude Code skills directory:

```bash
# Project-level (recommended)
mkdir -p .claude/skills
cp skill.md .claude/skills/speech-paper-daily.md

# Or global
mkdir -p ~/.claude/skills
cp skill.md ~/.claude/skills/speech-paper-daily.md
```

No external MCP servers or API keys required — works out of the box with Claude Code's built-in tools (`web_fetch`, `write`, `read`, etc.).

## Usage

Say any of the following to Claude Code:

- "find the latest speech papers"
- "search speech preprints"
- "speech paper digest"
- "any new speech papers today"
- "check the latest TTS/ASR/speech enhancement papers"

## Output

Reports are saved to `~/paper-digest/YYYY-MM-DD.md` with:
- Overview table of all papers
- Papers grouped by track (Speech Foundation Models / Speech Front-End)
- Each paper includes: summary, brutal take, technical approach, experimental results, and a 10-point rating

## Files

| File | Description |
|------|-------------|
| `skill.md` | Skill definition file containing the full pipeline specification, templates, rating criteria, and output format |
