# deepseek-v4.1-flash-abliterated

> DeepSeek 4.1 Flash with refusal direction removed at the weight level — behavior stays close to the base model.

**Family:** DeepSeek · **Type:** Abliterated — refusal direction removed from the weights · **Hosted availability:** preview

## What it's good for

DeepSeek Flash behavior without refusals — closest to the base model's quality profile.

## Specs

| | |
|---|---|
| Input | $0.30 / M tokens |
| Cached input | $0.055 / M tokens |
| Output | $1.25 / M tokens |
| Context window | 1,000,000 total (128,000 max output) |

Prices checked **2026-11-02** against the [live catalogue](https://routerhub.si/models.json) — the catalogue holds the exact per-token values.

## Get it

### Hosted API (no GPU)

Served by RouterHub as `deepseek-v4.1-flash-abliterated` — one OpenAI- and Anthropic-compatible endpoint, pay per token.

```python
import os
from openai import OpenAI

client = OpenAI(
    api_key=os.environ["ROUTERHUB_API_KEY"],
    base_url=os.environ["ROUTERHUB_BASE_URL"],  # copy from the dashboard
)

response = client.chat.completions.create(
    model="deepseek-v4.1-flash-abliterated",
    messages=[{"role": "user", "content": "Reply with exactly OK."}],
)
print(response.choices[0].message.content)
```

**[Get an API key](https://routerhub.si/register?next=onboarding&utm_source=github&utm_medium=readme&utm_campaign=uncensored-models&utm_content=deepseek-v4.1-flash-abliterated)** · [Setup guides](https://github.com/routerhubSI/uncensored-ai-api) · [Live rates](https://routerhub.si/models.json)

### Open weights (free, runs locally)

Community GGUF builds — all-time download counts checked **2026-11-02** via the Hugging Face API. Check each repo's license and model card before use:

| Build | Downloads | Likes |
|---|---:|---:|
| [audreyt/DeepSeek-V4.1-Flash-Abliterated-GGUF](https://huggingface.co/audreyt/DeepSeek-V4.1-Flash-Abliterated-GGUF) | 80,099 | 14 |
| [huihui-ai/Huihui-DeepSeek-V4-Flash-0731-abliterated-GGUF](https://huggingface.co/huihui-ai/Huihui-DeepSeek-V4-Flash-0731-abliterated-GGUF) | 365,035 | 235 |



## Compared to

- [deepseek-v4.1-flash-uncensored](deepseek-v4.1-flash-uncensored.md) — the tuned Flash variant
- [deepseek-v4.1-flash-1017-abliterated](deepseek-v4.1-flash-1017-abliterated.md) — the pinned October build

## Related

- [Uncensored models index](https://github.com/routerhubSI/uncensored-models) — this library
- [Telegram](https://t.me/routerhubsi) — model updates and pricing changes
