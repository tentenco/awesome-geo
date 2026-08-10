# GEO/AEO in 2026: verified landscape

Status: living document · Snapshot: 2026-08-10 · Scope: items first published or materially launched in 2026

This page separates dated changes from evergreen advice. Inclusion means the event or publication is relevant and verifiable; it is not an endorsement.

## Executive summary

Three shifts define 2026 so far:

1. **First-party measurement arrived.** Bing and Google introduced dedicated reporting for AI citations or generative-search impressions.
2. **Platforms challenged “special hack” narratives.** Google's first dedicated guide says ordinary eligibility and SEO fundamentals remain the basis for its AI features; `llms.txt`, machine-only rewrites, artificial mentions, and arbitrary content chunking do not receive special treatment.
3. **Measurement matured.** New research treats AI visibility as a stochastic distribution across prompts, runs, models, locations, and time—not a fixed rank.

## Verified timeline

### February

**2026-02-03 — Applied GEO research for Pinterest**  
[Generative Engine Optimization: A VLM and Agent Framework for Pinterest Acquisition Growth](https://arxiv.org/abs/2602.02961) presents a domain-specific agent and vision-language-model framework. Evidence class: preprint. Do not generalize its results to every engine or vertical.

**2026-02-10 — Bing Webmaster Tools AI Performance public preview**  
[Microsoft's announcement](https://blogs.bing.com/webmaster/February-2026/Introducing-AI-Performance-in-Bing-Webmaster-Tools-Public-Preview) documents total citations, average cited pages, sampled grounding queries, URL-level citation activity, and time trends across Microsoft Copilot, Bing AI summaries, and selected integrations. Evidence class: official.

### March

**2026-03-02 — AgenticGEO preprint**  
[AgenticGEO](https://arxiv.org/abs/2603.20213) proposes a self-evolving optimization system. Evidence class: preprint; the paper is useful for research directions, not a platform-endorsed playbook.

**2026-03-17 — Semrush 2026 trend guide**  
[AI Search Trends for 2026](https://www.semrush.com/blog/ai-search-trends/) summarizes the vendor's view of multimodal search, AI citations, and monitoring. Evidence class: vendor editorial.

### April

**2026-04-08 — Repeated-measurement research**  
[Don't Measure Once](https://arxiv.org/abs/2604.07585) argues that stochastic AI answers make one-off visibility checks unreliable. Evidence class: preprint. Operational implication: preserve raw answers and report repeated-run distributions.

### May

**2026-05-06 — Microsoft explains grounding indexes**  
[The evolving role of the index](https://blogs.bing.com/search/May-2026/Evolving-role-of-the-index-From-ranking-pages-to-supporting-answers) distinguishes a search system selecting pages from a grounding system selecting evidence for an answer. Evidence class: official engineering/product perspective.

**2026-05-15 — Google publishes its dedicated generative AI Search guide**  
[AI features and your website](https://developers.google.com/search/docs/appearance/ai-features) explains query fan-out, eligibility, content guidance, controls, measurement, AI agents, and myths. Google's [dated documentation log](https://developers.google.com/search/updates) verifies the addition. Evidence class: official.

Key scope note: this guide describes **Google Search**. Its statements should not automatically be attributed to ChatGPT, Claude, Perplexity, or Copilot.

**2026-05-27 — Preferred Sources begins extending to AI features**  
Google's [Search documentation log](https://developers.google.com/search/updates) says Preferred Sources started rolling out to AI Overviews and AI Mode. Evidence class: official.

### June

**2026-06-03 — Google Search Generative AI performance reports**  
[Google's announcement](https://developers.google.com/search/blog/2026/06/gen-ai-performance-reports) describes dedicated Search Console views for generative AI impressions in Search and Discover, initially rolled out to a subset of sites. Dimensions include page, country, device, and date. Evidence class: official.

**2026-06-03 — Semrush operational-gap study**  
[Only 22% of marketers have fully integrated AI search and SEO](https://www.semrush.com/blog/the-operational-gap-ai-seo-study/) reports survey results and investment priorities. Evidence class: vendor study; inspect sample and methodology before quoting.

**2026-06-16 — Google clarifies AI Mode counting**  
Google's [documentation log](https://developers.google.com/search/updates) states that AI Mode is counted toward Search Console totals. Evidence class: official.

### July

**2026-07-15 — Critical survey of GEO research**  
[Optimizing Visibility in Generative Engines: A Critical Survey of GEO (2023–2026)](https://arxiv.org/abs/2607.14035) reviews 45 studies and proposes a reproducible measurement protocol. Evidence class: preprint. Its useful corrective is that citation, mention, retrieval, prominence, and downstream effects are different outcomes.

**2026-07-29 — Google adds social/video analysis guidance**  
Google's [documentation log](https://developers.google.com/search/updates) records a new Search Console guide for analyzing social and video platform content. This matters because discovery is increasingly cross-surface. Evidence class: official.

## Verified product launches and updates

These links document a 2026 launch or material update. They do **not** independently validate the vendor's effectiveness.

| Date | Product update | Category | Evidence |
| --- | --- | --- | --- |
| 2026-02-05 | [Amplitude AI Visibility 1.5](https://amplitude.com/blog/amplitude-expands-ai-visibility) | Free monitoring/content workflow update | Vendor announcement |
| 2026-02-10 | [Bing Webmaster Tools AI Performance](https://blogs.bing.com/webmaster/February-2026/Introducing-AI-Performance-in-Bing-Webmaster-Tools-Public-Preview) | First-party citation analytics | Official |
| 2026-05-26 | [Onclusive GEO Analytics](https://news-en.onclusive.com/news/onclusive-launches-geo-analytics-to-measure-brand-visibility-in-ai-search) | PR/media + AI visibility | Vendor announcement |
| 2026-06-03 | [Google Search Console Generative AI reports](https://developers.google.com/search/blog/2026/06/gen-ai-performance-reports) | First-party impression analytics | Official, limited rollout |
| 2026-06-16 | [Jasper GEO Agent and GEO Hub](https://www.jasper.ai/blog/geo-agent-and-geo-hub) | Enterprise agent/workflow | Vendor announcement |
| 2026-06 | [Semrush 2026 AI Visibility Index](https://www.semrush.com/news/463141-semrush-releases-expanded-2026-ai-visibility-index-analyzing-126-million-ai-search-prompts/) | Cross-platform dataset/report | Vendor announcement |

## Concepts that became operational in 2026

- **Grounding query** — A retrieval query generated by an AI system to find evidence. Bing began exposing a sample in Webmaster Tools.
- **Query fan-out** — Multiple related searches across subtopics and data sources. Google documented this explicitly for AI Mode and AI Overviews.
- **Citation distribution** — The probability of a source being cited across repeated runs, rather than a single observed citation.
- **Evidence strength** — Whether retrieved material is accurate, fresh, attributable, and consistent enough to ground an answer.
- **Non-commodity content** — Original value that cannot be reproduced by generic summarization: first-party evidence, expertise, local information, unique products, tools, or analysis.
- **Agent readiness** — Making product, service, policy, and transaction information accurate and accessible enough for user-directed agents. This remains an emerging area; avoid claiming a universal agent-optimization standard.

## Claims to retire or qualify

| Claim | Better statement |
| --- | --- |
| “Install `llms.txt` to rank in Google AI.” | Google says it receives no special treatment for AI Overviews or AI Mode. Use it only when a specific consumer and use case justify it. |
| “One prompt test proves our GEO rank.” | Repeat prompts across runs, dates, engines, and relevant locales; preserve raw outputs. |
| “Schema makes an LLM cite you.” | Valid structured data can help machines understand eligible content, but no platform promises citations merely because markup exists. |
| “GEO replaces SEO.” | Crawlability, indexing, information quality, reputation, and user value remain foundations; AI visibility adds surfaces and metrics. |
| “Reddit mentions guarantee LLM visibility.” | Authentic community knowledge can be retrieved, but engineered promotion is unreliable, unethical, and often prohibited. |

## Update protocol

When adding a 2026 item, include the exact publication or launch date, original source, evidence class, one-sentence significance, and any rollout or methodology limitation. Move undated evergreen material to the topic documents rather than this timeline.
