# deepseek-v4.1-flash-1017-abliterated

> A pinned October 2026 abliterated build of DeepSeek 4.1 Flash — reproducible behavior across runs.

**Family:** DeepSeek · **Type:** Abliterated — refusal direction removed from the weights (pinned 2026-10-17 build) · **Hosted availability:** preview

## What it's good for

Same profile as the rolling abliterated Flash, pinned to the October 2026 build — pick it when runs must be reproducible.

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

Served by RouterHub as `deepseek-v4.1-flash-1017-abliterated` — one OpenAI- and Anthropic-compatible endpoint, pay per token.

```python
import os
from openai import OpenAI

client = OpenAI(
    api_key=os.environ["ROUTERHUB_API_KEY"],
    base_url=os.environ["ROUTERHUB_BASE_URL"],  # copy from the dashboard
)

response = client.chat.completions.create(
    model="deepseek-v4.1-flash-1017-abliterated",
    messages=[{"role": "user", "content": "Reply with exactly OK."}],
)
print(response.choices[0].message.content)
```

**[Get an API key](https://routerhub.si/register?next=onboarding&utm_source=github&utm_medium=readme&utm_campaign=uncensored-models&utm_content=deepseek-v4.1-flash-1017-abliterated)** · [Setup guides](https://github.com/routerhubSI/uncensored-ai-api) · [Live rates](https://routerhub.si/models.json)

### Open weights (free, runs locally)

Community GGUF builds — all-time download counts checked **2026-11-02** via the Hugging Face API. Check each repo's license and model card before use:

| Build | Downloads | Likes |
|---|---:|---:|
| [Abiray/DeepSeek-V4.1-Flash-1017-Uncensored-GSQ-RCO-IQ2_XXS-GGUF](https://huggingface.co/Abiray/DeepSeek-V4.1-Flash-1017-Uncensored-GSQ-RCO-IQ2_XXS-GGUF) | 366,471 | 67 |



## Compared to

- [deepseek-v4.1-flash-abliterated](deepseek-v4.1-flash-abliterated.md) — the rolling latest abliterated build

## Related

- [Uncensored models index](https://github.com/routerhubSI/uncensored-models) — this library
- [Telegram](https://t.me/routerhubsi) — model updates and pricing changes
