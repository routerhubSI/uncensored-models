# glm-5.3-flash-abliterated

> Fast, cheap abliterated GLM — the classic cheap-uncensored-chatbot profile.

| | |
|---|---|
| Provider | Z.ai (GLM) |
| Protocol | Chat Completions (OpenAI-compatible) |
| Input | $0.30 / M tokens |
| Cached input | $0.12 / M tokens |
| Output | $1.00 / M tokens |
| Context window | 1,048,576 total (917,504 max input, 131,072 max output) |
| Availability | preview |

Prices checked **2026-11-02** against the [live catalogue](https://routerhub.si/models.json). Cached-input rates vary in precision; the catalogue holds the exact values.

**Verified runs exist** for this variant in [model evals](https://github.com/routerhubSI/routerhub-model-evals), including its classic cheap-uncensored-chatbot profile.

## How to call

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

Anthropic-compatible and coding-agent setup guides: [uncensored-ai-api](https://github.com/routerhubSI/uncensored-ai-api).

## Related

- [Uncensored models index](https://github.com/routerhubSI/uncensored-models) — this repository's comparison table
- [RouterHub](https://routerhub.si/?utm_source=github&utm_medium=readme&utm_campaign=uncensored-models&utm_content=glm-5.3-flash-abliterated)
- [Telegram](https://t.me/routerhubsi)
