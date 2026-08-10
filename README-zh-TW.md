# Awesome GEO、AEO 與 AI 搜尋

[![Awesome](https://awesome.re/badge.svg)](https://awesome.re)
[![CC0 1.0](https://img.shields.io/badge/license-CC0--1.0-blue.svg)](LICENSE)
[![歡迎貢獻](https://img.shields.io/badge/contributions-welcome-brightgreen.svg)](CONTRIBUTING.md)

> 社群共同維護、重視證據的生成式引擎優化（GEO）、答案引擎優化（AEO）與 AI 搜尋能見度指南。

[English](README.md) · 最後審查：**2026-08-10** · [2026 年度追蹤](docs/2026-landscape.md)

## 從這裡開始

- 想建立實作流程：閱讀[實務 playbook](docs/playbook.md)
- 想查第一手資料：閱讀[官方指南](docs/official-guidance.md)
- 想選擇工具：參考[工具與生態系](docs/tools.md)
- 想建立 KPI：使用[衡量框架](docs/measurement.md)
- 想查研究證據：瀏覽[研究與資料集](docs/research.md)
- 想了解社群爭論：閱讀[Reddit 2026 熱門討論](docs/reddit-2026.md)

## 名詞怎麼用

業界尚未形成單一標準。本專案採用以下工作定義：

| 名詞 | 工作定義 | 主要成果 |
| --- | --- | --- |
| **GEO** | 改善來源或實體在生成式回答中被檢索、使用、正確描述或引用的機會。 | 引用、提及、正確描述 |
| **AEO** | 讓內容適合被直接回答型系統使用，包括精選摘要、助理與生成式搜尋。 | 回答收錄與品質 |
| **AI 搜尋能見度** | 橫跨 AI Overviews、AI Mode、ChatGPT、Copilot、Perplexity、Claude、Gemini 等產品的衡量範疇。 | 能見度、聲量、情緒、導流 |
| **SEO** | 改善搜尋引擎中的探索、索引、呈現與成效。 | 搜尋能見度與有效流量 |

彼此高度重疊。Google 已明確表示：既有 SEO 基礎仍適用於 AI Overviews 與 AI Mode，且沒有額外的技術門檻。其他答案引擎則使用不同 crawler、索引、介面與報表，不能把 Google 的說法直接套用到所有平台。

## 2026 年最重要的新變化

- **Google 於 5 月 15 日發布生成式 AI 搜尋專屬指南。**內容涵蓋 query fan-out、非同質化內容、多媒體／在地／購物資訊、AI agents，以及 GEO/AEO 迷思。[官方指南](https://developers.google.com/search/docs/appearance/ai-features)
- **Google Search Console 於 6 月 3 日開始測試 Generative AI performance reports。**可查看 impressions、頁面、國家、裝置與時間趨勢；目前並非所有網站都有。[官方公告](https://developers.google.com/search/blog/2026/06/gen-ai-performance-reports)
- **Bing Webmaster Tools 於 2 月 10 日推出 AI Performance public preview。**可查看 total citations、cited pages、grounding queries 與趨勢。[官方公告](https://blogs.bing.com/webmaster/February-2026/Introducing-AI-Performance-in-Bing-Webmaster-Tools-Public-Preview)
- **衡量方法成為核心研究問題。**AI 回答有隨機性，單次 prompt 截圖無法代表品牌能見度；應重複執行並用分布與信賴區間報告。[Don't Measure Once](https://arxiv.org/abs/2604.07585)
- **工具從監測走向工作流與 agent。**Amplitude、Onclusive、Jasper 等在 2026 推出或擴充產品，但廠商聲稱不等於獨立成效證據。[完整工具說明](docs/tools.md#verified-2026-launches-and-major-updates)

## Google 官方結論：哪些事不用做

Google 2026 指南針對自己的搜尋產品明確說明：

- 不需要 `llms.txt` 或其他「AI 專用」標記，才能進入 Google 生成式搜尋。
- 不必為 AI 強制把文章切成極小區塊。
- 不必把內容改寫成機器專用版本。
- 不應追求虛假或刻意操弄的品牌提及。

這不代表 `llms.txt` 在其他用途完全沒有價值，也不代表清楚的文章結構不重要；它只表示這些項目不是 Google AI Overviews／AI Mode 的特殊收錄條件。完整脈絡請看[官方指南整理](docs/official-guidance.md)。

## 實作基準

1. 先確保重要頁面可抓取、可索引、有內部連結、canonical 正確、主要內容以文字呈現。
2. 發布真正原創的資訊：第一手經驗、原始資料、清楚方法、具名作者與更新日期。
3. 讓主張可查證：附上來源、定義、表格、例子及必要脈絡。
4. 統一網站、商家資訊、產品 feed、社群檔案與可信第三方上的實體資料。
5. Schema 必須符合頁面可見內容，不得用結構化資料捏造事實。
6. 各引擎分開衡量，固定 prompt 集合、重複測量、保存原始回答，並連結到商業結果。
7. 假評論、假帳號、未揭露推廣與社群洗版屬於濫用，不是 GEO。

## 證據分級

所有新資源應標記為：**官方**、**同儕審查**、**預印本**、**獨立研究**、**廠商報告**或**社群討論**。熱門不等於正確；官方資料也只代表該平台的適用範圍。

## 社群與授權

歡迎依照[貢獻指南](CONTRIBUTING.md)提交新資源、修正失效連結、補充反證或改善翻譯。維護方式詳見[治理文件](GOVERNANCE.md)，參與者需遵守[行為準則](CODE_OF_CONDUCT.md)。

本整理以 [CC0 1.0 Universal](LICENSE) 貢獻給公眾領域，方便社群自由重用。所有外部連結內容仍屬原作者與原授權條款所有。
