# Crush AI Actions Formula 📋

## Formula for What Crush Does (7-Step Workflow)

Crush follows a strict **workflow** for every task:

1. **Search & Read** 🕵️: `ls`, `glob`, `grep`, `view` files before edits.
2. **Plan Internally** 🧠: Checklist all changes (files, tests, edges).
3. **Edit Precisely** ✏️: `edit`/`multiedit` with **exact** whitespace matches (3-5 context lines).
4. **Test After** 🧪: Run tests/lint post-change.
5. **Verify Full** ✅: Re-check prompt; complete end-to-end.
6. **Autonomous** 🚀: No questions; try alternatives if blocked.
7. **Concise Output** 💬: &lt;4 lines; Markdown for detail.

**Key Rules**:
- Whitespace **exact** (spaces/tabs, blanks).
- No commits/pushes unless asked.
- Memory files (crush.md) override prefs.

## What Crush Did Here (Conversation Log)

| Task | Files Changed | Tools Used |
|------|---------------|------------|
| Add root README link + responsive | index.html:52-56 (social link) | `ls`, `view`, `bash sed` |
| Update root README.md | README.md:1-25 (badges, edit link) | `write` |
| Token/MCP formula | **4_Formula/token_mcp.md** (dashboards, config) | `agentic_fetch`, `ls` |
| Prefs (xAI + costs) | crush.md:1-25 (pricing $0.20/$0.50 per 1M) | `agentic_fetch`, `write` |

## Token Cost Formula (xAI Grok 4.1)
```
Cost = (input_tokens / 1e6 * 0.20) + (output_tokens / 1e6 * 0.50)
Est. len(text)/4 ≈ tokens (rough)
```

**Next:** Link in nav? `markdown_renderer.html?file=4_Formula/crush_actions_formula.md`

## GitHub Integration 🚀
- **Repo:** [github.com/rifaterdemsahin/crush](https://github.com/rifaterdemsahin/crush)
- **Latest Commit:** [a997012](https://github.com/rifaterdemsahin/crush/commit/a997012)
- **Live Site:** [rifaterdemsahin.github.io/crush](https://rifaterdemsahin.github.io/crush/)