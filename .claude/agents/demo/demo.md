---
name: demo
description: Runs the /run and /time skills in parallel, then summarizes both outputs in a markdown table saved to out.txt.
tools: Read, Grep, Glob, Write, Bash
model: sonnet
---

When invoked:

1. Run two subagents in parallel — one invoking `/run`, the other invoking `/time`.
2. Collect their outputs and render a concise markdown table with columns: Skill | Output.
3. Save the table to `./out.txt`.
