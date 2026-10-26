# deepseek-v4.1-flash-uncensored

> Fast DeepSeek 4.1 Flash tuned to refuse less — a general-purpose uncensored workhorse.

**Family:** DeepSeek · **Type:** Uncensored — tuned to refuse less · **Hosted availability:** preview

## What it's good for

Everyday uncensored chat, summarization and tool loops where speed and cost matter.

## Specs

| | |
|---|---|
| Input | $0.15 / M tokens |
| Cached input | $0.0027 / M tokens |
| Output | $0.60 / M tokens |
| Context window | not published — check the catalogue |

Prices checked **2026-11-02** against the [live catalogue](https://routerhub.si/models.json) — the catalogue holds the exact per-token values.

## Get it

### Hosted API (no GPU)

Served by RouterHub as `deepseek-v4.1-flash-uncensored` — one OpenAI- and Anthropic-compatible endpoint, pay per token.

```python
import os
from openai import OpenAI

client = OpenAI(
    api_key=os.environ["ROUTERHUB_API_KEY"],
    base_url=os.environ["ROUTERHUB_BASE_URL"],  # copy from the dashboard
)

response = client.chat.completions.create(
    model="deepseek-v4.1-flash-uncensored",
    messages=[{"role": "user", "content": "Reply with exactly OK."}],
)
print(response.choices[0].message.content)
```

**[Get an API key](https://routerhub.si/register?next=onboarding&utm_source=github&utm_medium=readme&utm_campaign=uncensored-models&utm_content=deepseek-v4.1-flash-uncensored)** · [Setup guides](https://github.com/routerhubSI/uncensored-ai-api) · [Live rates](https://routerhub.si/models.json)

### Open weights (free, runs locally)

Community GGUF builds — all-time download counts checked **2026-11-02** via the Hugging Face API. Check each repo's license and model card before use:

| Build | Downloads | Likes |
|---|---:|---:|
| [pyrodog/DeepSeek-V4.1-Flash-UNCENSORED-DwarfStar-Q2](https://huggingface.co/pyrodog/DeepSeek-V4.1-Flash-UNCENSORED-DwarfStar-Q2) | 49,457 | 20 |
| [Adolphsson/DeepSeek-V4.1-Flash-UNCENSORED-GGUF](https://huggingface.co/Adolphsson/DeepSeek-V4.1-Flash-UNCENSORED-GGUF) | 37,641 | 11 |
| [dealignai/DeepSeek-V4.1-Flash-UNCENSORED-FP8](https://huggingface.co/dealignai/DeepSeek-V4.1-Flash-UNCENSORED-FP8) | 33,180 | 818 |



## Compared to

- [deepseek-v4-pro-uncensored](deepseek-v4-pro-uncensored.md) — the tuned flagship variant
- [deepseek-v4.1-flash-abliterated](deepseek-v4.1-flash-abliterated.md) — the rolling latest abliterated build

## Related

- [Uncensored models index](https://github.com/routerhubSI/uncensored-models) — this library
- [Telegram](https://t.me/routerhubsi) — model updates and pricing changes
