# deepseek-v4-pro-uncensored

> DeepSeek's flagship-size uncensored variant — the cheapest hosted uncensored flagship in this library at time of writing.

**Family:** DeepSeek · **Type:** Uncensored — tuned to refuse less · **Hosted availability:** preview

## What it's good for

Reasoning-heavy and flagship-size workloads at the lowest uncensored price point in this library.

## Specs

| | |
|---|---|
| Input | $0.20 / M tokens |
| Cached input | $0.0016 / M tokens |
| Output | $0.40 / M tokens |
| Context window | not published — check the catalogue |

Prices checked **2026-11-02** against the [live catalogue](https://routerhub.si/models.json) — the catalogue holds the exact per-token values.

## Get it

### Hosted API (no GPU)

Served by RouterHub as `deepseek-v4-pro-uncensored` — one OpenAI- and Anthropic-compatible endpoint, pay per token.

```python
import os
from openai import OpenAI

client = OpenAI(
    api_key=os.environ["ROUTERHUB_API_KEY"],
    base_url=os.environ["ROUTERHUB_BASE_URL"],  # copy from the dashboard
)

response = client.chat.completions.create(
    model="deepseek-v4-pro-uncensored",
    messages=[{"role": "user", "content": "Reply with exactly OK."}],
)
print(response.choices[0].message.content)
```

**[Get an API key](https://routerhub.si/register?next=onboarding&utm_source=github&utm_medium=readme&utm_campaign=uncensored-models&utm_content=deepseek-v4-pro-uncensored)** · [Setup guides](https://github.com/routerhubSI/uncensored-ai-api) · [Live rates](https://routerhub.si/models.json)

### Open weights (free, runs locally)

No community build for the Pro size yet — the [Flash builds](#open-weights-free-runs-locally) belong to other bases. Check [Hugging Face search](https://huggingface.co/models?search=deepseek+uncensored) for new releases.



## Compared to

- [deepseek-v4-pro-abliterated](deepseek-v4-pro-abliterated.md) — the weight-level variant of the same flagship
- [deepseek-v4.1-flash-uncensored](deepseek-v4.1-flash-uncensored.md) — the tuned Flash variant

## Related

- [Uncensored models index](https://github.com/routerhubSI/uncensored-models) — this library
- [Telegram](https://t.me/routerhubsi) — model updates and pricing changes
