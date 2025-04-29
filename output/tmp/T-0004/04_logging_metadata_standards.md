## 4  Logging & Metadata Standards

| File | Purpose | Format |
|------|---------|--------|
| `./output/logs/progress.log` | One-line status updates in chronological order | `ISO-8601 | TaskID | status | info` |
| `./output/logs/decisions.jsonl` | Every non-trivial decision | JSON lines: `{"timestamp": "...", "task": "T-0003", "decision": "...", "rationale": "..."}` |
| `./output/logs/errors.log` | Unhandled exceptions / fatal errors | Free-text |
| `./output/metadata.yaml` | Run-level data: goal, start/end timestamps, overall status | YAML |