<div align="center">

# Uncensored Models — every uncensored and abliterated model, with prices (2026)

**An uncensored model is a language model variant with fewer built-in refusals than the standard release — delivered either as a hosted API variant or as open weights. This index lists every hosted uncensored and abliterated variant with dated prices and context windows, plus the most-downloaded open-weight releases, in one comparable table.**

</div>

---

**Maintained by [RouterHub](https://routerhub.si/?utm_source=github&utm_medium=readme&utm_campaign=uncensored-models) — an API gateway, not the model owner. Hosted variants listed here include models RouterHub does not serve; open weights include releases by independent researchers. Prices are checked against the [public catalogue](https://routerhub.si/models.json) and dated below.**

Last updated: **November 2, 2026** · Prices: USD per million tokens · Behavior always depends on model version, prompt and provider policy — see [Honest limits](#honest-limits).

## Hosted uncensored models (API variants)

Every entry is OpenAI-compatible (Chat Completions) and currently labeled **preview** by the provider. "Cached input" is the rate for repeated prompt prefixes.

| Model ID | Family | Input | Cached input | Output | Context window |
|---|---|---:|---:|---:|---:|
| `deepseek-v4-pro-uncensored` | DeepSeek | $0.20 | $0.0016 | $0.40 | — |
| `deepseek-v4.1-flash-uncensored` | DeepSeek | $0.15 | $0.0027 | $0.60 | — |
| `deepseek-v4.1-flash-abliterated` | DeepSeek | $0.30 | $0.055 | $1.25 | 1,000,000 |
| `deepseek-v4.1-flash-1017-abliterated` | DeepSeek | $0.30 | $0.055 | $1.25 | 1,000,000 |
| `deepseek-v4-pro-abliterated` | DeepSeek | $0.40 | $0.04 | $1.60 | 1,000,000 |
| `glm-5.3` | Z.ai (GLM) | $0.20 | $0.12 | $0.63 | 1,048,576 |
| `glm-5.3-flash-uncensored` | Z.ai (GLM) | $0.15 | $0.0135 | $0.50 | — |
| `glm-5.3-abliterated` | Z.ai (GLM) | $0.40 | $0.16 | $1.33 | 1,048,576 |
| `glm-5.3-flash-abliterated` | Z.ai (GLM) | $0.30 | $0.12 | $1.00 | 1,048,576 |
| `qwen3.8-max-uncensored` | Qwen | $0.25 | $0.031 | $0.75 | 1,000,000 |

*Rates rounded from the catalogue; exact per-token values live in [`models.json`](https://routerhub.si/models.json). "—" means the catalogue does not publish that limit — check it before sizing prompts. Availability is preview and can change.*

Model-by-model notes:

- ### `deepseek-v4-pro-uncensored`
  DeepSeek's flagship-size uncensored variant. Cheapest hosted uncensored option in the index at this time.
- ### `glm-5.3-abliterated`
  Z.ai GLM 5.3 with abliteration applied — the most independently verified entry in this index: recorded comparisons with raw outputs and sandbox-scored acceptance runs are public in [model evals](https://github.com/routerhubSI/routerhub-model-evals). 917,504-token max input, 131,072 max output.
- ### `glm-5.3-flash-abliterated`
  The fast, cheap abliterated GLM. The classic "cheap uncensored chatbot" profile — recorded runs exist in [model evals](https://github.com/routerhubSI/routerhub-model-evals).

More hosted variants are added as providers release them. Standard (non-uncensored) frontier models — Claude, GPT, Gemini, Grok, DeepSeek, GLM and Qwen — are available on the same key; see the [full catalogue](https://routerhub.si/models?utm_source=github&utm_medium=readme&utm_campaign=uncensored-models).

## Open weights on Hugging Face

The abliterated ecosystem lives largely on Hugging Face. These are the most-downloaded uncensored/abliterated releases as of **November 2, 2026** (download counts via the Hugging Face API on that date). Most are community GGUF quantizations — check each repo's license and model card before use.

| Model | Downloads | Likes |
|---|---:|---:|
| [SC117/Qwen3.8-Flash-Next-GSQ-RCO-abliterated-GGUF](https://huggingface.co/SC117/Qwen3.8-Flash-Next-GSQ-RCO-abliterated-GGUF) | 3,553,530 | 609 |
| [huihui-ai/Huihui-Qwen3.8-27B-abliterated-GGUF](https://huggingface.co/huihui-ai/Huihui-Qwen3.8-27B-abliterated-GGUF) | 3,249,724 | 1,664 |
| [JonathanColetti/Qwen3.8-27B-Uncensored-GGUF](https://huggingface.co/JonathanColetti/Qwen3.8-27B-Uncensored-GGUF) | 2,619,075 | 1,858 |
| [HauhauCS/Qwen3.8-27B-Uncensored-HauhauCS-Aggressive-MTP-GGUF](https://huggingface.co/HauhauCS/Qwen3.8-27B-Uncensored-HauhauCS-Aggressive-MTP-GGUF) | 2,379,869 | 2,209 |
| [huihui-ai/Huihui-Qwen3.6-35B-A3B-abliterated-MTP-GGUF](https://huggingface.co/huihui-ai/Huihui-Qwen3.6-35B-A3B-abliterated-MTP-GGUF) | 2,297,059 | 70 |
| [DavidAU/Qwen3.5-9B-The-Defiant-Fable-Uncensored-Heretic-NEO-IMATRIX-MAX-MTP-GGUF](https://huggingface.co/DavidAU/Qwen3.5-9B-The-Defiant-Fable-Uncensored-Heretic-NEO-IMATRIX-MAX-MTP-GGUF) | 1,967,913 | 1,312 |
| [mradermacher/Ornith-1.5-9B-uncensored-GGUF](https://huggingface.co/mradermacher/Ornith-1.5-9B-uncensored-GGUF) | 1,709,749 | 265 |
| [DavidAU/Qwen3.8-27B-TURBO-Fable-Cold-Fusion-735-882-Heretic-Uncensored-NEO-CODER-MAX-MTP-GGUF](https://huggingface.co/DavidAU/Qwen3.8-27B-TURBO-Fable-Cold-Fusion-735-882-Heretic-Uncensored-NEO-CODER-MAX-MTP-GGUF) | 1,356,658 | 2,308 |
| [orcarouter/Qwen3.8-Flash-Next-Uncensored-GGUF](https://huggingface.co/orcarouter/Qwen3.8-Flash-Next-Uncensored-GGUF) | 1,149,873 | 1,246 |
| [0bserverx/Qwen3.8-27B-Heretic-Abliterated-Uncensored-GGUF](https://huggingface.co/0bserverx/Qwen3.8-27B-Heretic-Abliterated-Uncensored-GGUF) | 1,129,666 | 819 |
| [HauhauCS/Qwen3.6-35B-A3B-Uncensored-HauhauCS-Aggressive](https://huggingface.co/HauhauCS/Qwen3.6-35B-A3B-Uncensored-HauhauCS-Aggressive) | 1,111,177 | 4,075 |
| [HauhauCS/Gemma-4-E4B-Uncensored-HauhauCS-Aggressive](https://huggingface.co/HauhauCS/Gemma-4-E4B-Uncensored-HauhauCS-Aggressive) | 801,900 | 1,521 |

Want hosted access instead of running weights yourself? RouterHub serves several of the base models above as uncensored API variants — no GPU, pay per token. [Get an API key →](https://routerhub.si/register?next=onboarding&utm_source=github&utm_medium=readme&utm_campaign=uncensored-models)

## How to connect

Works with any OpenAI-compatible client — change two values: base URL and key.

```python
import os
from openai import OpenAI

client = OpenAI(
    api_key=os.environ["ROUTERHUB_API_KEY"],
    base_url=os.environ["ROUTERHUB_BASE_URL"],  # copy from the dashboard
)

response = client.chat.completions.create(
    model="MODEL_ID",  # any uncensored model ID above
    messages=[{"role": "user", "content": "Write a noir paragraph about a lighthouse."}],
)
print(response.choices[0].message.content)
```

Anthropic-compatible (Claude Code) and OpenAI-compatible clients are both supported — setup guides in [uncensored-ai-api](https://github.com/routerhubSI/uncensored-ai-api).

## Verify before you trust

Recorded comparisons for the GLM entries — standard, uncensored and abliterated — are public in **[model evals](https://github.com/routerhubSI/routerhub-model-evals)**: raw requests and responses, candidate hashes, sandbox-verified 17-test acceptance results and failed attempts included. First-party experiment maintained by RouterHub, not an independent audit.

## Uncensored vs abliterated

- **Uncensored** — a training or tuning outcome: the model was built or tuned to refuse less.
- **Abliterated** — a weight-level technique that removes refusal direction from an existing model, without retraining.

Both describe reduced refusal behavior. Neither guarantees refusal-free output. Longer comparison in [uncensored vs abliterated models](https://github.com/routerhubSI/uncensored-ai-api/blob/main/docs/02-uncensored-vs-abliterated-models.md).

## Honest limits

- **No provider guarantees a model will never refuse.** Uncensored and abliterated variants reduce refusal behavior; they do not remove the need for evaluation, guardrails or human review.
- **Behavior is version-dependent.** Upstream updates change behavior; re-evaluate after releases.
- **Prices and availability rotate.** The table above is dated — confirm current rates in the [catalogue](https://routerhub.si/models.json) before committing.
- **Open-weight download counts change** and popularity is not a quality measure.

## FAQ

**Can I run these models locally instead?**

Yes — the open-weight section links community releases you can run yourself. RouterHub exists for the case where you would rather pay per token than manage GPUs.

**Why are competitors listed here?**

Because the point of this index is to be complete and honest. If you maintain or discover an uncensored model that belongs here, open an issue.

**Does uncensored mean it will do anything I ask?**

No. Refusal behavior varies by model, version and prompt. You remain responsible for lawful, ethical use.

---

<div align="center">

**Star this repository if it helped you compare uncensored models.**

<sub>RouterHub is an independent API gateway. Model names and trademarks belong to their respective owners. Not affiliated with GitHub, OpenAI, Anthropic, Google, xAI, DeepSeek, Z.ai, Qwen, Moonshot AI or Hugging Face. Use responsibly and follow the terms that apply to you.</sub>

</div>
