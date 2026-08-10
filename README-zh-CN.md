# Awesome GEO、AEO 与 AI 搜索

[![Awesome](https://awesome.re/badge.svg)](https://awesome.re)
[![CC0 1.0](https://img.shields.io/badge/license-CC0--1.0-blue.svg)](LICENSE)
[![欢迎贡献](https://img.shields.io/badge/contributions-welcome-brightgreen.svg)](CONTRIBUTING.md)

> 由社区共同维护、重视证据的生成式引擎优化（GEO）、答案引擎优化（AEO）、AI 搜索可见性与开放网络指南。

[English](README.md) · [繁體中文](README-zh-TW.md) · [日本語](README-ja.md) · [한국어](README-ko.md) · [العربية](README-ar.md)

最后审查：**2026-08-10** · [2026 年发生了什么变化](docs/2026-landscape.md)

## 从这里开始

- **刚接触这个领域？**阅读[实践手册](docs/playbook.md)。
- **需要第一手来源？**查阅[官方指南](docs/official-guidance.md)。
- **正在选择软件？**比较[工具与生态系统](docs/tools.md)。
- **正在设计报告？**使用[衡量框架](docs/measurement.md)。
- **想追踪研究证据？**浏览[研究与数据集](docs/research.md)。
- **想了解从业者争论？**查看 [Reddit 2026 热门讨论](docs/reddit-2026.md)。

## 这些术语代表什么

行业尚未采用统一且稳定的分类方式。本项目使用以下工作定义：

| 术语 | 工作定义 | 主要成果 |
| --- | --- | --- |
| **GEO** | 改善来源或实体在生成式回答中被检索、使用、呈现或引用的机会。 | 引用、提及、准确呈现 |
| **AEO** | 使内容适合提供直接答案的系统，包括答案框、助手和生成式搜索。 | 答案收录与答案质量 |
| **AI 搜索可见性** | 横跨 AI Overviews、AI Mode、ChatGPT、Copilot、Perplexity、Claude、Gemini 等产品的整体衡量领域。 | 可见性、声量份额、情感、引荐流量 |
| **SEO** | 改善搜索引擎中的发现、索引、呈现和效果。 | 搜索可见性与有效流量 |

这些实践高度重叠。Google 明确表示，现有 SEO 基础仍适用于 AI Overviews 和 AI Mode，而且无需额外的特殊技术条件。其他答案引擎采用不同的爬虫、索引、界面和报告，因此必须分别评估其操作细节。

## 2026：信号，而不是炒作

以下是 2026 年首次出现、影响最重大的变化：

- **Google 于 2026-05-15 发布生成式 AI 搜索专项指南。**内容涵盖 query fan-out、非同质化内容、多媒体与本地信息、AI agents，以及 GEO/AEO 误区。[官方指南](https://developers.google.com/search/docs/appearance/ai-features) · [公告](https://developers.google.com/search/blog/2026/05/a-new-resource-for-optimizing)
- **Google Search Console 于 2026-06-03 推出 Generative AI performance reports。**初期仅向部分网站开放，可查看生成式 AI 功能中的展示、页面、国家、设备和时间趋势。[公告](https://developers.google.com/search/blog/2026/06/gen-ai-performance-reports)
- **Bing Webmaster Tools 于 2026-02-10 推出 AI Performance public preview。**包括 Microsoft AI 体验中的总引用次数、被引用页面、grounding queries 和趋势。[公告](https://blogs.bing.com/webmaster/February-2026/Introducing-AI-Performance-in-Bing-Webmaster-Tools-Public-Preview)
- **衡量本身成为研究问题。**新研究认为，由于 AI 回答具有概率性和随机性，必须重复测量并观察分布，不能只看单次 prompt 截图。[Don't Measure Once](https://arxiv.org/abs/2604.07585) · [2023–2026 批判性综述](https://arxiv.org/abs/2607.14035)
- **产品类别从监测转向工作流与 agents。**Amplitude 扩展 AI Visibility、Onclusive 推出 GEO Analytics、Jasper 推出 GEO Agent。这些是厂商声明，不是独立的效果证明。[生态系统详情](docs/tools.md#verified-2026-launches-and-major-updates)

完整时间线和来源说明请参阅[2026 年趋势与变更记录](docs/2026-landscape.md)。

## 官方平台资源

### Google 搜索

- [AI 功能与您的网站](https://developers.google.com/search/docs/appearance/ai-features) — 收录资格、query fan-out、控制方式、衡量与误区澄清。
- [搜索文档更新记录](https://developers.google.com/search/updates) — 带日期的官方变更记录，页面也提供 RSS。
- [Google 搜索基础指南](https://developers.google.com/search/docs/essentials) — 技术要求、垃圾内容政策和主要最佳实践。
- [创建实用、可靠、以人为本的内容](https://developers.google.com/search/docs/fundamentals/creating-helpful-content) — Google 的内容质量指南。
- [结构化数据简介](https://developers.google.com/search/docs/appearance/structured-data/intro-structured-data) — 使用与可见内容一致的受支持标记；结构化数据不是保证 GEO 成效的捷径。
- [Google 爬虫与抓取工具](https://developers.google.com/search/docs/crawling-indexing/overview-google-crawlers) — User agent 和抓取控制，包括 `Google-Extended` 文档链接。

### Microsoft 与 Bing

- [Bing Webmaster Tools AI Performance](https://blogs.bing.com/webmaster/February-2026/Introducing-AI-Performance-in-Bing-Webmaster-Tools-Public-Preview) — 2026 年推出的第一方引用报告。
- [索引角色的演变](https://blogs.bing.com/search/May-2026/Evolving-role-of-the-index-From-ranking-pages-to-supporting-answers) — Microsoft 对页面排序和答案 grounding 的区分。
- [IndexNow](https://www.indexnow.org/) — 通知参与搜索引擎 URL 变化的开放协议。
- [Bing Webmaster Guidelines](https://www.bing.com/webmasters/help/webmaster-guidelines-30fba23a) — 抓取、索引和质量的核心指南。

### OpenAI 与其他答案引擎

- [OpenAI 发布者 FAQ](https://help.openai.com/en/articles/12627856) — `OAI-SearchBot`、`noindex`、收录、引用和引荐跟踪。
- [OpenAI 爬虫文档](https://platform.openai.com/docs/bots) — 区分搜索、用户触发和训练相关的 user agents。
- [Anthropic 网络爬虫](https://support.anthropic.com/en/articles/8896518-does-anthropic-crawl-data-from-the-web-and-how-can-site-owners-block-the-crawler) — Anthropic 官方抓取控制。
- [Perplexity 爬虫文档](https://docs.perplexity.ai/guides/bots) — 官方 user agent 和 robots 指南。

爬虫控制矩阵及不能跨平台套用的说法，请参阅[官方指南](docs/official-guidance.md)。

## 核心研究

- [GEO: Generative Engine Optimization](https://arxiv.org/abs/2311.09735) — 奠基论文，发表于 KDD 2024；提出 GEO-Bench 和可见性干预实验。
- [GEO 项目与 benchmark](https://generative-engines.com/GEO/) — 项目网站、数据、代码和 benchmark 背景。
- [Don't Measure Once](https://arxiv.org/abs/2604.07585) — 2026 预印本，讨论随机输出环境下的重复测量。
- [生成式引擎可见性批判性综述（2023–2026）](https://arxiv.org/abs/2607.14035) — 2026 预印本，回顾术语、指标、证据、风险和可复现性。
- [AgenticGEO](https://arxiv.org/abs/2603.20213) — 2026 预印本，提出 agentic 优化系统。
- [面向 Pinterest acquisition growth 的 GEO 框架](https://arxiv.org/abs/2602.02961) — 2026 年 VLM／agent 应用框架；应谨慎看待其特定领域结论。

预印本均有明确标记，不应被视为平台保证。更多内容请参阅[研究与数据集](docs/research.md)。

## 工具地图

| 需求 | 建议起点 | 注意事项 |
| --- | --- | --- |
| Google AI 功能可见性 | [Google Search Console](https://search.google.com/search-console/about) | 第一方；截至本次审查，生成式 AI 报告仍为有限开放。 |
| Microsoft AI 引用 | [Bing Webmaster Tools](https://www.bing.com/webmasters/about) | 第一方 AI Performance public preview。 |
| 开源、自托管监测 | [GetCito](https://github.com/ai-search-guru/getcito-worlds-first-open-source-aio-aeo-or-geo-tool) | 部署前检查许可证、供应商费用、方法和安全性。 |
| 多引擎企业监测 | Profound、Semrush、Ahrefs、BrightEdge、seoClarity | 比较 prompt 方法、地区覆盖、原始证据、导出和保存政策。 |
| 中型团队监测 | Peec AI、Otterly.AI、Scrunch AI、LLMrefs、Rankscale | 根据实际市场确认引擎支持和 prompt 上限。 |
| 技术发现 | Search Console、Bing Webmaster Tools、IndexNow、爬虫日志 | 购买可见性软件前，先确认抓取和索引资格。 |

本项目不为厂商排名，也不接受付费收录。完整内容请参阅[工具目录与评估清单](docs/tools.md)。

## 实践基线

1. 确保重要页面可抓取、可索引、有内部链接、canonical 正确、具备良好使用体验，而且主要内容以文本呈现。
2. 发布原创信息：第一手经验、原始数据、清晰方法、署名作者和更新日期。
3. 让主张易于核查，提供来源链接、定义、表格、示例和必要背景。
4. 统一网站、社交资料、产品 feed、知识库和可信第三方中的实体信息。
5. Schema 必须与可见内容一致；绝不使用结构化数据捏造事实。
6. 分别衡量各个引擎，使用固定 prompt 集合、重复运行、保存原始回答，并关联业务结果。
7. 虚假提及、虚假评论、未披露推广和社区刷屏属于滥用，不是 GEO。

[实践手册](docs/playbook.md)会把这些基线转化为 30／60／90 天计划。

## 证据政策

每项投稿都应标注其证据类别：

- **官方** — 平台、标准组织、监管机构或产品所有者。
- **同行评审** — 已发表的学术研究，附会议或期刊及日期。
- **预印本** — 尚未经过同行评审的研究。
- **独立研究** — 方法可复现且样本信息已披露。
- **厂商报告** — 可能有用，但存在商业利益。
- **社区讨论** — 从业经验、假设或争论。

热门不等于证据。热门资源仍可能误导；官方声明也可能仅适用于单个平台。我们同时保留来源及其适用范围。

## 社区

- 提交资源前请阅读[贡献指南](CONTRIBUTING.md)。
- 使用资源建议 Issue 表单提出新增与修正。
- 阅读[治理文档](GOVERNANCE.md)，了解维护者职责与透明决策规则。
- 遵守[行为准则](CODE_OF_CONDUCT.md)，安全问题请按照[安全政策](SECURITY.md)报告。
- 欢迎相关商业工具，但必须披露关系并采用中立描述。本项目不接受付费收录。

## 许可证

为了最大程度方便重用，本整理依据 [CC0 1.0 Universal](LICENSE) 贡献给公共领域。外部链接内容仍保留其原始版权与许可证。
