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

## Usage

See `SKILL.md` for full documentation and examples.

## Publish to ClawHub

```bash
npm install -g clawhub
clawhub login
clawhub publish . --slug twelvelabs-video-intelligence --name "TwelveLabs Video Intelligence" --version 1.0.0 --tags latest --changelog "Initial release"
```
