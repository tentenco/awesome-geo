# Awesome GEO, AEO & AI Search

[![Awesome](https://awesome.re/badge.svg)](https://awesome.re)
[![CC0 1.0](https://img.shields.io/badge/license-CC0--1.0-blue.svg)](LICENSE)
[![Contributions welcome](https://img.shields.io/badge/contributions-welcome-brightgreen.svg)](CONTRIBUTING.md)

> A community-curated, evidence-aware guide to Generative Engine Optimization (GEO), Answer Engine Optimization (AEO), AI search visibility, and the open web.

**[繁體中文](README-zh-TW.md)** · [简体中文](README-zh-CN.md) · [日本語](README-ja.md) · [한국어](README-ko.md) · [العربية](README-ar.md)

Last reviewed: **2026-10-07** · [What changed in 2026](docs/2026-landscape.md)

## Start here

- **New to the field?** Read the [practitioner's playbook](docs/playbook.md).
- **Need primary sources?** Use the [official guidance](docs/official-guidance.md).
- **Choosing software?** Compare the [tools and ecosystem](docs/tools.md).
- **Designing reporting?** Use the [measurement framework](docs/measurement.md).
- **Following the evidence?** Browse [research and datasets](docs/research.md).
- **Tracking practitioner debate?** See [Reddit's top 2026 discussions](docs/reddit-2026.md).

## What these terms mean

The industry does not use one stable taxonomy. This project uses the following working definitions:

| Term | Working definition | Primary outcome |
| --- | --- | --- |
| **GEO** | Improving whether a source or entity is retrieved, used, represented, or cited in a generated answer. | Citations, mentions, accurate representation |
| **AEO** | Making content eligible and useful for systems that provide a direct answer, including answer boxes, assistants, and generative search. | Answer inclusion and answer quality |
| **AI search visibility** | The umbrella measurement discipline across AI Overviews, AI Mode, ChatGPT, Copilot, Perplexity, Claude, Gemini, and similar products. | Visibility, share of voice, sentiment, referrals |
| **SEO** | Improving discovery, indexing, presentation, and performance in search engines. | Search visibility and qualified traffic |

These practices overlap. Google explicitly says its existing SEO fundamentals remain applicable to AI Overviews and AI Mode and that no special technical requirements are needed. Other answer engines have different crawlers, indexes, interfaces, and reporting, so their operational details must be evaluated separately.

## 2026: the signal, not the hype

These are the most consequential changes first published in 2026:

- **Google published dedicated generative-AI Search guidance** on 2026-05-15. It covers query fan-out, non-commodity content, multimodal and local information, AI agents, and myths about GEO/AEO. [Official guide](https://developers.google.com/search/docs/appearance/ai-features) · [announcement](https://developers.google.com/search/blog/2026/05/a-new-resource-for-optimizing)
- **Google Search Console introduced Generative AI performance reports** on 2026-06-03, initially for a subset of sites. The reports expose impressions, pages, countries, devices, and time trends for generative AI features. [Announcement](https://developers.google.com/search/blog/2026/06/gen-ai-performance-reports)
- **Bing Webmaster Tools introduced AI Performance** in public preview on 2026-02-10, including total citations, cited pages, grounding queries, and trends across Microsoft AI experiences. [Announcement](https://blogs.bing.com/webmaster/February-2026/Introducing-AI-Performance-in-Bing-Webmaster-Tools-Public-Preview)
- **Measurement became a research problem of its own.** New work argues that probabilistic answers require repeated runs and distributions, not a single prompt snapshot. [Don't Measure Once](https://arxiv.org/abs/2604.07585) · [2023–2026 critical survey](https://arxiv.org/abs/2607.14035)
- **The product category moved from monitoring toward workflows and agents.** Examples include Amplitude's expanded AI Visibility tool, Onclusive GEO Analytics, and Jasper's GEO Agent. These are vendor claims, not independent proof of effectiveness. [Ecosystem details](docs/tools.md#verified-2026-launches-and-major-updates)

Read the dated [2026 landscape and changelog](docs/2026-landscape.md) for the complete timeline and source notes.

## Official platform resources

### Google Search

- [AI features and your website](https://developers.google.com/search/docs/appearance/ai-features) — Eligibility, query fan-out, controls, measurement, and myth-busting.
- [Search documentation updates](https://developers.google.com/search/updates) — Dated canonical changelog; an RSS feed is available on the page.
- [Search Essentials](https://developers.google.com/search/docs/essentials) — Technical requirements, spam policies, and key best practices.
- [Helpful, reliable, people-first content](https://developers.google.com/search/docs/fundamentals/creating-helpful-content) — Google's content quality guidance.
- [Structured data introduction](https://developers.google.com/search/docs/appearance/structured-data/intro-structured-data) — Use supported markup that matches visible content; structured data is not a guaranteed GEO shortcut.
- [Google crawlers and fetchers](https://developers.google.com/search/docs/crawling-indexing/overview-google-crawlers) — User agents and crawl controls, including `Google-Extended` documentation links.

### Microsoft and Bing

- [AI Performance in Bing Webmaster Tools](https://blogs.bing.com/webmaster/February-2026/Introducing-AI-Performance-in-Bing-Webmaster-Tools-Public-Preview) — First-party citation reporting introduced in 2026.
- [The evolving role of the index](https://blogs.bing.com/search/May-2026/Evolving-role-of-the-index-From-ranking-pages-to-supporting-answers) — Microsoft's distinction between ranking pages and grounding answers.
- [IndexNow](https://www.indexnow.org/) — Open protocol for notifying participating engines of URL changes.
- [Bing Webmaster Guidelines](https://www.bing.com/webmasters/help/webmaster-guidelines-30fba23a) — Core crawl, index, and quality guidance.

### OpenAI and other answer engines

- [OpenAI publisher FAQ](https://help.openai.com/en/articles/12627856) — `OAI-SearchBot`, `noindex`, inclusion, citations, and referral tracking.
- [OpenAI crawler documentation](https://platform.openai.com/docs/bots) — Distinguishes search, user-triggered, and training-related user agents.
- [Anthropic web crawlers](https://support.anthropic.com/en/articles/8896518-does-anthropic-crawl-data-from-the-web-and-how-can-site-owners-block-the-crawler) — Anthropic's crawl controls.
- [Perplexity crawler documentation](https://docs.perplexity.ai/guides/bots) — Official user-agent and robots guidance.

See [official guidance](docs/official-guidance.md) for a crawler-control matrix and claims that should not be generalized across platforms.

## Essential research

- [GEO: Generative Engine Optimization](https://arxiv.org/abs/2311.09735) — The foundational paper; KDD 2024. Introduced GEO-Bench and experimental visibility interventions.
- [GEO project and benchmark](https://generative-engines.com/GEO/) — Project site, data, code, and benchmark context.
- [Don't Measure Once: Measuring Visibility in AI Search (GEO)](https://arxiv.org/abs/2604.07585) — 2026 preprint on repeated measurement under stochastic outputs.
- [Optimizing Visibility in Generative Engines: A Critical Survey (2023–2026)](https://arxiv.org/abs/2607.14035) — 2026 preprint reviewing terminology, metrics, evidence, risks, and reproducibility.
- [AgenticGEO](https://arxiv.org/abs/2603.20213) — 2026 preprint proposing an agentic optimization system.
- [GEO for Pinterest acquisition growth](https://arxiv.org/abs/2602.02961) — 2026 applied VLM/agent framework; treat its domain-specific findings cautiously.

Preprints are labelled as such and should not be treated as platform guarantees. More in [research and datasets](docs/research.md).

## Tool map

| Need | Start with | Notes |
| --- | --- | --- |
| Google AI feature visibility | [Google Search Console](https://search.google.com/search-console/about) | First-party; generative AI report has limited rollout as of this review. |
| Microsoft AI citations | [Bing Webmaster Tools](https://www.bing.com/webmasters/about) | First-party AI Performance public preview. |
| Open-source, self-hosted monitoring | [GetCito](https://github.com/ai-search-guru/getcito-worlds-first-open-source-aio-aeo-or-geo-tool) | Inspect license, provider costs, methodology, and security before deployment. |
| Multi-engine enterprise monitoring | Profound, Semrush, Ahrefs, BrightEdge, seoClarity | Compare prompt methodology, geographic coverage, raw evidence, export, and retention. |
| Mid-market monitoring | Peec AI, Otterly.AI, Scrunch AI, LLMrefs, Rankscale | Verify engines and prompt limits against your actual market. |
| Technical discovery | Search Console, Bing Webmaster Tools, IndexNow, crawler logs | Establish crawl/index eligibility before buying visibility software. |

This project does not rank vendors and accepts no paid placement. See the full [tool directory and evaluation checklist](docs/tools.md).

## Practical baseline

1. Make important pages crawlable, indexable, internally linked, canonical, fast enough to use, and available as text.
2. Publish original information: direct experience, primary data, clear methodology, named authors, and dated updates.
3. Make claims easy to verify with source links, definitions, tables, examples, and meaningful context.
4. Keep entity facts consistent across your site, profiles, product feeds, knowledge bases, and trusted third parties.
5. Use schema only when it matches visible content and a supported vocabulary; never use it to invent facts.
6. Measure each engine separately with a stable prompt set, repeated runs, raw answer capture, and business outcomes.
7. Treat synthetic mentions, fake reviews, undisclosed promotion, and community spam as abuse—not GEO.

The [playbook](docs/playbook.md) turns this baseline into a 30/60/90-day program.

## Evidence policy

Every submission should identify its evidence class:

- **Official** — Platform, standards body, regulator, or product owner.
- **Peer-reviewed** — Published academic work with venue and date.
- **Preprint** — Research not yet established by peer review.
- **Independent study** — Reproducible methodology and disclosed sample.
- **Vendor report** — Useful but commercially interested.
- **Community discussion** — Practitioner experience, hypothesis, or debate.

Popularity is not proof. A resource can be popular and still be misleading; an official statement can be limited to one platform. We preserve both the source and its scope.

## Community

- Read [CONTRIBUTING.md](CONTRIBUTING.md) before proposing a resource.
- Use the resource suggestion issue form for additions and corrections.
- Read [GOVERNANCE.md](GOVERNANCE.md) for maintainer responsibilities and transparent decision rules.
- Follow the [Code of Conduct](CODE_OF_CONDUCT.md) and report security issues through [SECURITY.md](SECURITY.md).
- Commercial tools are welcome when relevant, clearly disclosed, and described neutrally. Paid placement is not accepted.

## License

To maximize reuse, this curated collection is dedicated to the public domain under [CC0 1.0 Universal](LICENSE). Linked resources retain their original copyrights and licenses.
