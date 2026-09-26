# Awesome GEO、AEO 與 AI 搜尋

[![Awesome](https://awesome.re/badge.svg)](https://awesome.re)
[![CC0 1.0](https://img.shields.io/badge/license-CC0--1.0-blue.svg)](LICENSE)
[![歡迎貢獻](https://img.shields.io/badge/contributions-welcome-brightgreen.svg)](CONTRIBUTING.md)

> 由社群共同維護、重視證據的生成式引擎優化（GEO）、答案引擎優化（AEO）、AI 搜尋能見度與開放網路指南。

[English](README.md) · [简体中文](README-zh-CN.md) · [日本語](README-ja.md) · [한국어](README-ko.md) · [العربية](README-ar.md)

最後審查：**2026-08-10** · [2026 年有哪些變化](docs/2026-landscape.md)

## 從這裡開始

- **剛接觸這個領域？**閱讀[實務操作手冊](docs/playbook.md)。
- **需要第一手來源？**查閱[官方指南](docs/official-guidance.md)。
- **正在選擇軟體？**比較[工具與生態系](docs/tools.md)。
- **正在設計報表？**使用[衡量框架](docs/measurement.md)。
- **想追蹤研究證據？**瀏覽[研究與資料集](docs/research.md)。
- **想了解從業者爭論？**查看 [Reddit 2026 熱門討論](docs/reddit-2026.md)。

## 這些名詞代表什麼

業界尚未採用統一且穩定的分類方式。本專案使用以下工作定義：

| 名詞 | 工作定義 | 主要成果 |
| --- | --- | --- |
| **GEO** | 改善來源或實體在生成式回答中被檢索、使用、呈現或引用的機會。 | 引用、提及、正確呈現 |
| **AEO** | 讓內容適合提供直接答案的系統使用，包括答案框、助理與生成式搜尋。 | 答案收錄與答案品質 |
| **AI 搜尋能見度** | 橫跨 AI Overviews、AI Mode、ChatGPT、Copilot、Perplexity、Claude、Gemini 等產品的整體衡量領域。 | 能見度、聲量占比、情緒、導流 |
| **SEO** | 改善搜尋引擎中的探索、索引、呈現與成效。 | 搜尋能見度與有效流量 |

這些實務高度重疊。Google 明確表示，既有 SEO 基礎仍適用於 AI Overviews 與 AI Mode，而且不需要額外的特殊技術條件。其他答案引擎使用不同的 crawler、索引、介面與報表，因此必須分別評估其操作細節。

## 2026：訊號，而不是炒作

以下是 2026 年首次出現、影響最重大的變化：

- **Google 於 2026-05-15 發布生成式 AI 搜尋專屬指南。**內容涵蓋 query fan-out、非同質化內容、多媒體與在地資訊、AI agents，以及 GEO/AEO 迷思。[官方指南](https://developers.google.com/search/docs/appearance/ai-features) · [公告](https://developers.google.com/search/blog/2026/05/a-new-resource-for-optimizing)
- **Google Search Console 於 2026-06-03 推出 Generative AI performance reports。**初期僅開放部分網站，可查看生成式 AI 功能的曝光、頁面、國家、裝置與時間趨勢。[公告](https://developers.google.com/search/blog/2026/06/gen-ai-performance-reports)
- **Bing Webmaster Tools 於 2026-02-10 推出 AI Performance public preview。**包含 Microsoft AI 體驗中的總引用次數、被引用頁面、grounding queries 與趨勢。[公告](https://blogs.bing.com/webmaster/February-2026/Introducing-AI-Performance-in-Bing-Webmaster-Tools-Public-Preview)
- **衡量本身成為研究問題。**新研究主張，由於 AI 回答帶有機率與隨機性，必須重複測量並觀察分布，不能只看單次 prompt 截圖。[Don't Measure Once](https://arxiv.org/abs/2604.07585) · [2023–2026 批判性綜述](https://arxiv.org/abs/2607.14035)
- **產品類別從監測走向工作流與 agents。**Amplitude 擴充 AI Visibility、Onclusive 推出 GEO Analytics、Jasper 推出 GEO Agent。這些是廠商聲明，不是獨立的成效證明。[生態系詳情](docs/tools.md#verified-2026-launches-and-major-updates)

完整時間軸與來源說明請見[2026 年度趨勢與變更記錄](docs/2026-landscape.md)。

## 官方平台資源

### Google 搜尋

- [AI 功能與你的網站](https://developers.google.com/search/docs/appearance/ai-features) — 收錄資格、query fan-out、控制方式、衡量與迷思破解。
- [搜尋文件更新記錄](https://developers.google.com/search/updates) — 附日期的官方變更記錄，頁面亦提供 RSS。
- [Google 搜尋基礎指南](https://developers.google.com/search/docs/essentials) — 技術要求、垃圾內容政策與主要最佳實務。
- [建立實用、可靠、以人為本的內容](https://developers.google.com/search/docs/fundamentals/creating-helpful-content) — Google 的內容品質指南。
- [結構化資料簡介](https://developers.google.com/search/docs/appearance/structured-data/intro-structured-data) — 使用與可見內容相符的支援標記；結構化資料不是保證 GEO 成效的捷徑。
- [Google crawler 與 fetcher](https://developers.google.com/search/docs/crawling-indexing/overview-google-crawlers) — User agent 與抓取控制，包含 `Google-Extended` 文件連結。

### Microsoft 與 Bing

- [Bing Webmaster Tools AI Performance](https://blogs.bing.com/webmaster/February-2026/Introducing-AI-Performance-in-Bing-Webmaster-Tools-Public-Preview) — 2026 年推出的第一方引用報表。
- [索引角色的演變](https://blogs.bing.com/search/May-2026/Evolving-role-of-the-index-From-ranking-pages-to-supporting-answers) — Microsoft 對網頁排名與回答 grounding 的區分。
- [IndexNow](https://www.indexnow.org/) — 通知參與搜尋引擎網址變更的開放協定。
- [Bing Webmaster Guidelines](https://www.bing.com/webmasters/help/webmaster-guidelines-30fba23a) — 抓取、索引與品質的核心指南。

### OpenAI 與其他答案引擎

- [OpenAI 發布者 FAQ](https://help.openai.com/en/articles/12627856) — `OAI-SearchBot`、`noindex`、收錄、引用與導流追蹤。
- [OpenAI crawler 文件](https://platform.openai.com/docs/bots) — 區分搜尋、使用者觸發與訓練相關的 user agents。
- [Anthropic 網路 crawler](https://support.anthropic.com/en/articles/8896518-does-anthropic-crawl-data-from-the-web-and-how-can-site-owners-block-the-crawler) — Anthropic 官方抓取控制。
- [Perplexity crawler 文件](https://docs.perplexity.ai/guides/bots) — 官方 user agent 與 robots 指南。

Crawler 控制矩陣及不可跨平台套用的說法，請見[官方指南](docs/official-guidance.md)。

## 核心研究

- [GEO: Generative Engine Optimization](https://arxiv.org/abs/2311.09735) — 奠基論文，發表於 KDD 2024；提出 GEO-Bench 與能見度干預實驗。
- [GEO 專案與 benchmark](https://generative-engines.com/GEO/) — 專案網站、資料、程式碼與 benchmark 背景。
- [Don't Measure Once](https://arxiv.org/abs/2604.07585) — 2026 預印本，探討隨機輸出環境下的重複測量。
- [生成式引擎能見度批判性綜述（2023–2026）](https://arxiv.org/abs/2607.14035) — 2026 預印本，回顧名詞、指標、證據、風險與再現性。
- [AgenticGEO](https://arxiv.org/abs/2603.20213) — 2026 預印本，提出 agentic 優化系統。
- [Pinterest acquisition growth 的 GEO 框架](https://arxiv.org/abs/2602.02961) — 2026 的 VLM／agent 應用框架；應謹慎看待其特定領域結果。

預印本均有明確標記，不應被視為平台保證。更多內容請見[研究與資料集](docs/research.md)。

## 工具地圖

| 需求 | 建議起點 | 注意事項 |
| --- | --- | --- |
| Google AI 功能能見度 | [Google Search Console](https://search.google.com/search-console/about) | 第一方；截至本次審查，生成式 AI 報表仍有限量開放。 |
| Microsoft AI 引用 | [Bing Webmaster Tools](https://www.bing.com/webmasters/about) | 第一方 AI Performance public preview。 |
| 開源、自行託管的監測 | [GetCito](https://github.com/ai-search-guru/getcito-worlds-first-open-source-aio-aeo-or-geo-tool) | 部署前檢查授權、供應商費用、方法與安全性。 |
| 多引擎企業監測 | Profound、Semrush、Ahrefs、BrightEdge、seoClarity | 比較 prompt 方法、地區覆蓋、原始證據、匯出與保存政策。 |
| 中型團隊監測 | Peec AI、Otterly.AI、Scrunch AI、LLMrefs、Rankscale | 依實際市場確認引擎支援及 prompt 上限。 |
| 技術探索 | Search Console、Bing Webmaster Tools、IndexNow、crawler logs | 購買能見度軟體前，先確認抓取與索引資格。 |

本專案不替廠商排名，也不接受付費刊登。完整內容請見[工具目錄與評估清單](docs/tools.md)。

## 實務基準

1. 確保重要頁面可抓取、可索引、有內部連結、canonical 正確、具備足夠使用體驗，而且主要內容以文字呈現。
2. 發布原創資訊：第一手經驗、原始資料、清楚方法、具名作者與更新日期。
3. 讓主張容易查證，提供來源連結、定義、表格、例子與必要脈絡。
4. 統一網站、社群檔案、產品 feed、知識庫及可信第三方上的實體資料。
5. Schema 必須符合可見內容；絕不使用結構化資料捏造事實。
6. 各引擎分別衡量，使用固定 prompt 集合、重複執行、保存原始回答，並連結到商業成果。
7. 假提及、假評論、未揭露推廣與社群洗版屬於濫用，不是 GEO。

[實務操作手冊](docs/playbook.md)會把這些基準轉換成 30／60／90 天計畫。

## 證據政策

每項投稿都應標示其證據類別：

- **官方** — 平台、標準組織、監管機關或產品所有者。
- **同儕審查** — 已發表的學術研究，附場合與日期。
- **預印本** — 尚未完成同儕審查的研究。
- **獨立研究** — 方法可重現且樣本資訊已揭露。
- **廠商報告** — 可能有用，但帶有商業利益。
- **社群討論** — 從業經驗、假設或爭論。

熱門不等於證明。熱門資源仍可能誤導；官方聲明也可能只適用於單一平台。我們會同時保留來源及其適用範圍。

## 社群

- 提交資源前請閱讀[貢獻指南](CONTRIBUTING.md)。
- 使用資源建議 Issue 表單提出新增與修正。
- 閱讀[治理文件](GOVERNANCE.md)，了解維護者責任與透明決策規則。
- 遵守[行為準則](CODE_OF_CONDUCT.md)，安全問題請依照[安全政策](SECURITY.md)回報。
- 歡迎具相關性的商業工具，但必須揭露關係並採中立描述。本專案不接受付費刊登。

## 授權

為了讓資源能被最大程度重用，本整理依 [CC0 1.0 Universal](LICENSE) 貢獻給公眾領域。外部連結內容仍保留其原始著作權與授權。
