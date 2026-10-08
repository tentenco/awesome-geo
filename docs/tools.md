# GEO/AEO tools and ecosystem

Last reviewed: 2026-10-07

This is a capability map, not a leaderboard. Pricing, coverage, and product behavior change frequently; verify them with the vendor before purchase. Commercial inclusion is unpaid.

## Choose the measurement before the tool

A credible tool should disclose enough to answer:

- Which engines, interfaces, models, locales, and devices does it sample?
- Where do prompts come from, and can you supply your own?
- Does it repeat prompts and report variability?
- Can you inspect and export raw answers, citations, timestamps, and errors?
- How are mentions, citation position, sentiment, and share of voice calculated?
- Are historical methodology changes documented?
- What are retention, privacy, API, seat, and prompt-volume limits?

See the full [measurement framework](measurement.md#vendor-evaluation-questions).

## First-party and open infrastructure

- [Google Search Console](https://search.google.com/search-console/about) — Search eligibility and performance. A dedicated generative AI report began limited rollout in June 2026.
- [Bing Webmaster Tools](https://www.bing.com/webmasters/about) — Crawl/index data plus AI Performance citations and grounding-query samples in 2026 public preview.
- [IndexNow](https://www.indexnow.org/) — Open change-notification protocol supported by participating engines.
- [Schema.org](https://schema.org/) — Community vocabulary for structured data; markup must reflect visible facts and does not guarantee citations.
- [GetCito](https://github.com/ai-search-guru/getcito-worlds-first-open-source-aio-aeo-or-geo-tool) — Self-hosted AI-visibility tracker. Review its license, code, provider/API costs, security, and scoring methodology before production use.
- [Princeton NLP GEO code](https://github.com/GEO-optim/GEO) — Research implementation and benchmark material associated with the foundational GEO work; not a production rank tracker.

## Cross-engine visibility and monitoring

### Enterprise

- [Profound](https://www.tryprofound.com/) — Multi-engine answer monitoring, citation/source analysis, and enterprise workflows.
- [Semrush AI Visibility](https://www.semrush.com/ai-visibility/) — AI visibility integrated with a broader SEO/competitive-research suite.
- [Ahrefs Brand Radar](https://ahrefs.com/brand-radar) — Brand mentions, citations, web visibility, and competitive discovery across search/AI datasets.
- [BrightEdge](https://www.brightedge.com/) — Enterprise search platform with AI-search monitoring and content workflows.
- [seoClarity](https://www.seoclarity.net/) — Enterprise SEO and AI visibility capabilities.
- [Conductor](https://www.conductor.com/) — Enterprise organic marketing platform with AI-search features.
- [Onclusive GEO Analytics](https://news-en.onclusive.com/news/onclusive-launches-geo-analytics-to-measure-brand-visibility-in-ai-search) — Combines AI answers with earned, broadcast, print, and social media intelligence.

### Teams and agencies

- [Peec AI](https://peec.ai/) — Prompt monitoring, citations, sentiment, and competitor share of voice.
- [Otterly.AI](https://otterly.ai/) — AI-search monitoring and citation tracking.
- [Scrunch AI](https://scrunch.ai/) — Brand visibility plus content/agent experience workflows.
- [LLMrefs](https://llmrefs.com/) — AI visibility and keyword/prompt tracking.
- [Rankscale](https://rankscale.ai/) — Multi-engine brand monitoring and analytics.
- [Corank](https://corank.ai/) — AI visibility audits and recurring monitoring across ChatGPT, Perplexity, Claude, Gemini, and Google AI Overviews, with source-role analysis and action recommendations.
- [AthenaHQ](https://www.athenahq.ai/) — AI-search monitoring, prompt research, and optimization workflows.
- [Writesonic GEO](https://writesonic.com/generative-engine-optimization-geo) — Monitoring and content workflow within the Writesonic platform.
- [SE Ranking AI Search Toolkit](https://seranking.com/ai-search/) — AI visibility integrated with an SEO suite.
- [Amplitude AI Visibility](https://amplitude.com/ai-visibility) — Free visibility entry point tied to Amplitude analytics/content workflows.
- [Contentpen 2.0](https://martechseries.com/predictive-ai/ai-platforms-machine-learning/contentpen-2-0-launches-as-an-all-in-one-seo-aeo-tool-with-ai-visibility-tracking-across-7-ai-engines/) — All-in-one SEO/AEO positioning with visibility tracking across ChatGPT, Google AI, Copilot, Gemini, Perplexity, Grok, and Claude (launch covered 2026-10-05; vendor claims unverified).

## Open-source GEO projects and agent skills

Added in the October 2026 sweep of trending GitHub projects active in the previous ~30 days. Star counts and activity dates are as reported on 2026-10-07 and were not independently re-fetched; inspect license, code, provider costs, and scoring methodology before production use. Inclusion is not an endorsement of effectiveness.

- [GEOFlow](https://github.com/yaojingang/GEOFlow) — Open-source GEO platform with AI-visibility tracking; dense September 2026 releases (v3.0.0/v3.1.0).
  Evidence: community. Published or materially updated: 2026-10-01. Limitations: ~3,758 stars as reported; release quality and measurement methodology unaudited.
- [nevoai-geo-platform](https://github.com/kwdos/nevoai-geo-platform) — Visibility tracking covering DeepSeek, Doubao, Yuanbao, and ERNIE citations plus share of voice; distinctive China-engine coverage.
  Evidence: community. Published or materially updated: 2026-10-07. Limitations: new project (created 2026-09-22); methodology and data quality unaudited.
- [open-geo](https://github.com/geofn-com/open-geo) — Self-described "Lighthouse for GEO": `llms.txt` generator/doctor, MCP server, and TypeScript CLI for audits.
  Evidence: community. Published or materially updated: 2026-09-14. Limitations: new project; audit scoring unaudited and `llms.txt` has no documented Google AI Search effect.
- [geo-optimizer-skill](https://github.com/auriti-labs/geo-optimizer-skill) — Audit-and-optimize toolkit for ChatGPT, Perplexity, Gemini, and AI Overviews citations (CLI, Python, MCP, Astro).
  Evidence: community. Published or materially updated: 2026-09-30. Limitations: ~1,012 stars as reported; citation-impact claims unaudited.
- [eGEOagents](https://github.com/mverab/eGEOagents) — Agent toolkit for refactoring content toward ChatGPT, Perplexity, Gemini, and Claude citations.
  Evidence: community. Published or materially updated: 2026-10-07. Limitations: ~197 stars as reported; rewrite effectiveness unaudited.
- [yao-geo-skills](https://github.com/yaojingang/yao-geo-skills) — Continuously updated collection of GEO agent skills from the same maintainer as GEOFlow.
  Evidence: community. Published or materially updated: 2026-10-01. Limitations: ~867 stars as reported; skill quality varies by task.
- [ai-visibility-framework](https://github.com/lifebricksglobal/ai-visibility-framework) — Open AEO/GEO framework combining RAG practice, `llms.txt`, and entity authority.
  Evidence: community. Published or materially updated: 2026-10-07. Limitations: new project (created 2026-09-27); framework outcomes unevaluated.
- [opengeo-platform](https://github.com/jack20002/opengeo-platform) — Self-hosted visibility platform with measurement, content studio, and attribution loop.
  Evidence: community. Published or materially updated: 2026-09-27. Limitations: new project; scoring and attribution methodology unaudited.
- [GEORank](https://github.com/yaojingang/GEORank) — Rank-measurement companion to GEOFlow from the same maintainer, active through September 2026.
  Evidence: community. Published or materially updated: 2026-09-16. Limitations: ~490 stars as reported; metric definitions unaudited.
- [genpark citation scorer skill](https://github.com/alphaparkinc/genpark-generative-engine-optimization-and-citation-scorer-skill) — Python skill scoring citation visibility in generative answers.
  Evidence: community. Published or materially updated: 2026-10-05. Limitations: very new and low-adoption; scorer validity unevaluated.

## Independent tool comparisons

- [5 AI Search Visibility Tools to Track Brand Mentions](https://growthner.com/blog/ai-search-visibility-tools-to-track-your-brand-mentions-in-llms/) — Third-party comparison of Semrush, Ahrefs, Profound, Peec, and Otterly ($29–$199), noting 91% of cited URLs appear in only one LLM.
  Evidence: independent. Published or materially updated: 2026-09-30. Limitations: single publisher's test design; verify engines, sample, and pricing before purchase.

## Technical, entity, and content infrastructure

- [Screaming Frog SEO Spider](https://www.screamingfrog.co.uk/seo-spider/) — Crawl audits, extraction, internal linking, rendering, and custom validation.
- [Sitebulb](https://sitebulb.com/) — Technical crawling, prioritization, and visualization.
- [Google Rich Results Test](https://search.google.com/test/rich-results) — Tests Google-supported rich-result markup, not “GEO rank.”
- [Schema Markup Validator](https://validator.schema.org/) — General Schema.org syntax and vocabulary validation.
- [OpenRefine](https://openrefine.org/) — Open-source cleanup and reconciliation for inconsistent entity data.
- [Wikidata Query Service](https://query.wikidata.org/) — Explore open knowledge-graph entities and identifiers; follow Wikidata sourcing and conflict-of-interest norms when editing.
- [Google Merchant Center](https://www.google.com/retail/solutions/merchant-center/) — First-party product feeds and commerce data for eligible Google surfaces.
- [Bing Places for Business](https://www.bingplaces.com/) and [Google Business Profile](https://www.google.com/business/) — Maintain accurate local entity facts.

## Verified 2026 launches and major updates

“Verified” means the date and launch are supported by a first-party announcement. It does not verify marketing performance claims.

- **Bing Webmaster Tools AI Performance** — Public preview announced 2026-02-10. [Official announcement](https://blogs.bing.com/webmaster/February-2026/Introducing-AI-Performance-in-Bing-Webmaster-Tools-Public-Preview)
- **Amplitude AI Visibility 1.5** — Expanded monitoring/content workflow announced 2026-02-05. [Vendor announcement](https://amplitude.com/blog/amplitude-expands-ai-visibility)
- **Onclusive GEO Analytics** — AI visibility inside a media-intelligence platform, announced 2026-05-26. [Vendor announcement](https://news-en.onclusive.com/news/onclusive-launches-geo-analytics-to-measure-brand-visibility-in-ai-search)
- **Google Search Console Generative AI reports** — Limited rollout announced 2026-06-03. [Official announcement](https://developers.google.com/search/blog/2026/06/gen-ai-performance-reports)
- **Jasper GEO Agent and GEO Hub** — Enterprise workflow announced on 2026-06-16. [Vendor announcement](https://www.jasper.ai/blog/geo-agent-and-geo-hub)
- **Semrush 2026 AI Visibility Index expansion** — Dataset expansion announced in June 2026. [Vendor announcement](https://www.semrush.com/news/463141-semrush-releases-expanded-2026-ai-visibility-index-analyzing-126-million-ai-search-prompts/)

## Tool-selection scorecard

Score each item 0 (absent), 1 (partial), or 2 (strong):

| Dimension | What good looks like |
| --- | --- |
| Audience fit | Engines, countries, languages, and prompt intents match real customers. |
| Method transparency | Prompt source, repetitions, scoring, failures, and product changes are disclosed. |
| Evidence access | Raw answers, citations, timestamps, and exports are available. |
| Variance handling | Repeated runs and uncertainty are visible rather than hidden in one score. |
| First-party integration | Search Console, Bing, analytics, logs, or warehouse data can be reconciled. |
| Actionability | Findings map to a source, page, fact, or workflow that can be improved. |
| Privacy/security | Retention, subprocessors, training use, SSO/RBAC, and deletion are acceptable. |
| Portability | API/export access prevents lock-in and allows independent audit. |
| Cost clarity | Prompt, engine, project, history, export, and seat limits are explicit. |

Run a time-boxed pilot with a frozen prompt panel. Compare raw evidence and repeatability, not dashboard polish alone.

## Submission policy for commercial tools

A tool submission must include a canonical URL, current supported engines, evidence/export method, pricing URL or “contact sales,” privacy policy, declared submitter affiliation, and one neutral sentence describing the actual capability. Affiliate links, unverifiable superlatives, copied listicle language, and paid placement are rejected.
