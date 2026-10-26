# glm-5.3-flash-uncensored

> Fast GLM 5.3 Flash tuned to refuse less — cheap, quick, fewer refusals.

**Family:** Z.ai (GLM) · **Type:** Uncensored — tuned to refuse less · **Hosted availability:** preview

## What it's good for

High-volume chat, classification and quick tasks where cost per message matters more than flagship depth.

## Specs

| | |
|---|---|
| Input | $0.15 / M tokens |
| Cached input | $0.0135 / M tokens |
| Output | $0.50 / M tokens |
| Context window | not published — check the catalogue |

Prices checked **2026-11-02** against the [live catalogue](https://routerhub.si/models.json) — the catalogue holds the exact per-token values.

## Get it

### Hosted API (no GPU)

Served by RouterHub as `glm-5.3-flash-uncensored` — one OpenAI- and Anthropic-compatible endpoint, pay per token.

```python
import os
from openai import OpenAI

client = OpenAI(
    api_key=os.environ["ROUTERHUB_API_KEY"],
    base_url=os.environ["ROUTERHUB_BASE_URL"],  # copy from the dashboard
)

response = client.chat.completions.create(
    model="glm-5.3-flash-uncensored",
    messages=[{"role": "user", "content": "Reply with exactly OK."}],
)
print(response.choices[0].message.content)
```

**[Get an API key](https://routerhub.si/register?next=onboarding&utm_source=github&utm_medium=readme&utm_campaign=uncensored-models&utm_content=glm-5.3-flash-uncensored)** · [Setup guides](https://github.com/routerhubSI/uncensored-ai-api) · [Live rates](https://routerhub.si/models.json)

### Open weights (free, runs locally)

Community GGUF builds — all-time download counts checked **2026-11-02** via the Hugging Face API. Check each repo's license and model card before use:

| Build | Downloads | Likes |
|---|---:|---:|
| [BoldingBuilds/orcarouter_GLM-5.3-Flash-Uncensored-GGUF](https://huggingface.co/BoldingBuilds/orcarouter_GLM-5.3-Flash-Uncensored-GGUF) | 504,769 | 37 |
| [GCSA-AiLab/GLM-5.3-Flash-Uncensored-RCO-GSQ-GGUF](https://huggingface.co/GCSA-AiLab/GLM-5.3-Flash-Uncensored-RCO-GSQ-GGUF) | 54,592 | 10 |
| [AliceThirty/GLM-5.3-Flash-UNCENSORED-GGUF](https://huggingface.co/AliceThirty/GLM-5.3-Flash-UNCENSORED-GGUF) | 29,302 | 22 |
| [orcarouter/GLM-5.3-Flash-Uncensored-FP8](https://huggingface.co/orcarouter/GLM-5.3-Flash-Uncensored-FP8) | 25,518 | 316 |



## Compared to

- [glm-5.3-uncensored](glm-5.3-uncensored.md) — the tuned variant of the same base
- [glm-5.3-flash-abliterated](glm-5.3-flash-abliterated.md) — the cheap, fast abliterated Flash

## Related

- [Uncensored models index](https://github.com/routerhubSI/uncensored-models) — this library
- [Telegram](https://t.me/routerhubsi) — model updates and pricing changes
