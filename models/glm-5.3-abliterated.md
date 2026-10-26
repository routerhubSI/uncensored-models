# glm-5.3-abliterated

> Z.ai GLM 5.3 with refusal direction removed at the weight level — the most independently verified model in this library.

**Family:** Z.ai (GLM) · **Type:** Abliterated — refusal direction removed from the weights · **Hosted availability:** preview

## What it's good for

When you want the full GLM 5.3 with refusals stripped — and evidence in hand: the only model here with public recorded eval runs.

## Specs

| | |
|---|---|
| Input | $0.40 / M tokens |
| Cached input | $0.16 / M tokens |
| Output | $1.33 / M tokens |
| Context window | 1,048,576 total (917,504 max input, 131,072 max output) |

Prices checked **2026-11-02** against the [live catalogue](https://routerhub.si/models.json) — the catalogue holds the exact per-token values.

## Get it

### Hosted API (no GPU)

Served by RouterHub as `glm-5.3-abliterated` — one OpenAI- and Anthropic-compatible endpoint, pay per token.

```python
import os
from openai import OpenAI

client = OpenAI(
    api_key=os.environ["ROUTERHUB_API_KEY"],
    base_url=os.environ["ROUTERHUB_BASE_URL"],  # copy from the dashboard
)

response = client.chat.completions.create(
    model="glm-5.3-abliterated",
    messages=[{"role": "user", "content": "Reply with exactly OK."}],
)
print(response.choices[0].message.content)
```

**[Get an API key](https://routerhub.si/register?next=onboarding&utm_source=github&utm_medium=readme&utm_campaign=uncensored-models&utm_content=glm-5.3-abliterated)** · [Setup guides](https://github.com/routerhubSI/uncensored-ai-api) · [Live rates](https://routerhub.si/models.json)

### Open weights (free, runs locally)

Community GGUF builds — all-time download counts checked **2026-11-02** via the Hugging Face API. Check each repo's license and model card before use:

| Build | Downloads | Likes |
|---|---:|---:|
| [audnai/penclaw-GLM-5.3-abliterated](https://huggingface.co/audnai/penclaw-GLM-5.3-abliterated) | 2,860 | 521 |
| [huihui-ai/Huihui-GLM-5.3-Flash-abliterated-GGUF](https://huggingface.co/huihui-ai/Huihui-GLM-5.3-Flash-abliterated-GGUF) | 44,757 | 343 |

---

**Recorded runs exist** for this variant: raw requests and responses, candidate hashes and sandbox-scored 17-test acceptance results are public in [model evals](https://github.com/routerhubSI/routerhub-model-evals).

## Compared to

- [glm-5.3-uncensored](glm-5.3-uncensored.md) — the tuned variant of the same base
- [glm-5.3-flash-abliterated](glm-5.3-flash-abliterated.md) — the cheap, fast abliterated Flash

## Related

- [Uncensored models index](https://github.com/routerhubSI/uncensored-models) — this library
- [Telegram](https://t.me/routerhubsi) — model updates and pricing changes
