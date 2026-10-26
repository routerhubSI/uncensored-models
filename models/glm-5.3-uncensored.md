# glm-5.3-uncensored

> Z.ai GLM 5.3 tuned to refuse less — the full GLM capability set with relaxed refusal behavior.

**Family:** Z.ai (GLM) · **Type:** Uncensored — tuned to refuse less · **Hosted availability:** preview

## What it's good for

Long-form writing, roleplay and agentic workflows where a mid-task refusal breaks the loop. Tuned variant, so tool-use behavior matches the official GLM 5.3.

## Specs

| | |
|---|---|
| Input | $0.20 / M tokens |
| Cached input | $0.12 / M tokens |
| Output | $0.63 / M tokens |
| Context window | not published — check the catalogue |

Prices checked **2026-11-02** against the [live catalogue](https://routerhub.si/models.json) — the catalogue holds the exact per-token values.

## Get it

### Hosted API (no GPU)

Served by RouterHub as `glm-5.3-uncensored` — one OpenAI- and Anthropic-compatible endpoint, pay per token.

```python
import os
from openai import OpenAI

client = OpenAI(
    api_key=os.environ["ROUTERHUB_API_KEY"],
    base_url=os.environ["ROUTERHUB_BASE_URL"],  # copy from the dashboard
)

response = client.chat.completions.create(
    model="glm-5.3-uncensored",
    messages=[{"role": "user", "content": "Reply with exactly OK."}],
)
print(response.choices[0].message.content)
```

**[Get an API key](https://routerhub.si/register?next=onboarding&utm_source=github&utm_medium=readme&utm_campaign=uncensored-models&utm_content=glm-5.3-uncensored)** · [Setup guides](https://github.com/routerhubSI/uncensored-ai-api) · [Live rates](https://routerhub.si/models.json)

### Open weights (free, runs locally)

Community GGUF builds — all-time download counts checked **2026-11-02** via the Hugging Face API. Check each repo's license and model card before use:

| Build | Downloads | Likes |
|---|---:|---:|
| [softwareweaver/GLM-5.3-Uncensored-GGUF](https://huggingface.co/softwareweaver/GLM-5.3-Uncensored-GGUF) | 22,161 | 17 |
| [BoldingBuilds/orcarouter_GLM-5.3-Flash-Uncensored-GGUF](https://huggingface.co/BoldingBuilds/orcarouter_GLM-5.3-Flash-Uncensored-GGUF) | 504,769 | 37 |



## Compared to

- [glm-5.3-flash-uncensored](glm-5.3-flash-uncensored.md) — the faster, cheaper tuned variant
- [glm-5.3-abliterated](glm-5.3-abliterated.md) — the abliterated full-size model, with public eval runs

## Related

- [Uncensored models index](https://github.com/routerhubSI/uncensored-models) — this library
- [Telegram](https://t.me/routerhubsi) — model updates and pricing changes
