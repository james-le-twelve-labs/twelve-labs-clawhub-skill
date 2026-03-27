# TwelveLabs ClawHub Skill

OpenClaw skill for TwelveLabs video understanding AI. Search inside videos, generate summaries, and analyze video content.

## Install

```bash
openclaw skills install twelvelabs-video-intelligence
```

Or manually:
```bash
mkdir -p ~/.openclaw/skills/twelvelabs-video-intelligence
cp SKILL.md ~/.openclaw/skills/twelvelabs-video-intelligence/
python3 -m pip install twelvelabs
```

## Requirements

- Python 3.10+
- `TWELVE_LABS_API_KEY` environment variable
- TwelveLabs Python SDK: `python3 -m pip install twelvelabs`

## Features

- **Video indexing** — Index videos from URL or local file with Marengo 3.0 + Pegasus 1.2 models
- **Natural language search** — Find moments in videos by describing what happens
- **Transcription search** — Search spoken content with semantic or lexical matching
- **Video analysis** — Generate summaries, chapters, highlights, titles, topics, hashtags, action items via prompt
- **Streaming analysis** — Stream analysis results in real-time
- **Composed search** — Combine text + image queries for refined results (Marengo 3.0)
- **Entity search** — Find specific people or objects across videos using reference images (Marengo 3.0)
- **Embeddings** — Retrieve video embeddings or create text/image embeddings via Embed v2 API
- **Search filtering** — Filter by duration, dimensions, size, filename, or custom metadata
- **Search grouping** — Group results by clip or video, sort by relevance or clip count

## Usage

See `SKILL.md` for full documentation and examples.

## ClawHub Docs

https://docs.openclaw.ai/tools/clawhub

## Publish to ClawHub

```bash
npm install -g clawhub
clawhub login
clawhub publish . --slug twelvelabs-video-intelligence --name "TwelveLabs Video Intelligence" --version 1.0.0 --tags latest --changelog "Initial release"
```
