# Awesome GEO、AEO、AI Search

[![Awesome](https://awesome.re/badge.svg)](https://awesome.re)
[![CC0 1.0](https://img.shields.io/badge/license-CC0--1.0-blue.svg)](LICENSE)
[![Contributions welcome](https://img.shields.io/badge/contributions-welcome-brightgreen.svg)](CONTRIBUTING.md)

> Generative Engine Optimization（GEO）、Answer Engine Optimization（AEO）、AI 検索の可視性、オープンウェブに関する、コミュニティ主導かつエビデンス重視のガイドです。

[English](README.md) · [繁體中文](README-zh-TW.md) · [简体中文](README-zh-CN.md) · [한국어](README-ko.md) · [العربية](README-ar.md)

最終レビュー：**2026-08-10** · [2026 年の変更点](docs/2026-landscape.md)

## はじめに

- **初めて学ぶ方：**[実践プレイブック](docs/playbook.md)をお読みください。
- **一次情報が必要な方：**[公式ガイダンス](docs/official-guidance.md)をご利用ください。
- **ツールを選定中の方：**[ツールとエコシステム](docs/tools.md)を比較してください。
- **レポートを設計する方：**[測定フレームワーク](docs/measurement.md)をご利用ください。
- **研究を追いたい方：**[研究とデータセット](docs/research.md)をご覧ください。
- **実務者の議論を知りたい方：**[Reddit の 2026 年注目スレッド](docs/reddit-2026.md)をご覧ください。

## 用語の定義

業界にはまだ安定した共通分類がありません。本プロジェクトでは、以下を作業上の定義として用います。

| 用語 | 作業上の定義 | 主な成果 |
| --- | --- | --- |
| **GEO** | 生成された回答において、情報源やエンティティが取得、利用、表現、引用される可能性を改善すること。 | 引用、言及、正確な表現 |
| **AEO** | 回答ボックス、アシスタント、生成 AI 検索など、直接回答を提供するシステムで利用しやすいコンテンツにすること。 | 回答への採用と品質 |
| **AI 検索の可視性** | AI Overviews、AI Mode、ChatGPT、Copilot、Perplexity、Claude、Gemini などを横断する測定領域。 | 可視性、シェア・オブ・ボイス、感情、流入 |
| **SEO** | 検索エンジンにおける発見、インデックス、表示、成果を改善すること。 | 検索可視性と質の高い流入 |

これらの実務領域は重なっています。Google は、既存の SEO の基本が AI Overviews と AI Mode にも適用され、特別な追加技術要件はないと明示しています。他の回答エンジンは異なるクローラー、インデックス、インターフェース、レポートを使用するため、運用上の詳細は個別に評価する必要があります。

## 2026：誇張ではなく重要なシグナル

2026 年に初めて公開された、最も重要な変化は次のとおりです。

- **Google は 2026-05-15 に生成 AI 検索専用ガイドを公開しました。**Query fan-out、独自性の高いコンテンツ、マルチメディア／ローカル情報、AI agents、GEO/AEO の誤解を扱っています。[公式ガイド](https://developers.google.com/search/docs/appearance/ai-features) · [発表](https://developers.google.com/search/blog/2026/05/a-new-resource-for-optimizing)
- **Google Search Console は 2026-06-03 に Generative AI performance reports を導入しました。**当初は一部サイト向けで、生成 AI 機能におけるインプレッション、ページ、国、デバイス、時系列を確認できます。[発表](https://developers.google.com/search/blog/2026/06/gen-ai-performance-reports)
- **Bing Webmaster Tools は 2026-02-10 に AI Performance の public preview を開始しました。**Microsoft の AI 体験における総引用数、引用ページ、grounding queries、推移を確認できます。[発表](https://blogs.bing.com/webmaster/February-2026/Introducing-AI-Performance-in-Bing-Webmaster-Tools-Public-Preview)
- **測定自体が研究課題になりました。**AI の回答は確率的であるため、単一のプロンプトのスクリーンショットではなく、反復測定と分布が必要だとする研究が登場しました。[Don't Measure Once](https://arxiv.org/abs/2604.07585) · [2023–2026 批判的サーベイ](https://arxiv.org/abs/2607.14035)
- **製品カテゴリは監視からワークフローと agents へ進みました。**Amplitude の AI Visibility 拡張、Onclusive GEO Analytics、Jasper GEO Agent などがあります。これらはベンダーの主張であり、独立した効果検証ではありません。[エコシステム詳細](docs/tools.md#verified-2026-launches-and-major-updates)

完全な時系列と出典は、[2026 年のランドスケープと変更履歴](docs/2026-landscape.md)をご覧ください。

## 公式プラットフォーム資料

### Google 検索

- [AI 機能とウェブサイト](https://developers.google.com/search/docs/appearance/ai-features) — 適格性、query fan-out、制御、測定、誤解の解説。
- [検索ドキュメント更新履歴](https://developers.google.com/search/updates) — 日付付きの公式変更履歴。RSS も提供されています。
- [Google 検索の基本事項](https://developers.google.com/search/docs/essentials) — 技術要件、スパムポリシー、主要なベストプラクティス。
- [有用で信頼性の高い、人を第一に考えたコンテンツ](https://developers.google.com/search/docs/fundamentals/creating-helpful-content) — Google のコンテンツ品質ガイド。
- [構造化データの概要](https://developers.google.com/search/docs/appearance/structured-data/intro-structured-data) — 表示内容と一致する対応マークアップを使用してください。構造化データは GEO の近道を保証しません。
- [Google クローラーとフェッチャー](https://developers.google.com/search/docs/crawling-indexing/overview-google-crawlers) — `Google-Extended` を含む user agent とクロール制御。

### Microsoft と Bing

- [Bing Webmaster Tools AI Performance](https://blogs.bing.com/webmaster/February-2026/Introducing-AI-Performance-in-Bing-Webmaster-Tools-Public-Preview) — 2026 年導入のファーストパーティ引用レポート。
- [インデックスの役割の進化](https://blogs.bing.com/search/May-2026/Evolving-role-of-the-index-From-ranking-pages-to-supporting-answers) — ページ順位付けと回答の grounding の違いに関する Microsoft の説明。
- [IndexNow](https://www.indexnow.org/) — 対応検索エンジンへ URL 変更を通知するオープンプロトコル。
- [Bing Webmaster Guidelines](https://www.bing.com/webmasters/help/webmaster-guidelines-30fba23a) — クロール、インデックス、品質に関する基本ガイド。

### OpenAI とその他の回答エンジン

- [OpenAI パブリッシャー FAQ](https://help.openai.com/en/articles/12627856) — `OAI-SearchBot`、`noindex`、掲載、引用、流入測定。
- [OpenAI クローラー文書](https://platform.openai.com/docs/bots) — 検索、ユーザー起点、学習関連の user agent を区別。
- [Anthropic ウェブクローラー](https://support.anthropic.com/en/articles/8896518-does-anthropic-crawl-data-from-the-web-and-how-can-site-owners-block-the-crawler) — Anthropic 公式のクロール制御。
- [Perplexity クローラー文書](https://docs.perplexity.ai/guides/bots) — 公式 user agent と robots ガイド。

クローラー制御の比較とプラットフォーム間で一般化できない主張は、[公式ガイダンス](docs/official-guidance.md)をご覧ください。

## 主要研究

- [GEO: Generative Engine Optimization](https://arxiv.org/abs/2311.09735) — KDD 2024 の基礎論文。GEO-Bench と可視性介入実験を導入。
- [GEO プロジェクトとベンチマーク](https://generative-engines.com/GEO/) — プロジェクトサイト、データ、コード、ベンチマークの背景。
- [Don't Measure Once](https://arxiv.org/abs/2604.07585) — 確率的出力における反復測定を扱う 2026 年のプレプリント。
- [生成エンジンの可視性に関する批判的サーベイ（2023–2026）](https://arxiv.org/abs/2607.14035) — 用語、指標、証拠、リスク、再現性をレビューする 2026 年のプレプリント。
- [AgenticGEO](https://arxiv.org/abs/2603.20213) — Agentic 最適化システムを提案する 2026 年のプレプリント。
- [Pinterest acquisition growth 向け GEO フレームワーク](https://arxiv.org/abs/2602.02961) — 2026 年の VLM／agent 応用。領域固有の結果は慎重に扱ってください。

プレプリントは明示しており、プラットフォームによる保証として扱うべきではありません。詳細は[研究とデータセット](docs/research.md)をご覧ください。

## ツールマップ

| ニーズ | 最初に使うもの | 注意点 |
| --- | --- | --- |
| Google AI 機能の可視性 | [Google Search Console](https://search.google.com/search-console/about) | ファーストパーティ。本レビュー時点で生成 AI レポートは限定提供。 |
| Microsoft AI の引用 | [Bing Webmaster Tools](https://www.bing.com/webmasters/about) | ファーストパーティの AI Performance public preview。 |
| オープンソース／セルフホスト監視 | [GetCito](https://github.com/ai-search-guru/getcito-worlds-first-open-source-aio-aeo-or-geo-tool) | 導入前にライセンス、API 費用、手法、セキュリティを確認。 |
| 複数エンジンの企業監視 | Profound、Semrush、Ahrefs、BrightEdge、seoClarity | プロンプト手法、地域対応、生データ、エクスポート、保持を比較。 |
| 中規模チームの監視 | Peec AI、Otterly.AI、Scrunch AI、LLMrefs、Rankscale | 実際の市場に合うエンジンとプロンプト上限を確認。 |
| 技術的な発見 | Search Console、Bing Webmaster Tools、IndexNow、クローラーログ | 可視性ツールを購入する前にクロール／インデックス適格性を確立。 |

本プロジェクトはベンダーを順位付けせず、有料掲載も受け付けません。[ツール一覧と評価チェックリスト](docs/tools.md)をご覧ください。

## 実践の基準

1. 重要ページをクロール・インデックス可能にし、内部リンク、canonical、利用体験、テキスト形式の主要情報を整えます。
2. 一次体験、独自データ、明確な方法、著者名、更新日を含む独自情報を公開します。
3. 出典リンク、定義、表、例、必要な文脈を付け、主張を検証しやすくします。
4. サイト、プロフィール、商品 feed、ナレッジベース、信頼できる第三者でエンティティ情報を統一します。
5. Schema は表示内容と一致させ、構造化データで事実を作り上げてはいけません。
6. エンジンごとに、固定プロンプト群、反復実行、生の回答保存、事業成果への接続を行います。
7. 人工的な言及、偽レビュー、非開示の宣伝、コミュニティスパムは GEO ではなく不正行為です。

[実践プレイブック](docs/playbook.md)では、この基準を 30／60／90 日の計画に展開しています。

## エビデンスポリシー

各投稿は、次のエビデンス区分を明記してください。

- **公式** — プラットフォーム、標準化団体、規制機関、製品所有者。
- **査読済み** — 掲載先と日付が確認できる学術研究。
- **プレプリント** — 査読で確立されていない研究。
- **独立研究** — 再現可能な方法と開示されたサンプル。
- **ベンダーレポート** — 有用な場合もあるが、商業的利害を持つ資料。
- **コミュニティ議論** — 実務経験、仮説、議論。

人気は証明ではありません。人気資料でも誤解を招く可能性があり、公式見解でも特定プラットフォームに限定される場合があります。本プロジェクトは出典と適用範囲の両方を残します。

## コミュニティ

- リソースを提案する前に[コントリビューションガイド](CONTRIBUTING.md)をお読みください。
- 追加や修正にはリソース提案 Issue フォームをご利用ください。
- メンテナーの責任と透明な意思決定については[ガバナンス](GOVERNANCE.md)をご覧ください。
- [行動規範](CODE_OF_CONDUCT.md)を守り、セキュリティ問題は[セキュリティポリシー](SECURITY.md)に従って報告してください。
- 商用ツールも関連性があり、関係を開示し、中立的に記述されていれば歓迎します。有料掲載は受け付けません。

## ライセンス

最大限の再利用を可能にするため、このキュレーションは [CC0 1.0 Universal](LICENSE) のもとでパブリックドメインに提供されます。リンク先の資料には、それぞれの著作権とライセンスが引き続き適用されます。
