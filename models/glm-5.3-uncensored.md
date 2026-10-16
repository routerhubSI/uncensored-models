# glm-5.3-uncensored

> Z.ai GLM 5.3 tuned to refuse less. Full 1M-token context.

| | |
|---|---|
| Provider | Z.ai (GLM) |
| Protocol | Chat Completions (OpenAI-compatible) |
| Input | $0.20 / M tokens |
| Cached input | $0.12 / M tokens |
| Output | $0.63 / M tokens |
| Context window | not published — check the catalogue before sizing prompts |
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
    model="glm-5.3-uncensored",
    messages=[{"role": "user", "content": "Reply with exactly OK."}],
)
print(response.choices[0].message.content)
```

Anthropic-compatible and coding-agent setup guides: [uncensored-ai-api](https://github.com/routerhubSI/uncensored-ai-api).

## Related

- [Uncensored models index](https://github.com/routerhubSI/uncensored-models) — this repository's comparison table
- [RouterHub](https://routerhub.si/?utm_source=github&utm_medium=readme&utm_campaign=uncensored-models&utm_content=glm-5.3-uncensored)
- [Telegram](https://t.me/routerhubsi)
