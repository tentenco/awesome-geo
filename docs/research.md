# GEO/AEO research and datasets

Last reviewed: 2026-10-07

Research status matters. “Preprint” means the work is public but should not be presented as peer-reviewed evidence unless a venue is independently verified.

## Foundational work

- **GEO: Generative Engine Optimization** — KDD 2024 research introducing the term, GEO-Bench, visibility metrics, and controlled optimization experiments. [Paper](https://arxiv.org/abs/2311.09735) · [project](https://generative-engines.com/GEO/) · [code](https://github.com/GEO-optim/GEO)
- **Retrieval-Augmented Generation for Knowledge-Intensive NLP Tasks** — Foundational RAG architecture underlying much contemporary grounded-answer discussion. [Paper](https://arxiv.org/abs/2005.11401)
- **WebGPT: Browser-assisted question-answering with human feedback** — Early work on browsing, source use, and citation-oriented answer generation. [Paper](https://arxiv.org/abs/2112.09332)
- **Lost in the Middle** — Evidence that information position can affect long-context use. Relevant background, but not a direct GEO recipe. [Paper](https://arxiv.org/abs/2307.03172)

## New in 2026

- **Generative Engine Optimization: A VLM and Agent Framework for Pinterest Acquisition Growth** — Applied multimodal/agent framework. Preprint, 2026-02-03. [Paper](https://arxiv.org/abs/2602.02961)
- **AgenticGEO: A Self-Evolving Agentic System for Generative Engine Optimization** — Agentic optimization proposal. Preprint, 2026-03-02. [Paper](https://arxiv.org/abs/2603.20213)
- **Don't Measure Once: Measuring Visibility in AI Search (GEO)** — Focuses on probabilistic variation and repeated measurement. Preprint, 2026-04-08. [Paper](https://arxiv.org/abs/2604.07585)
- **GEO Creates Underexamined Risks** — Position paper on concentration, disclosure, governance, and academic blind spots. Preprint, 2026-05-18. [Paper](https://arxiv.org/abs/2606.12439)
- **Optimizing Visibility in Generative Engines: A Critical Survey (2023–2026)** — Reviews 45 studies, competing metrics, causal limits, risks, and reproducibility. Preprint, 2026-07-15. [Paper](https://arxiv.org/abs/2607.14035)

## Industry studies worth auditing

These can reveal large-scale patterns but have commercial incentives. Read the method, sampling frame, engine/interface dates, and denominator before quoting a number.

- [Semrush 2026 AI Visibility Index](https://www.semrush.com/news/463141-semrush-releases-expanded-2026-ai-visibility-index-analyzing-126-million-ai-search-prompts/) — Vendor announcement for a 126-million-prompt analysis.
- [Semrush operational-gap study](https://www.semrush.com/blog/the-operational-gap-ai-seo-study/) — 2026 marketer adoption survey.
- [Semrush AI search trends](https://www.semrush.com/blog/ai-search-trends/) — 2026 vendor editorial and data synthesis.
- [Ahrefs AI search research](https://ahrefs.com/blog/category/ai-search/) — Ongoing studies with query and citation datasets; verify each article's date and method separately.
- **AthenaHQ State of AI Search 2026** — Vendor benchmark reporting millions of responses across 8 LLMs: the average brand is mentioned in 16.3% of target responses, leaders reach 56.5%, and ~16% of owned-domain content goes uncited. Status: vendor.
  Published: 2026-09-29. [Press release](https://www.globenewswire.com/news-release/2026/09/29/3370800/0/en/new-report-finds-average-brand-is-invisible-in-84-of-target-responses-in-ai-search.html)
  Limitations: vendor-designed sample and undisclosed prompt panel; prefer the original AthenaHQ report over syndicated copies when available.
- **Per-engine citation leaders, September 2026 (Ahrefs Brand Radar synthesis)** — Third-party synthesis of Ahrefs data across 3M+ US queries per engine: YouTube leads AI Overviews (22.9%), Reddit leads AI Mode/Gemini/ChatGPT/Perplexity, Amazon tops Copilot. Status: vendor-data synthesis.
  Published: 2026-09-02. [Synthesis](https://netcontentseo.com/article/there-is-no-single-ai-citation-strategy-reddit-leads-four-engines-youtube-leads-ai-overviews-and-amazon-dominates-copilot-1000)
  Limitations: secondary synthesis, not Ahrefs primary output; verify query sets and date windows before quoting per-engine shares.
- **OtterlyAI AI Citations Report 2026** — Vendor report on citation frequency, third-party authority, and the shift from SEO metrics to entity alignment. Status: vendor.
  Published: 2026. [Report](https://otterly.ai/blog/theaicitationsreport-2026/)
  Limitations: commercially interested sample and methodology; confirm exact publication date and denominators before citing.
- **What Is llms.txt and Does It Work? (depra.ai study mirror)** — Independent India-shopping study finding 53% of cited sites had an `llms.txt` but no evidence any major engine uses it for citation decisions; Google states it ignores the file. Status: independent.
  Published: 2026-09-15. [Mirror](https://dev.to/ifham_baig_2d0ab31dae97b3/what-is-llmstxt-and-does-it-work-1k49)
  Limitations: dev.to mirror of the original depra.ai write-up; domain- and market-specific sample, not a cross-platform causal test.

## How to evaluate a GEO study

### Population and sampling

- Were prompts taken from real behavior, generated from keywords, or authored by researchers?
- Which topics, languages, locations, engines, account states, and dates were represented?
- Is the sample representative of the claim being made?

### Experimental design

- Were prompts and content interventions pre-specified?
- Were multiple runs used to handle stochastic output?
- Was there a baseline, control, randomization, or matched comparison?
- Were engine/model updates documented during collection?

### Metric validity

- Is “visibility” a mention, retrieval, citation, citation prominence, attributed text, or user action?
- Does the metric distinguish accurate from inaccurate mentions?
- Are missing answers, refusals, tool failures, and citation-free answers in the denominator?

### Reproducibility and conflicts

- Are prompts, code, raw outputs, annotations, and dates available?
- Can another team reproduce the score?
- Is the study selling the tool or technique it concludes is necessary?
- Are affiliations, funding, and limitations disclosed?

## Open research needs

- Longitudinal datasets spanning engine updates and locales
- Standardized, privacy-aware prompt panels based on real information needs
- Human-validated citation correctness and claim-level attribution
- Causal experiments separating content changes from index/model drift
- Better measurement of referrals, assisted conversions, and zero-click value
- Audits of bias, market concentration, publisher impact, manipulation, and spam
- Reproducible comparisons of crawler controls and freshness
- Non-English and non-US benchmarks

## Contribution format

```markdown
- **Title** — One neutral sentence. Status: peer-reviewed/preprint/vendor/independent.
  Published: YYYY-MM-DD. [Paper](...) · [Code](...) · [Data](...)
  Limitations: ...
```

