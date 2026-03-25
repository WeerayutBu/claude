# demo-claude

A minimal Python project demonstrating [Claude Code](https://claude.ai/code) agents and skills.

## Run

```bash
python main.py
```

## Structure

```
.
├── main.py                    # App entry point
└── .claude/
    ├── agents/
    │   └── demo/              # Orchestrator agent: runs /run + /time in parallel, saves summary to out.txt
    ├── skills/
    │   ├── run/               # /run  — executes main.py
    │   └── time/              # /time — returns current timestamp
    └── settings.json          # Permissions
```

## Usage

1. **Run the app directly**
   ```bash
   python main.py
   ```

2. **Use a skill** — type in Claude Code chat:
   ```
   /run
   /time
   ```

3. **Invoke the demo agent** — ask Claude Code in chat:
   ```
   run the demo agent
   ```
   It runs `/run` and `/time` in parallel and saves the results to `out.txt`.

## Skills

| Command | What it does |
|---------|-------------|
| `/run`  | Runs `main.py` and shows output |
| `/time` | Returns the current date and time |

## Agent

The `demo` agent invokes `/run` and `/time` in parallel, then saves a summary table to `out.txt`.
