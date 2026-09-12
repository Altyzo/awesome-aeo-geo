# Awesome AEO & GEO

A curated list of tools, research, benchmarks, and resources for Answer Engine Optimization (AEO) and Generative Engine Optimization (GEO).

> Maintained by [Altyzo](https://altyzo.com) — self-hosted autonomous AI agents for SEO, AEO, and GEO.

## Why this list exists

The search landscape has fundamentally changed. 68% of US Google searches ended without a click in the first four months of 2026 (SparkToro/Datos, June 2026). AI Overviews reduce the organic click-through rate for the top-ranking page by 58% — from 7.3% to 1.6% on AI Overview keywords (Ahrefs, analysis of 300,000 keywords, Dec 2023 vs Dec 2025). Google AI Mode passed 1 billion monthly users.

The opportunity: AI search visitors convert at roughly 4.4x the rate of traditional organic traffic (Semrush, 2025). Pages cited in AI Overviews earn 35% more organic clicks than non-cited competitors on the same results page.

The problem: only 11% of domains are cited by both ChatGPT and Perplexity. ChatGPT cites only 15% of the pages it retrieves, and the top 10 domains for any topic capture 46% of all citations (SE Ranking, analysis of 129,000 domains). Each AI platform operates on fundamentally different citation logic.

This list collects the tools, research, and standards that define the AEO and GEO category. It is maintained by [Altyzo](https://altyzo.com) and updated as the category evolves. Category funding passed $350M in 2026 — Profound raised $155M, Bluefish $68M, AirOps $55M+, and Semrush was acquired by Adobe for ~$1.9B.

## Table of Contents

1. [Research & Benchmarks](#research--benchmarks)
2. [AI Visibility Tracking](#ai-visibility-tracking)
3. [AEO/GEO Audit Tools](#aeogeo-audit-tools)
4. [Schema & Structured Data](#schema--structured-data)
5. [Content Optimization for AI Search](#content-optimization-for-ai-search)
6. [llms.txt & AI Crawler Policy](#llmstxt--ai-crawler-policy)
7. [Open Source Building Blocks](#open-source-building-blocks)
8. [Guides & Reports](#guides--reports)
9. [Datasets & Benchmarks](#datasets--benchmarks)
10. [Standards & Specifications](#standards--specifications)

## Research & Benchmarks

The academic foundation of GEO and AEO.

- [GEO: Generative Engine Optimization](https://arxiv.org/abs/2311.09735) - Aggarwal et al., KDD 2024. The paper that introduced GEO as a paradigm. Showed content optimization can boost visibility in generative engine responses by up to 40%.
- [GEO-Bench](https://huggingface.co/datasets/GEO-optim/geo-bench) - Large-scale benchmark of 10,000 queries across nine domains for evaluating generative engine visibility. Hosted on Hugging Face.
- [GEO-optim/GEO](https://github.com/GEO-optim/GEO) - Official code and benchmark for the GEO paper. Includes optimization strategies and evaluation metrics.
- [GEO Leaderboard](https://huggingface.co/spaces/GEO-optim/geo-bench) - Live Hugging Face leaderboard for GEO-Bench performance.
- [GEO: Generative Engine Optimization (Project Page)](https://generative-engines.com/GEO/) - Princeton/IIT Delhi project page with visualizations, key highlights, and links to code, dataset, and paper.

## AI Visibility Tracking

Tools that monitor where your brand appears in AI-generated answers across ChatGPT, Perplexity, Google AI Overviews, Claude, and Gemini.

- [Profound](https://www.tryprofound.com) - AEO platform with answer engine insights, prompt volume tracking, and agent analytics. Raised $96M Series C at $1B valuation (Feb 2026).
- [Otterly.ai](https://otterly.ai) - AI Overview citation tracking. Research found 59.8% of AI Overview citations are brand websites, higher than ChatGPT or Perplexity.
- [LLM Pulse](https://llmpulse.ai) - Tracks AI Overview citations and mentions across Google, ChatGPT, Perplexity, Gemini, and AI Mode. From EUR49/mo with unlimited seats.
- [Semrush AI Visibility Toolkit](https://www.semrush.com) - Native add-on for Semrush users, now bundled into Semrush One. Semrush acquired by Adobe for ~$1.9B (Apr 2026).
- [Ahrefs Brand Radar](https://ahrefs.com) - AI brand visibility tracking integrated into Ahrefs. Ahrefs holds 14.83% SEO tool market share with the industry's largest backlink index (35 trillion backlinks).
- [seoClarity ArcAI](https://www.seoclarity.com) - Enterprise AI visibility tracking. Approximately $3,000/mo.
- [Mentionova](https://mentionova.com) - Six-engine AI visibility coverage with Reddit engagement tracking and actionable plays.
- [Peec AI](https://peec.ai) - AI search visibility monitoring across multiple engines.
- [Bluefish](https://bluefish.ai) - AI visibility platform. Raised $68M.
- [AirOps](https://airops.com) - AI-powered content and visibility workflows. Raised $55M+.
- [Writesonic GEO](https://writesonic.com) - GEO content optimization and AI visibility tracking.
- [Gumshoe.AI](https://gumshoe.ai) - AI search citation monitoring.
- [Omnibound](https://www.omnibound.ai) - Free AI search visibility checker plus paid tracking plans.
- [Knowatoa](https://knowatoa.com) - AI search ranking and citation tracking.
- [AthenaHQ](https://athenahq.com) - AI visibility monitoring and reporting.
- [ZipTie](https://ziptie.ai) - AI search visibility tracking.

## AEO/GEO Audit Tools

Tools that check whether your site is readable, crawlable, and citable by AI engines.

- [foglift-scan](https://foglift.io) - MIT-licensed CLI on npm for AI search scoring. The only open-source CLI purpose-built for AI search audit.
- [geo-optimizer-skill](https://github.com/Auriti-Labs/geo-optimizer-skill) - Open-source AEO/GEO audit toolkit. Available as GitHub Action and PyPI package. Audits ChatGPT, Perplexity, Gemini, Claude, and Google AI Overviews citation readiness.
- [Altyzo AEO Audit Checklist](https://github.com/altyzo/aeo-audit-checklist) - Open-source CLI that checks any URL for AEO readiness: schema, FAQ blocks, entity coverage, llms.txt, semantic HTML, heading structure. *(Our own.)*

## Schema & Structured Data

Structured data is the #1 technical requirement for AI citation. These tools generate and validate it.

- [Schema.org](https://schema.org) - The canonical specification for structured data, maintained by Google, Microsoft, Yandex, and Yahoo. AI engines use schema to understand entity relationships and content structure.
- [Google Rich Results Test](https://search.google.com/test/rich-results) - Google's official validator for structured data that qualifies for rich results and AI Overviews.
- [Schema Markup Validator](https://validator.schema.org) - W3C-hosted validator for schema.org markup.
- [Altyzo Schema Markup Generator](https://github.com/altyzo/schema-markup-generator) - TypeScript library and CLI for generating JSON-LD: Article, FAQPage, HowTo, BreadcrumbList, Organization, Product. *(Our own.)*

## Content Optimization for AI Search

Tools that help restructure content for citation-friendly formatting.

- [GEOFlow](https://github.com/yaojingang/GEOFlow) - Open-source GEO content engineering and multi-site distribution platform with AI quality inspection. 3.6K GitHub stars.
- [Writesonic GEO](https://writesonic.com) - GEO content optimization with AI-generated, citation-structured articles.
- [flow](https://github.com/AgriciDaniel/flow) - Evidence-led SEO playbook for the AI-search era. 72 docs, 42 AI prompts, 27 diagrams, 15 sourced 2026 stats. CC BY 4.0.

## llms.txt & AI Crawler Policy

The emerging standard for telling AI crawlers what they can and cannot access.

- [llms.txt](https://llmstxt.org) - The proposed standard for providing context to LLMs. Similar to robots.txt but for AI crawlers.
- [llms.txt Guide (Altyzo)](https://altyzo.com/blog/llms-txt-guide) - Practical guide to implementing llms.txt for AI crawler access control. *(Our own.)*

## Open Source Building Blocks

General-purpose open source tools that power AEO/GEO workflows.

- [LangChain](https://github.com/langchain-ai/langchain) - Framework for building AI workflows, prompt monitoring, and custom visibility trackers.
- [LlamaIndex](https://github.com/run-llama/llama_index) - Data framework for structuring content for AI retrieval and discoverability.
- [Haystack](https://github.com/deepset-ai/haystack) - Retrieval and semantic search framework. Useful for citation analysis in AI systems.
- [Promptfoo](https://github.com/promptfoo/promptfoo) - Test prompts across multiple LLMs and compare AI-generated responses.
- [Ragas](https://github.com/explodinggradients/ragas) - Evaluation framework for AI-generated answers, relevance, and citation quality.
- [Firecrawl](https://github.com/mendableai/firecrawl) - Crawl websites and convert content into LLM-friendly formats. Open source with hosted API.

## Guides & Reports

Analyses, studies, and playbooks that define the AEO/GEO category.

- [GEO, AEO, and SEO in 2026: The enterprise guide to AI visibility](https://writer.com/blog/geo-aeo-optimization/) - Writer.com. Comprehensive enterprise guide covering share of model, silent shortlists, and the 25% search volume decline predicted by Gartner.
- [Best 22 AEO Tools for Answer Engine Optimization in 2026](https://www.omnibound.ai/blog/best-aeo-tools-for-answer-engine-optimization) - Omnibound. Scored evaluation of 22 AEO platforms against five weighted criteria.
- [16 Best Google AI Overviews Tracking Tools in 2026](https://llmpulse.ai/blog/best-google-ai-overviews-trackers/) - LLM Pulse. Tested 16 tools that monitor brand visibility inside AI Overviews.
- [Best AI Visibility Tracking Tools (2026)](https://www.integrate.io/blog/best-ai-visibility-tracking-tools) - Integrate.io. Covers 16 tools from $20/mo to $3,000/mo.
- [In 2026, Less Than One-Third of Google Searches Still Send a Click](https://sparktoro.com/blog/in-2026-less-than-one-third-of-google-searches-still-send-a-click/) - SparkToro/Datos, June 2026. The zero-click study defining the AI search era.
- [AI Overviews Reduce Clicks](https://ahrefs.com/blog/ai-overviews-reduce-clicks-update/) - Ahrefs. Analysis of 300,000 keywords comparing Dec 2023 to Dec 2025. CTR for top-ranking page drops 58% on AI Overview keywords.
- [Google AI Overviews Drive Drop in Organic & Paid CTR](https://www.searchengineland.com/google-ai-overviews-drive-drop-organic-paid-ctr-464212/) - Search Engine Land, citing Seer Interactive. 25.1M impressions across 42 orgs. Organic CTR fell 61%.

## Datasets & Benchmarks

Data for training, evaluating, and benchmarking AEO/GEO systems.

- [GEO-Bench](https://huggingface.co/datasets/GEO-optim/geo-bench) - 10,000 queries across nine domains with relevant web sources. The standard benchmark for generative engine visibility.
- [GEO Leaderboard](https://huggingface.co/spaces/GEO-optim/geo-bench) - Live Hugging Face leaderboard for GEO-Bench performance.

## Standards & Specifications

The specs that govern how AI engines read and cite your content.

- [Schema.org](https://schema.org) - Structured data specification used by Google, Microsoft, Yandex, and AI engines for entity understanding.
- [llms.txt](https://llmstxt.org) - Proposed standard for providing context to LLMs and AI crawlers.
- [robots.txt](https://developers.google.com/search/docs/crawling-indexing/robots/robots_txt) - Google's robots.txt specification. Controls crawler access including AI crawlers.
- [JSON-LD](https://json-ld.org/) - JSON-based serialization of linked data. The recommended format for structured data by Google.

## Contributing

Contributions welcome. Open a pull request or an issue with your suggestion.

- Add the link at the bottom of the relevant category
- Check it is not already listed
- Keep descriptions to one line
- No affiliate links

## License

[MIT](./LICENSE)
