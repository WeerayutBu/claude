# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project

Python demo project showcasing Claude Code agents and skills.

## Commands

```bash
python main.py   # Run the app
```

## Structure

- `main.py` — Application entry point
- `.claude/agents/demo/` — Demo agent: runs `/run` and `/time` skills in parallel, summarizes results
- `.claude/skills/run/` — `/run` skill: executes `main.py`
- `.claude/skills/time/` — `/time` skill: returns current timestamp
- `.claude/settings.json` — Project permissions
