# Token & MCP Usage Formula 🧮

## View Token Usage
**No Crush CLI command; use provider consoles:**

| Provider | Dashboard Link | Env Var |
|----------|----------------|---------|
| OpenAI | [Usage](https://platform.openai.com/usage) | `OPENAI_API_KEY` |
| Anthropic | [Keys](https://console.anthropic.com/settings/keys) | `ANTHROPIC_API_KEY` |
| xAI Grok | xAI Console | `XAI_API_KEY` |
| Vercel | Vercel Dashboard | `VERCEL_API_KEY` |

## MCP Config (Reduces Tokens 70-98%)
`cat crush.json` → &quot;mcp&quot; section:

```json
{
  &quot;mcp&quot;: {
    &quot;filesystem&quot;: {
      &quot;type&quot;: &quot;stdio&quot;,
      &quot;command&quot;: &quot;node&quot;,
      &quot;args&quot;: [&quot;/path/mcp-server.js&quot;]
    }
  }
}
```

## Formulas
- **Tokens Est.:** `prompt_chars / 4 + completion_chars / 4`
- **Cost (xAI):** `(input/1M * $0.20) + (output/1M * $0.50)`

**Est. this doc:** ~800 tokens / $0.0003