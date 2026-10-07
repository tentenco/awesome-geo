# Measuring AI search visibility

Last reviewed: 2026-10-07

AI visibility is not a single rank. The same prompt can produce different sources across runs, models, dates, locations, accounts, and interface states. A defensible program measures a distribution and keeps the raw evidence.

## Measurement stack

### Layer 1: eligibility

Track whether the intended URL is crawlable, indexable, canonical, renderable, and permitted for the relevant bot. Use server logs, Google Search Console, Bing Webmaster Tools, URL inspection, and robots tests.

### Layer 2: retrieval and citation

For each prompt and engine, record:

- whether the brand/entity is mentioned;
- whether a first-party URL is cited;
- which third-party sources are cited;
- citation position or prominence, if the interface exposes it;
- whether the cited source supports the nearby claim;
- answer accuracy, sentiment, and material omissions.

### Layer 3: demand and traffic

Measure AI referrals, landing pages, engaged sessions, assisted conversions, branded-search changes, and direct traffic cautiously. Referrer preservation varies by product and interface.

### Layer 4: business outcome

Connect exposure to qualified leads, sales, subscriptions, support deflection, or another declared outcome. Mentions without relevance or accuracy are not necessarily valuable.

## Core metrics

| Metric | Definition | Caveat |
| --- | --- | --- |
| Mention rate | Runs containing the entity / valid runs | A mention may be negative or inaccurate. |
| Citation rate | Runs citing an owned URL / valid runs | Citation does not prove the source determined the answer. |
| Source share of voice | Brand citations or mentions / category total in the same prompt panel | Prompt selection strongly affects the result. |
| Accurate-answer rate | Runs passing a predefined factual rubric / assessed runs | Requires human review or a validated evaluator. |
| Citation diversity | Unique cited domains or URLs over the period | More diversity is not always better. |
| Stability | Variation across repeat runs and periods | Low stability requires larger samples. |
| Qualified AI referral rate | Qualified AI sessions / all measurable AI referrals | Some interfaces hide or strip referrers. |
| Outcome rate | Desired outcomes / measurable AI referrals or exposed cohort | Attribution is incomplete and often directional. |

## Minimum viable experiment

1. Select 20–50 prompts from real customer research, grouped by discovery, comparison, validation, and purchase/support intent.
2. Freeze prompt text and document locale, account state, engine, model/interface, and date.
3. Run each prompt at least five times per measurement window when practical.
4. Store the full answer, citations, timestamp, engine, and run identifier.
5. Score mentions, owned citations, competitor citations, accuracy, and sentiment with a written rubric.
6. Report proportions and variability; do not turn one run into a “rank.”
7. Change one content or distribution variable at a time where feasible.
8. Re-run on a fixed cadence and annotate engine or product changes.

The 2026 preprint [Don't Measure Once](https://arxiv.org/abs/2604.07585) provides the core rationale for repeated observations. The [critical GEO survey](https://arxiv.org/abs/2607.14035) provides a broader review and reproducibility protocol. Both are preprints, not platform specifications.

## Prompt panel design

A useful panel samples the customer journey:

- **Category:** “What types of tools solve X?”
- **Problem:** “How should a team diagnose Y?”
- **Comparison:** “Compare A and B for this context.”
- **Recommendation:** “What are reliable options for this constraint?”
- **Validation:** “What are the limitations or complaints about A?”
- **Entity fact:** “What is A's policy, price, compatibility, or location?”
- **Task/agent:** “Find or prepare the next step for X,” only where the product supports it.

Do not create a panel solely from prompts where the brand is already named; that measures answer representation, not unprompted discovery.

## First-party reporting in 2026

- [Google Search Console Generative AI performance reports](https://developers.google.com/search/blog/2026/06/gen-ai-performance-reports) expose generative-feature impressions and dimensions for a limited rollout. They do not turn every AI answer into a conventional keyword report.
- [Bing Webmaster Tools AI Performance](https://blogs.bing.com/webmaster/February-2026/Introducing-AI-Performance-in-Bing-Webmaster-Tools-Public-Preview) exposes citation counts, cited pages, sampled grounding queries, and trends for supported Microsoft experiences.

Use first-party reporting as the anchor. Use third-party trackers to add cross-engine sampling, raw-answer archives, competitor comparisons, and workflow—not as an unquestionable source of “search volume.”

## Practitioner guides and benchmarks (added October 2026)

- [How to Track AI Search Visibility in 2026: Complete GEO Measurement Guide](https://dev.to/edo911/how-to-track-ai-search-visibility-in-2026-the-complete-geo-measurement-guide-4fka) — Practitioner guide built around a citation-rate metric, a 12-query starter method, and a weekly routine compatible with the minimum viable experiment above.
  Evidence: community. Published or materially updated: 2026-09-11. Limitations: single author's workflow; adapt prompt panel and run counts to your own surface before adopting.
- [AthenaHQ State of AI Search 2026](https://www.globenewswire.com/news-release/2026/09/29/3370800/0/en/new-report-finds-average-brand-is-invisible-in-84-of-target-responses-in-ai-search.html) — Vendor benchmark across 8 LLMs useful for calibrating mention-rate expectations (average 16.3% mentioned).
  Evidence: vendor. Published or materially updated: 2026-09-29. Limitations: vendor sample; read method and denominator before quoting. Full notes in [research](research.md).
- [OtterlyAI AI Citations Report 2026](https://otterly.ai/blog/theaicitationsreport-2026/) — Vendor report on citation frequency and third-party authority patterns.
  Evidence: vendor. Published or materially updated: 2026. Limitations: exact date and methodology unconfirmed; treat as directional.

## Vendor evaluation questions

- Are prompts real, inferred, generated, or customer-supplied?
- How many repeats are run, and how is variance shown?
- Which exact engines, interfaces, locales, and account states are sampled?
- Are raw answers, citations, timestamps, and screenshots exportable?
- How are brand aliases, ambiguous names, sentiment, and citation positions scored?
- Are retries, errors, safety refusals, and missing citations included in the denominator?
- Can methodology changes be distinguished from real visibility changes?
- What data is retained, and can sensitive prompts be excluded from model training?

## Reporting template

```text
Measurement window:
Engines/interfaces:
Markets/locales:
Prompt panel version:
Runs per prompt:
Valid/failed runs:

Mention rate (with denominator):
Owned citation rate (with denominator):
Accurate-answer rate (rubric linked):
Source share of voice:
Qualified referral outcomes:

Known product/method changes:
Interventions during period:
Limitations:
Raw evidence location:
```

