# deepseek-v4.1-flash-abliterated

> Fast DeepSeek 4.1 Flash with refusal direction removed at the weight level.

| | |
|---|---|
| Provider | DeepSeek |
| Protocol | Chat Completions (OpenAI-compatible) |
| Input | $0.30 / M tokens |
| Cached input | $0.055 / M tokens |
| Output | $1.25 / M tokens |
| Context window | 1,000,000 total (128,000 max output) |
| Availability | preview |

Prices checked **2026-11-02** against the [live catalogue](https://routerhub.si/models.json). Cached-input rates vary in precision; the catalogue holds the exact values.

No recorded runs for this variant yet — the shared task and harness are public in [model evals](https://github.com/routerhubSI/routerhub-model-evals).

## How to call

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

Anthropic-compatible and coding-agent setup guides: [uncensored-ai-api](https://github.com/routerhubSI/uncensored-ai-api).

## Related

- [Uncensored models index](https://github.com/routerhubSI/uncensored-models) — this repository's comparison table
- [RouterHub](https://routerhub.si/?utm_source=github&utm_medium=readme&utm_campaign=uncensored-models&utm_content=deepseek-v4.1-flash-abliterated)
- [Telegram](https://t.me/routerhubsi)
