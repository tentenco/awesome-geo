# Awesome GEO, AEO 및 AI 검색

[![Awesome](https://awesome.re/badge.svg)](https://awesome.re)
[![CC0 1.0](https://img.shields.io/badge/license-CC0--1.0-blue.svg)](LICENSE)
[![Contributions welcome](https://img.shields.io/badge/contributions-welcome-brightgreen.svg)](CONTRIBUTING.md)

> 생성 엔진 최적화(GEO), 답변 엔진 최적화(AEO), AI 검색 가시성 및 오픈 웹을 위한 커뮤니티 중심의 근거 기반 가이드입니다.

[English](README.md) · [繁體中文](README-zh-TW.md) · [简体中文](README-zh-CN.md) · [日本語](README-ja.md) · [العربية](README-ar.md)

최종 검토: **2026-08-10** · [2026년에 달라진 점](docs/2026-landscape.md)

## 시작하기

- **처음 접하시나요?** [실무 플레이북](docs/playbook.md)을 읽어보세요.
- **1차 출처가 필요한가요?** [공식 가이드](docs/official-guidance.md)를 확인하세요.
- **소프트웨어를 선택 중인가요?** [도구와 생태계](docs/tools.md)를 비교하세요.
- **보고 체계를 설계 중인가요?** [측정 프레임워크](docs/measurement.md)를 활용하세요.
- **연구 근거를 추적하고 싶나요?** [연구 및 데이터셋](docs/research.md)을 살펴보세요.
- **실무자 논쟁을 보고 싶나요?** [Reddit의 2026년 주요 토론](docs/reddit-2026.md)을 확인하세요.

## 용어 정의

업계에는 아직 안정된 단일 분류 체계가 없습니다. 이 프로젝트는 다음과 같은 실무 정의를 사용합니다.

| 용어 | 실무 정의 | 주요 성과 |
| --- | --- | --- |
| **GEO** | 생성된 답변에서 출처나 개체가 검색, 사용, 표현 또는 인용될 가능성을 개선하는 활동. | 인용, 언급, 정확한 표현 |
| **AEO** | 답변 상자, 어시스턴트, 생성형 검색처럼 직접 답변을 제공하는 시스템이 콘텐츠를 유용하게 활용하도록 만드는 활동. | 답변 포함 및 품질 |
| **AI 검색 가시성** | AI Overviews, AI Mode, ChatGPT, Copilot, Perplexity, Claude, Gemini 등을 아우르는 측정 분야. | 가시성, 점유율, 감성, 유입 |
| **SEO** | 검색 엔진에서 발견, 색인, 표시 및 성과를 개선하는 활동. | 검색 가시성과 양질의 트래픽 |

이러한 실무는 서로 겹칩니다. Google은 기존 SEO 기본 원칙이 AI Overviews와 AI Mode에도 적용되며 특별한 추가 기술 요건이 없다고 명시합니다. 다른 답변 엔진은 서로 다른 크롤러, 색인, 인터페이스, 보고 체계를 사용하므로 운영 세부 사항을 별도로 평가해야 합니다.

## 2026: 과장이 아닌 중요한 신호

2026년에 처음 공개된 가장 중요한 변화는 다음과 같습니다.

- **Google은 2026-05-15에 생성형 AI 검색 전용 가이드를 발표했습니다.** Query fan-out, 비범용 콘텐츠, 멀티미디어와 지역 정보, AI agents, GEO/AEO 오해를 다룹니다. [공식 가이드](https://developers.google.com/search/docs/appearance/ai-features) · [발표](https://developers.google.com/search/blog/2026/05/a-new-resource-for-optimizing)
- **Google Search Console은 2026-06-03에 Generative AI performance reports를 도입했습니다.** 초기에는 일부 사이트에 제공되며 생성형 AI 기능의 노출, 페이지, 국가, 기기, 시간 추이를 보여줍니다. [발표](https://developers.google.com/search/blog/2026/06/gen-ai-performance-reports)
- **Bing Webmaster Tools는 2026-02-10에 AI Performance public preview를 출시했습니다.** Microsoft AI 경험에서 총 인용, 인용된 페이지, grounding queries 및 추이를 제공합니다. [발표](https://blogs.bing.com/webmaster/February-2026/Introducing-AI-Performance-in-Bing-Webmaster-Tools-Public-Preview)
- **측정 자체가 연구 문제가 되었습니다.** AI 답변은 확률적으로 달라지므로 한 번의 프롬프트 캡처가 아니라 반복 실행과 분포로 측정해야 한다는 연구가 나왔습니다. [Don't Measure Once](https://arxiv.org/abs/2604.07585) · [2023–2026 비판적 조사](https://arxiv.org/abs/2607.14035)
- **제품 범주는 모니터링에서 워크플로와 agents로 이동했습니다.** Amplitude AI Visibility 확장, Onclusive GEO Analytics, Jasper GEO Agent 등이 있습니다. 이는 공급업체의 주장이지 독립적인 효과 증명은 아닙니다. [생태계 상세 정보](docs/tools.md#verified-2026-launches-and-major-updates)

전체 일정과 출처는 [2026년 환경 및 변경 기록](docs/2026-landscape.md)을 참고하세요.

## 공식 플랫폼 자료

### Google 검색

- [AI 기능과 웹사이트](https://developers.google.com/search/docs/appearance/ai-features) — 자격 요건, query fan-out, 제어, 측정 및 오해 바로잡기.
- [검색 문서 업데이트](https://developers.google.com/search/updates) — 날짜가 표시된 공식 변경 기록과 RSS.
- [Google 검색 필수 요소](https://developers.google.com/search/docs/essentials) — 기술 요건, 스팸 정책, 핵심 모범 사례.
- [유용하고 신뢰할 수 있는 사람 중심 콘텐츠](https://developers.google.com/search/docs/fundamentals/creating-helpful-content) — Google의 콘텐츠 품질 지침.
- [구조화된 데이터 소개](https://developers.google.com/search/docs/appearance/structured-data/intro-structured-data) — 표시 콘텐츠와 일치하는 지원 마크업을 사용하세요. 구조화된 데이터는 GEO 성과를 보장하지 않습니다.
- [Google 크롤러 및 가져오기 도구](https://developers.google.com/search/docs/crawling-indexing/overview-google-crawlers) — `Google-Extended`를 포함한 user agent와 크롤 제어.

### Microsoft와 Bing

- [Bing Webmaster Tools AI Performance](https://blogs.bing.com/webmaster/February-2026/Introducing-AI-Performance-in-Bing-Webmaster-Tools-Public-Preview) — 2026년에 도입된 퍼스트파티 인용 보고서.
- [색인의 역할 변화](https://blogs.bing.com/search/May-2026/Evolving-role-of-the-index-From-ranking-pages-to-supporting-answers) — 페이지 순위와 답변 grounding의 차이에 대한 Microsoft의 설명.
- [IndexNow](https://www.indexnow.org/) — 참여 검색 엔진에 URL 변경을 알리는 개방형 프로토콜.
- [Bing Webmaster Guidelines](https://www.bing.com/webmasters/help/webmaster-guidelines-30fba23a) — 크롤링, 색인 및 품질에 관한 핵심 지침.

### OpenAI 및 기타 답변 엔진

- [OpenAI 게시자 FAQ](https://help.openai.com/en/articles/12627856) — `OAI-SearchBot`, `noindex`, 포함, 인용 및 추천 트래픽 추적.
- [OpenAI 크롤러 문서](https://platform.openai.com/docs/bots) — 검색, 사용자 요청 및 학습 관련 user agent 구분.
- [Anthropic 웹 크롤러](https://support.anthropic.com/en/articles/8896518-does-anthropic-crawl-data-from-the-web-and-how-can-site-owners-block-the-crawler) — Anthropic의 공식 크롤 제어.
- [Perplexity 크롤러 문서](https://docs.perplexity.ai/guides/bots) — 공식 user agent 및 robots 지침.

크롤러 제어 표와 플랫폼 간에 일반화할 수 없는 주장에 대해서는 [공식 가이드](docs/official-guidance.md)를 참고하세요.

## 핵심 연구

- [GEO: Generative Engine Optimization](https://arxiv.org/abs/2311.09735) — KDD 2024의 기초 논문으로 GEO-Bench와 가시성 개입 실험을 소개합니다.
- [GEO 프로젝트와 벤치마크](https://generative-engines.com/GEO/) — 프로젝트 사이트, 데이터, 코드 및 벤치마크 배경.
- [Don't Measure Once](https://arxiv.org/abs/2604.07585) — 확률적 출력에서 반복 측정을 다룬 2026년 프리프린트.
- [생성 엔진 가시성에 대한 비판적 조사(2023–2026)](https://arxiv.org/abs/2607.14035) — 용어, 지표, 근거, 위험, 재현성을 검토한 2026년 프리프린트.
- [AgenticGEO](https://arxiv.org/abs/2603.20213) — Agentic 최적화 시스템을 제안한 2026년 프리프린트.
- [Pinterest acquisition growth를 위한 GEO 프레임워크](https://arxiv.org/abs/2602.02961) — 2026년 VLM／agent 응용 연구로, 특정 영역의 결과를 신중하게 해석해야 합니다.

프리프린트는 명확히 표시하며 플랫폼의 보장으로 간주해서는 안 됩니다. 자세한 내용은 [연구 및 데이터셋](docs/research.md)을 참고하세요.

## 도구 지도

| 필요 사항 | 시작 도구 | 참고 사항 |
| --- | --- | --- |
| Google AI 기능 가시성 | [Google Search Console](https://search.google.com/search-console/about) | 퍼스트파티. 검토 시점에 생성형 AI 보고서는 제한적으로 제공됩니다. |
| Microsoft AI 인용 | [Bing Webmaster Tools](https://www.bing.com/webmasters/about) | 퍼스트파티 AI Performance public preview. |
| 오픈소스 자체 호스팅 모니터링 | [GetCito](https://github.com/ai-search-guru/getcito-worlds-first-open-source-aio-aeo-or-geo-tool) | 배포 전 라이선스, API 비용, 방법론, 보안을 검토하세요. |
| 다중 엔진 기업 모니터링 | Profound, Semrush, Ahrefs, BrightEdge, seoClarity | 프롬프트 방법, 지역 범위, 원시 증거, 내보내기, 보존 정책을 비교하세요. |
| 중견 팀 모니터링 | Peec AI, Otterly.AI, Scrunch AI, LLMrefs, Rankscale | 실제 시장에 맞는 엔진과 프롬프트 한도를 확인하세요. |
| 기술적 발견 | Search Console, Bing Webmaster Tools, IndexNow, 크롤러 로그 | 가시성 소프트웨어를 구매하기 전에 크롤링과 색인 자격을 확립하세요. |

이 프로젝트는 공급업체 순위를 매기거나 유료 게재를 받지 않습니다. [도구 목록 및 평가 체크리스트](docs/tools.md)를 참고하세요.

## 실무 기준선

1. 중요 페이지가 크롤링 및 색인 가능하고 내부 링크, canonical, 사용 경험, 텍스트 형태의 핵심 정보를 갖추도록 합니다.
2. 직접 경험, 원본 데이터, 명확한 방법, 저자명, 업데이트 날짜가 있는 독창적인 정보를 게시합니다.
3. 출처 링크, 정의, 표, 예시 및 필요한 맥락을 제공하여 주장을 검증하기 쉽게 만듭니다.
4. 사이트, 프로필, 제품 feed, 지식 베이스 및 신뢰할 수 있는 제3자에서 개체 정보를 일관되게 유지합니다.
5. Schema는 표시 콘텐츠와 일치해야 하며 구조화된 데이터로 사실을 만들어서는 안 됩니다.
6. 엔진별로 고정된 프롬프트 세트, 반복 실행, 원시 답변 저장, 비즈니스 성과 연결을 수행합니다.
7. 조작된 언급, 가짜 리뷰, 미공개 홍보, 커뮤니티 스팸은 GEO가 아니라 남용입니다.

[실무 플레이북](docs/playbook.md)은 이 기준선을 30／60／90일 프로그램으로 전환합니다.

## 근거 정책

모든 제출물은 다음 근거 유형을 명시해야 합니다.

- **공식** — 플랫폼, 표준 기구, 규제 기관 또는 제품 소유자.
- **동료 심사** — 발표 장소와 날짜가 있는 출판된 학술 연구.
- **프리프린트** — 동료 심사를 통해 확립되지 않은 연구.
- **독립 연구** — 재현 가능한 방법과 공개된 표본.
- **공급업체 보고서** — 유용할 수 있지만 상업적 이해관계가 있는 자료.
- **커뮤니티 토론** — 실무 경험, 가설 또는 논쟁.

인기는 증거가 아닙니다. 인기 있는 자료도 오해를 불러올 수 있고 공식 발표도 특정 플랫폼에만 적용될 수 있습니다. 우리는 출처와 적용 범위를 모두 보존합니다.

## 커뮤니티

- 리소스를 제안하기 전에 [기여 가이드](CONTRIBUTING.md)를 읽어주세요.
- 추가 및 수정에는 리소스 제안 Issue 양식을 사용하세요.
- 유지관리자의 책임과 투명한 결정 규칙은 [거버넌스](GOVERNANCE.md)를 참고하세요.
- [행동 강령](CODE_OF_CONDUCT.md)을 준수하고 보안 문제는 [보안 정책](SECURITY.md)에 따라 신고하세요.
- 관련성이 있고 관계를 공개하며 중립적으로 설명한 상용 도구도 환영합니다. 유료 게재는 허용하지 않습니다.

## 라이선스

최대한 자유롭게 재사용할 수 있도록 이 큐레이션은 [CC0 1.0 Universal](LICENSE)에 따라 퍼블릭 도메인에 기여됩니다. 링크된 자료에는 원래의 저작권과 라이선스가 계속 적용됩니다.
