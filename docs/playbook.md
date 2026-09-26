# Practical GEO/AEO playbook

Last reviewed: 2026-08-10

This playbook focuses on durable work that improves both human usefulness and machine retrieval. It does not promise rankings or citations.

## Phase 1 — establish the baseline (days 1–30)

### Technical discovery

- Inventory canonical URLs, index status, sitemaps, internal links, render paths, status codes, and duplicate pages.
- Verify that important facts exist in accessible text, not only images, video, client-only widgets, or PDFs.
- Audit robots and CDN/WAF rules against each desired crawler purpose.
- Connect Google Search Console and Bing Webmaster Tools; enable IndexNow where it fits the stack.
- Segment measurable AI referrals in analytics, while documenting referrer limitations.

### Entity and fact inventory

Create a versioned source of truth for names, descriptions, people, locations, products, pricing, availability, policies, certifications, and dates. Assign an owner and update cadence. Resolve contradictions across the website, feeds, directories, help center, social profiles, and major third-party references.

### Prompt and answer baseline

Build the first prompt panel from customer interviews, sales/support logs, site search, Search Console, and category research. Run repeated tests following the [measurement framework](measurement.md), and record incorrect facts as well as missing mentions.

## Phase 2 — build answer-worthy assets (days 31–60)

Prioritize content that adds information to the web:

- primary research with sample, method, field dates, and downloadable data;
- expert explanations with named authors and relevant credentials;
- comparison pages with declared criteria, tested dates, and limitations;
- product/service documentation with exact capabilities and constraints;
- original tools, calculators, templates, datasets, examples, and benchmarks;
- local information with current addresses, hours, service areas, and policies;
- visual evidence supported by captions, transcripts, and relevant surrounding text.

For every important page, ask:

1. What unique claim or evidence exists here?
2. Can a reader verify each consequential assertion?
3. Is the main answer clear without removing necessary nuance?
4. Are authorship, dates, conflicts, corrections, and limitations visible?
5. Does structured data truthfully match the page?

## Phase 3 — earn trustworthy corroboration (days 61–90)

- Publish material worth referencing, then conduct transparent PR and expert outreach.
- Participate in relevant communities by answering questions fully and disclosing affiliations.
- Correct inaccurate directory, profile, marketplace, and knowledge-base data.
- Invite independent reviews without scripting sentiment or hiding incentives.
- Make original data easy to cite with stable URLs, definitions, tables, and downloadable files.
- Consolidate duplicate or outdated pages so systems encounter one current source of truth.

Never automate fake questions, fake reviews, undisclosed endorsements, link schemes, or astroturfed Reddit discussions. These violate community trust and may violate platform policies.

## Continuous loop

```text
Observe → classify the gap → improve the source of truth → publish/distribute
   ↑                                                        ↓
report outcomes ← repeat measurement ← wait for recrawl/retrieval
```

Classify a gap before acting:

- **Not eligible:** crawl, index, preview, or policy problem.
- **Not retrieved:** intent mismatch, weak evidence, stale or duplicative source.
- **Retrieved but not cited:** attribution/interface issue or stronger competing source.
- **Mentioned incorrectly:** entity ambiguity or inconsistent facts.
- **Visible but no outcome:** wrong prompt intent, weak proposition, or attribution gap.

## Content review checklist

- [ ] One clear purpose and intended audience
- [ ] Original contribution beyond generic synthesis
- [ ] Factual claims linked to primary sources where possible
- [ ] Method and limitations for statistics or tests
- [ ] Named author/editor and reviewed date
- [ ] Descriptive headings and accessible tables
- [ ] Stable canonical URL and meaningful internal links
- [ ] Structured data matches visible content
- [ ] Corrections and update history are visible
- [ ] No hidden machine-only content or manufactured consensus

## What to automate

Good candidates: broken-link checks, crawl monitoring, schema validation, URL inventories, prompt scheduling, evidence capture, diffs, and anomaly alerts.

Keep humans responsible for: source judgment, factual verification, community participation, conflict disclosure, editorial quality, high-stakes accuracy, and decisions that affect people.

