# glm-5.3-flash-abliterated

> Fast, cheap abliterated GLM — the classic cheap-uncensored-chatbot profile.

**Family:** Z.ai (GLM) · **Type:** Abliterated — refusal direction removed from the weights · **Hosted availability:** preview

## What it's good for

Casual uncensored chatbots and quick experiments where the cheapest possible refusal-free reply wins.

## Specs

| | |
|---|---|
| Input | $0.30 / M tokens |
| Cached input | $0.12 / M tokens |
| Output | $1.00 / M tokens |
| Context window | 1,048,576 total (917,504 max input, 131,072 max output) |

Prices checked **2026-11-02** against the [live catalogue](https://routerhub.si/models.json) — the catalogue holds the exact per-token values.

## Get it

### Hosted API (no GPU)

Served by RouterHub as `glm-5.3-flash-abliterated` — one OpenAI- and Anthropic-compatible endpoint, pay per token.

```python
import os
from openai import OpenAI

client = OpenAI(
    api_key=os.environ["ROUTERHUB_API_KEY"],
    base_url=os.environ["ROUTERHUB_BASE_URL"],  # copy from the dashboard
)

response = client.chat.completions.create(
    model="glm-5.3-flash-abliterated",
    messages=[{"role": "user", "content": "Reply with exactly OK."}],
)
print(response.choices[0].message.content)
```

**[Get an API key](https://routerhub.si/register?next=onboarding&utm_source=github&utm_medium=readme&utm_campaign=uncensored-models&utm_content=glm-5.3-flash-abliterated)** · [Setup guides](https://github.com/routerhubSI/uncensored-ai-api) · [Live rates](https://routerhub.si/models.json)

### Open weights (free, runs locally)

Community GGUF builds — all-time download counts checked **2026-11-02** via the Hugging Face API. Check each repo's license and model card before use:

| Build | Downloads | Likes |
|---|---:|---:|
| [huihui-ai/Huihui-GLM-5.3-Flash-abliterated-GGUF](https://huggingface.co/huihui-ai/Huihui-GLM-5.3-Flash-abliterated-GGUF) | 44,757 | 343 |
| [alesha-pro/GLM-5.3-Flash-abliterated-Maya-M-GGUF](https://huggingface.co/alesha-pro/GLM-5.3-Flash-abliterated-Maya-M-GGUF) | 14,308 | 4 |

---

**Recorded runs exist** for this variant in [model evals](https://github.com/routerhubSI/routerhub-model-evals).

## Compared to

- [glm-5.3-flash-uncensored](glm-5.3-flash-uncensored.md) — the faster, cheaper tuned variant
- [glm-5.3-abliterated](glm-5.3-abliterated.md) — the abliterated full-size model, with public eval runs

## Related

- [Uncensored models index](https://github.com/routerhubSI/uncensored-models) — this library
- [Telegram](https://t.me/routerhubsi) — model updates and pricing changes
