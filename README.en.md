# AfterAI SEO/GEO

**An SEO/GEO skill for overseas Chinese business owners, website developers, and service providers.** Discuss the business in Chinese while optimizing the website in Australian English, another target-market language, or a confirmed English–Chinese bilingual site. It brings search engine optimization (SEO) and generative engine optimization (GEO) into one practical workflow: assess, plan, implement in batches, then review and maintain.

[中文](README.md) · [Usage and stage triggers](afterai-seo-geo/USAGE.md) · [Skill entry](afterai-seo-geo/SKILL.md)

## Built for overseas Chinese operators

**Conversation language, website language, target market, and report language are separate decisions.** A Chinese-speaking owner does not automatically need Chinese pages or offer Chinese-language services. The skill first establishes the actual audience and business facts, then plans keywords and edits for the appropriate language.

| Situation | What the skill does |
|---|---|
| You run an Australian local business site and prefer to work in Chinese, but customers use English | It discusses goals, keywords, and plans in Chinese while writing website titles, descriptions, and copy in Australian English. It does not add Chinese pages by default. |
| Your restaurant or store serves both English- and Chinese-speaking customers | It checks the existing language versions, target areas, Simplified or Traditional Chinese needs, and business facts before planning pages and search questions for each audience. |

The same adaptable process can serve local businesses, ecommerce, B2B, software, content, and personal or organizational websites. These examples do not imply that every industry has been tested.

## Use

Copy the complete [`afterai-seo-geo/`](afterai-seo-geo/) folder into your host's supported skills directory, or ask a file-capable assistant to read its [SKILL.md](afterai-seo-geo/SKILL.md) and referenced files. Keep the folder structure. The installable bundle consists of 13 Markdown files, with no executable, Python, Node, JSON, separate YAML, gstack, superpowers, or paid SEO API dependency. Development documents under `docs/` are not required.

Open a separate workspace for each client and try one of these requests:

> Use AfterAI SEO/GEO to assess this Australian local business website. Please respond to me in Chinese, but keep all website changes in Australian English. Ask about my business goal, priority keywords, and whether I want a full-site audit or a representative sample. Give me scores and a report before discussing edits; do not edit the site yet.

> Use AfterAI SEO/GEO to assess the website in this local project. It has not launched. Check the source and, if available, the local preview. Report what cannot yet be verified online.

> Use AfterAI SEO/GEO to plan improvements for my Shopify store. Review the current storefront and distinguish theme changes from shared product-data changes before proposing edits.

Everyday use needs only **“start,” “continue,” and “monthly check.”** You can also request a narrow task, such as a homepage audit, a GEO plan, or a client report. “Start” begins intake and assessment; it does not authorize website edits. This is one skill; its reference files are loaded as needed, and the assistant maintains records for you. Precise phase requests remain available in the [usage guide](afterai-seo-geo/USAGE.md). Reference instructions are Chinese-first; output follows the configured languages. Compatibility with every host has not been demonstrated.

## How it works

1. **Assess.** Briefly establish the primary outcome, supplied keywords, market, and website languages, then let the operator choose a full-site audit or representative sample unless they already specified the scope. Inspect a public URL, local source, or preview and report evidence-backed SEO, GEO, and visual-experience scores with the actual checked scope and unknowns.
2. **Plan.** After the first report, ask about past website problems, changes already tried and their results, and the desired future site; reuse answers already given. Then expand queries and map them to pages. Decide whether priority pages, navigation, and enquiry or purchase journeys should be kept, improved, reorganized, merged, or expanded. Rank tasks as “most important,” “next,” and “later.” Define a first-launch gate for new sites and releasable batches for live sites. Recommend a knowledge base only when demand and maintenance capacity justify it.
3. **Implement.** Within the agreed scope, check and improve applicable crawl/index settings, URLs and canonicals, titles and descriptions, content, internal links, mobile experience, and Schema/JSON-LD. Then develop evidence-based GEO content and observe AI search responses. For a new site, complete and preview-verify all known, controllable core work in its agreed launch scope before the first public release; for a live site, publish verified batches. Check the actual live environment and outcomes after release.
4. **Review monthly.** Rescore on a comparable basis and keep readiness separate from observed search impressions, enquiries, and AI mentions or citations. Routine checks may sample 2–4 fixed AI questions with explicit scope; a full review retains the full panel. Produce the next concrete task list. If no prior data exists, create a first baseline rather than inventing a trend.

The assistant maintains the plan and evidence. The operator supplies essential business facts, selects or delegates keyword priorities, and reviews concrete changes. Unresolved prices, service areas, promises, or other claims pause only the work that depends on them. Narrow requests and report-only requests do not require the whole workflow.

## Evidence, tools, and limits

- **Live and local websites:** Public pages, local HTML/code, and localhost previews can be assessed when the host can read them. Source-only work cannot establish real indexing, rankings, traffic, or AI recommendations; those outcomes remain unmeasured without live evidence.
- **Code sites and Shopify:** Both have implementation guidance. The Shopify guide is not a connector. Automated changes require an actual connection, field permissions, and specific authorization; an unpublished theme does not isolate shared product data.
- **Scores and GEO observations:** SEO, GEO, and visual scores are diagnostics with evidence and coverage, not a search-platform ranking formula. The default GEO observation set is 10 questions across three surfaces—ChatGPT search, Google AI Overview, and Gemini. Doubao and DeepSeek can be added as separate, optional tests for a relevant Chinese-speaking audience. Manual collection is supported; missing answers are marked unmeasured rather than invented.
- **Cost and outcomes:** The skill requires no paid SEO tool or API. Your existing website, AI products, or host environment may have their own costs. No first-place ranking, AI citation, traffic increase, or enquiry increase is guaranteed. Scheduled monthly runs require real host scheduling support and setup.

Keep each client's profile, plan, reports, and evidence in a verified private location outside the public skill bundle and website deployment output. A client-side `seo-geo/` directory is the default only when it is private; otherwise choose another verified location or deliver records in chat. This project's `.gitignore` excludes its root `output/` and any `seo-geo/` records, but it does not protect separate client repositories. Inspect the actual tracked and staged files before publishing because ignore rules do not remove files already tracked by Git.

The current version is the **0.2.3 public preview**. The update turns spoken customer briefs into polished, accurate website copy for the target audience, while keeping SEO and GEO content natural and useful rather than copying colloquial phrasing or stuffing keywords. A fictional local site was actually edited and a public site was inspected read-only. Live Shopify writes, cross-host operation, and ranking gains remain unverified; see the [evaluation record](docs/evaluation-log.md). The project uses the [MIT License](LICENSE).

See [Contributing](CONTRIBUTING.md) for evidence and privacy requirements. Source links for search and platform rules appear in the relevant reference files and should be checked against current official guidance when used.
