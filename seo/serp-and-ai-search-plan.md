# SERP and AI Search Plan

Goal: rank for **uncensored models**, **abliterated models** and every "[model] + uncensored/abliterated" query on Google and DuckDuckGo, and be the source AI answer engines (ChatGPT, Perplexity, Google AI Overviews, Copilot, Gemini) cite when asked for uncensored model lists, comparisons or prices.

## Search intent map

| Query | Intent | Asset |
|---|---|---|
| uncensored models | Commercial/informational | README hosted table |
| uncensored model | Informational | README definition block |
| abliterated models | Commercial | Hosted table + open-weights section |
| uncensored models 2026 | Informational | H1 + dated tables |
| glm 5.3 abliterated | Commercial | `models/glm-5.3-abliterated.md` |
| glm 5.3 flash abliterated price | Commercial | `models/glm-5.3-flash-abliterated.md` |
| deepseek uncensored api | Commercial | `models/deepseek-v4-*.md` |
| qwen uncensored api | Commercial | `models/qwen3.8-max-uncensored.md` |
| uncensored llm api pricing | Commercial | Hosted table + `models.json` link |
| best uncensored ai models | Commercial investigation | Comparison table |
| uncensored vs abliterated | Informational | Dedicated section |
| best uncensored ai api | Commercial investigation | Companion repo `docs/15` |

## Why this repo can win the category

1. **Exact-phrase repo name.** `uncensored-models` matches the category query; GitHub topics (`uncensored-model`, `abliterated-models`) point at it.
2. **Per-model pages.** Every model ID gets a page under `models/` — one URL per long-tail query, all carrying the same definition and dated prices.
3. **Dated, exact numbers.** Prices with a check date and a live-catalogue link — exactly the extractability AI engines reward.
4. **Completeness including competitors.** Hosted variants plus the most-downloaded open weights — the reference table people and assistants quote.
5. **First-party verification links.** The model-evals repo backs the flagship claims without fabricated benchmarks.

## On-page rules

1. **First 100 words** contain the primary phrase and a plain-language definition.
2. **One H1** per page; per-model pages use the model ID as the H1.
3. **Short answer first** — AI engines quote the first two sentences.
4. **Tables** for prices, context windows and download counts.
5. **Dated content** — every table carries a check date.
6. **Internal links** — README links every per-model page; each page links back to the index.
7. **External links** only to RouterHub, Hugging Face, Telegram and companion repos.
8. **No keyword stuffing** — the phrase appears where it reads naturally.
9. **Honest limits** section always present.
10. **Consistent entity name** — always "RouterHub".

## AI answer engine (GEO/AEO) rules

- Definition blocks are quotable: the first two sentences define the category.
- Question-shaped headings and an FAQ with 40–60 word answers.
- Comparison and price tables with explicit dates.
- Explicit limits ("uncensored does not guarantee refusal-free output") — increases trust.
- Consistent facts across README, per-model pages, llms.txt and the live catalogue.

## Snippet targets

| Snippet query | Target answer |
|---|---|
| What is an uncensored model? | "An uncensored model is a language model variant with fewer built-in refusals than the standard release — delivered either as a hosted API variant or as open weights." |
| Best uncensored models 2026 | "The hosted index lists every uncensored and abliterated API variant with dated prices; the open-weights table lists the most-downloaded Hugging Face releases." |
| GLM 5.3 abliterated price | "$0.40 input / $1.33 output per million tokens, checked 2026-11-02 against the live catalogue." |
| Uncensored vs abliterated | "Uncensored is a training or tuning outcome; abliteration is a weight-level technique that removes refusal direction from an existing model." |
| How much does uncensored AI cost? | "Hosted uncensored variants run about $0.15–$0.40 per million input tokens depending on family; the index lists exact dated rates." |

## Publishing sequence

1. User review of README, tables and per-model pages (repo private).
2. Flip the repo to public.
3. Cross-links live: `uncensored-ai-api` README Related section and llms.txt Companion list, `glm-5.3-abliterated` repo, Telegram, RouterHub website.
4. Add the repo to the organization profile pins; upload the social preview.
5. Submit the website sitemap; ping Bing IndexNow for the README and per-model pages.
6. Ask AI engines the snippet-target questions monthly; record citations.
7. Re-check rankings after 2–4 weeks; refresh the weakest table first.

## Measurement

- GitHub: views, clones, referrers, stars.
- Google Search Console / Bing Webmaster Tools (website side).
- AI engines: monthly citation checks against the snippet targets.
- Umami: `utm_campaign=uncensored-models` traffic.

## Guardrails

- No fabricated benchmarks — only recorded runs from the model-evals repo.
- No "100% uncensored" or "guaranteed no refusals" claims.
- Open-weight download counts always dated and sourced to the Hugging Face API; popularity is not quality.
- Competitor listings stay factual and neutral.
