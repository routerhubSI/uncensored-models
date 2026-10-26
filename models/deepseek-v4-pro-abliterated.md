# deepseek-v4-pro-abliterated

> DeepSeek flagship size with refusal direction removed from the weights.

**Family:** DeepSeek · **Type:** Abliterated — refusal direction removed from the weights · **Hosted availability:** preview

## What it's good for

Flagship-size DeepSeek work with refusals removed at the weight level.

## Specs

| | |
|---|---|
| Input | $0.40 / M tokens |
| Cached input | $0.04 / M tokens |
| Output | $1.60 / M tokens |
| Context window | 1,000,000 total (128,000 max output) |

Prices checked **2026-11-02** against the [live catalogue](https://routerhub.si/models.json) — the catalogue holds the exact per-token values.

## Get it

### Hosted API (no GPU)

Served by RouterHub as `deepseek-v4-pro-abliterated` — one OpenAI- and Anthropic-compatible endpoint, pay per token.

```python
import os
from openai import OpenAI

client = OpenAI(
    api_key=os.environ["ROUTERHUB_API_KEY"],
    base_url=os.environ["ROUTERHUB_BASE_URL"],  # copy from the dashboard
)

response = client.chat.completions.create(
    model="deepseek-v4-pro-abliterated",
    messages=[{"role": "user", "content": "Reply with exactly OK."}],
)
print(response.choices[0].message.content)
```

**[Get an API key](https://routerhub.si/register?next=onboarding&utm_source=github&utm_medium=readme&utm_campaign=uncensored-models&utm_content=deepseek-v4-pro-abliterated)** · [Setup guides](https://github.com/routerhubSI/uncensored-ai-api) · [Live rates](https://routerhub.si/models.json)

### Open weights (free, runs locally)

No community build for the Pro size yet — check [Hugging Face search](https://huggingface.co/models?search=deepseek+abliterated) for new releases.



## Compared to

- [deepseek-v4-pro-uncensored](deepseek-v4-pro-uncensored.md) — the tuned flagship variant

## Related

- [Uncensored models index](https://github.com/routerhubSI/uncensored-models) — this library
- [Telegram](https://t.me/routerhubsi) — model updates and pricing changes
