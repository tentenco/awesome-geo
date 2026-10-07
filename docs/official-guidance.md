# Official AI-search guidance

Last reviewed: 2026-10-07

This is the primary-source layer of the project. It distinguishes **search inclusion**, **model training**, and **user-triggered retrieval** because one robots directive rarely controls all three.

## Google Search

### What Google currently says

[AI features and your website](https://developers.google.com/search/docs/appearance/ai-features) is the canonical starting point. For AI Overviews and AI Mode:

- A supporting page must be indexed and eligible to appear in Search with a snippet.
- There are no additional technical requirements beyond ordinary Search eligibility.
- Google may use query fan-out to search multiple subtopics and sources.
- Important content should be available as text; images and video can supplement it.
- Structured data should match visible content.
- Existing preview controls such as `nosnippet`, `data-nosnippet`, `max-snippet`, and `noindex` affect how content may appear.
- Search eligibility does not guarantee crawling, indexing, retrieval, citation, or traffic.

### Google's 2026 myth-busting

For Google Search specifically, the guide says there is no special advantage from:

- `llms.txt` or other AI-specific files/markup;
- mechanically splitting content into tiny chunks;
- rewriting pages solely for AI systems;
- manufacturing mentions on third-party sites.

Clear structure can still help people, and `llms.txt` can still be used by products that explicitly consume it. The narrow claim is that these are not special Google AI Search requirements.

### Canonical Google references

- [Search documentation updates](https://developers.google.com/search/updates)
- [Search Essentials](https://developers.google.com/search/docs/essentials)
- [Technical requirements](https://developers.google.com/search/docs/essentials/technical)
- [Spam policies](https://developers.google.com/search/docs/essentials/spam-policies)
- [Creating helpful, reliable, people-first content](https://developers.google.com/search/docs/fundamentals/creating-helpful-content)
- [Structured data guidelines](https://developers.google.com/search/docs/appearance/structured-data/sd-policies)
- [Robots meta tag and `X-Robots-Tag`](https://developers.google.com/search/docs/crawling-indexing/robots-meta-tag)
- [Google crawler overview](https://developers.google.com/search/docs/crawling-indexing/overview-google-crawlers)
- [Search Console generative AI reports](https://developers.google.com/search/blog/2026/06/gen-ai-performance-reports)

## Microsoft and Bing

[AI Performance in Bing Webmaster Tools](https://blogs.bing.com/webmaster/February-2026/Introducing-AI-Performance-in-Bing-Webmaster-Tools-Public-Preview) is the key 2026 operational resource. It documents citations, cited URLs, sampled grounding queries, and trends.

Additional official references:

- [Bing Webmaster Guidelines](https://www.bing.com/webmasters/help/webmaster-guidelines-30fba23a)
- [The evolving role of the index](https://blogs.bing.com/search/May-2026/Evolving-role-of-the-index-From-ranking-pages-to-supporting-answers)
- [Content controls for Bing Chat](https://blogs.bing.com/webmaster/september-2023/Announcing-new-options-for-webmasters-to-control-usage-of-their-content-in-Bing-Chat)
- [IndexNow documentation](https://www.indexnow.org/documentation)

Microsoft's useful distinction is that classic search ranks candidate pages, while grounding selects evidence that an AI system can use to support an answer. They share infrastructure but have different evaluation problems.

## OpenAI

- [Publisher FAQ](https://help.openai.com/en/articles/12627856) — Inclusion in ChatGPT search, `OAI-SearchBot`, `noindex`, citations, and analytics.
- [Crawler documentation](https://platform.openai.com/docs/bots) — Current user agents and controls.
- [Introducing ChatGPT search](https://openai.com/index/introducing-chatgpt-search/) — Product and publisher context.

OpenAI distinguishes search discovery from training controls. Review the current crawler page rather than copying an old robots snippet: names and behavior may change.

## Anthropic

- [Does Anthropic crawl data from the web?](https://support.anthropic.com/en/articles/8896518-does-anthropic-crawl-data-from-the-web-and-how-can-site-owners-block-the-crawler) — Official crawler purposes and block controls.
- [Web search tool documentation](https://docs.anthropic.com/en/docs/agents-and-tools/tool-use/web-search-tool) — How web search works for API applications; useful context, not a ranking guide.

## Perplexity

- [Official bots guide](https://docs.perplexity.ai/guides/bots) — User agents and robots behavior.

## Crawler-control matrix

Always verify the linked live documentation before deployment.

| Operator | Discovery/search purpose | Training purpose | Important distinction |
| --- | --- | --- | --- |
| Google | `Googlebot` and documented special-case crawlers | `Google-Extended` controls certain Gemini/Vertex grounding and training uses | Blocking `Google-Extended` does not remove a page from Google Search. |
| OpenAI | `OAI-SearchBot`; user actions may use `ChatGPT-User` | `GPTBot` | Search inclusion and training are separate controls. |
| Anthropic | See current official crawler page | See current official crawler page | Anthropic documents multiple tokens by purpose; do not assume one rule covers all use. |
| Perplexity | `PerplexityBot`; user-triggered access may differ | See current official bots guide | Follow the current guide and validate access in server logs. |
| Microsoft | Bing crawl/index infrastructure | Microsoft documents `NOCACHE`/`NOARCHIVE` behavior for certain Bing Chat uses | Controls can affect snippets, answers, and training differently. |

## Practical controls audit

1. Inventory `robots.txt`, meta robots, `X-Robots-Tag`, CDN/WAF rules, paywall behavior, and authentication.
2. Decide separately whether you want traditional search inclusion, generative-answer inclusion, user-directed retrieval, and training.
3. Apply the smallest control that matches the policy decision.
4. Test with server logs and first-party webmaster tools; a validator cannot prove downstream use.
5. Record the decision owner and review date. Recheck quarterly because crawler documentation changes.

## Observed crawler-control shifts (September 2026)

- [Cloudflare's September 15 change and AI crawler refusals](https://www.semrush.com/blog/cloudfare-blocks-ai-training/) — Pre/post analysis of 1,046 sites reporting higher refusal rates for training crawlers (ClaudeBot 19.9→22.8%, GPTBot 18.9→22.0%) alongside sharp drops for search crawlers (OAI-SearchBot 16.9→3.0%, Perplexity-User 14.9→2.2%), with controls flat.
  Evidence: vendor/secondary. Published or materially updated: 2026-09. Limitations: secondary vendor analysis of a third-party change; verify dates, sample, and bot classifications in server logs before acting.

## No universal “GEO compliance” standard

Schema.org, robots.txt, sitemaps, IndexNow, HTTP status codes, canonical links, and accessibility standards are real technical building blocks. There is currently no cross-platform standard that guarantees inclusion or ranking in generated answers. Treat any “one file unlocks every LLM” claim as unverified unless each named platform documents support.
