---
name: gold-macro
description: Run daily gold macro/price analysis via a stable wrapper script. Use when the user asks for 黄金趋势、买卖区间、关键驱动、事件风险、日更摘要，and responses should be anchored to local data builds.
---

# Gold Macro Skill

## Run

Use the wrapper instead of calling service scripts directly.

```bash
python3 /Users/skin/Projects/量化/skills/gold-macro/scripts/run.py daily
```

## Supported intents

- `brief`
- `daily`
- `full`
- `trend`
- `buy`
- `sell`
- `risk`

## Rules

- Start from trend, then drivers, then action zones.
- If refresh fails and cached data exists, explicitly state that cache is being used.
- Preserve key support/resistance levels from script output.
