# AfterAI SEO/GEO evaluation log

Started 2026-09-22; last updated 2026-10-07. This file records actual development checks, not customer SEO results.

The [0.1.2 pre-release validation](release-validation.md) records the original package checks. Later private site pilots are summarized below; the historical checks and limits remain as dated evidence. The current local package version is 0.2.2; the latest public GitHub release remains 0.2.1. No ranking improvement has been validated. Version 0.1.19 changed only the fictional public example and version labels. Version 0.1.20 strengthens the on-site page and user-journey decision. Version 0.1.21 distinguishes prelaunch completion from incremental live-site releases; version 0.2.0 improves follow-through, evidence handling, monthly sampling and conditional Shopify AI checks. Version 0.2.1 adds an explicit first-audit scope choice and report-led pre-edit interview. Version 0.2.2 moves unknown business and keyword decisions ahead of finalized content, page-structure and GEO recommendations. The scoring rubric is unchanged.

For local 0.2.2, a review of the private Rombe 0.2.0 audit thread found that the operator chose a read-only assessment, then received a report with page changes and phases before primary business and keywords were selected. The published 0.2.1 instructions still allowed that order because the interview was required before a dependent write, while the report template unconditionally requested priorities and phases. The revised instructions now permit scored findings and independent technical fixes immediately, but require business and keyword questions before settling dependent recommendations; report-only users receive the questions as an optional next step. A consistency review also corrected an unconditional phased-route sentence in the report template. Static release checks passed: official skill validator, strict UTF-8 decoding of 20 tracked Markdown files, 84 local links, exactly 13 Markdown-only installable files, and `git diff --check`. No fresh live-site audit or AI-search outcome test was performed for 0.2.2.

For 0.2.1, a read-only baseline instruction test of the released 0.2.0 package used a 120-page multilingual site scenario and an audit-to-implementation continuation. The baseline selected a finite representative sample without asking for a full-site/sampled choice and had no explicit prompt about past website problems, prior SEO/GEO work or desired future site. The revised package passed six read-only forward scenarios: unspecified broad audit asks once; explicit full-site audit batches discovered pages and reports remaining work; narrow homepage audit avoids a duplicate choice; report-only stops; continuation asks report-led history and desired-site questions while reusing answers; narrow technical repair avoids a broad interview. Reviewer-noted wording that called every baseline a “sample” was corrected. Full-site page-level scoring now keeps discovered but unchecked pages in the denominator and discloses denominator changes when more pages are found. This is an instruction-behavior test, not a 120-page crawl or live-site outcome test.

A separate edge check confirmed the intended denominator behavior: if 120 in-scope pages are discovered and 8 checked for a page-level item, 112 remain unmeasured; finding 20 more pages changes the denominator to 140 and prevents a false before/after score claim. This illustration does not mean overall SEO coverage equals 8/120, since other site- and page-level items have separate evidence. The official skill validator passed, all 13 installable files remain Markdown, 20 tracked Markdown files decoded strictly as UTF-8, 84 local file links resolved, and `git diff --check` passed. No live 120-page crawl, customer website change or outcome measurement was performed for 0.2.1.

For 0.2.0, a fictional Australian-English local business site was used as a pre-edit behavior baseline. Its explicitly delegated keyword/page direction and authorized local-edit scope led the existing 0.1.21 instructions to update three existing pages and CSS and add one dedicated service page; the output had HTTP 200 in local preview, nonempty page-specific titles/descriptions, one H1 per page, resolved local links and no invented business claims. Mobile visual quality, production response/indexing, and actual enquiry behavior were not verified. This demonstrated that the prior version already supported real local edits; the revision addresses duplicate-approval ambiguity rather than claiming a new capability. A separate public commerce site was readable through a web reading tool but not through one raw HTTP client (403), so visible content could be sampled while raw HTML metadata, response/crawl controls, rendered layout, GSC and AI-answer outcomes stayed unmeasured. No customer website was changed, and the public site's identity and private notes are omitted from this repository. This is a limited read-only input-path pilot, not a full client audit or ranking test.

An independent read-only forward review of the revised package checked authorized local continuation, theme-only Shopify scope and optional AI product paths, and month-two partial AI sampling against a full prior baseline. All three scenarios remained actionable. A minor ambiguity that could have made any GSC anomaly trigger a full AI question rerun was narrowed to AI-answer trends. Static release checks passed: the official skill validator, strict UTF-8 decoding of 20 tracked Markdown files, 81 local file links, exactly 13 installable Markdown files, and `git diff --check`. These checks do not establish successful Shopify writes or SEO/GEO outcome gains.

For 0.1.21, a read-only scenario review of the previous text confirmed that it allowed a new site to publish a first batch and defer known core-page work to phase 2. After revision, a read-only forward review of the supplied updated rules produced the intended outcomes: complete the agreed new-site launch essentials before first publication, while publishing an urgent fix on an already-live site before optional expansion. That reviewer received excerpts because its local file reads failed; this is a limited behavior probe, not an independent full-package run. A scope loophole identified in the probe was closed by requiring the first-launch scope to cover the promised primary user journey or for the promise to be explicitly changed. The official skill validator passed, 30 Markdown files decoded as UTF-8, 95 local file links resolved, and `git diff --check` passed. No new live site, Shopify write, ranking or AI recommendation measurement was performed.

For 0.1.20, a source-only review of the separate restaurant pilot found that priority-page title, description and H1 already existed, while a generic navigation label and PDF-centered menu content still left an on-site improvement opportunity. A separate read-only forward test used the revised skill on three local pages and proposed a concrete route from homepage to brunch content to booking, while keeping business rules and live outcomes unverified and making no edits. This is evidence that existing metadata does not settle the page or journey decision, not proof that a proposed rewrite will improve rankings or bookings. Static checks passed for 20 tracked Markdown files under strict UTF-8 decoding, 78 local file links, whitespace, and the official skill validator using `PYTHONUTF8=1`. No new live website edit, Shopify write, AI recommendation test or search outcome measurement was performed for this version.

The 0.1.17 release-standard review found and corrected four operational gaps: inherited Google generative-AI inclusion control needs an effective parent-state check and its Discover impact disclosed; monthly AI retesting needs the GEO collection rules; the primary business outcome needs an evidence source for later review; and Shopify search visibility plus display-versus-SEO fields need explicit checks. These corrections form 0.1.18. Three independent read-only reviewers checked logic, package hygiene and eight behavior scenarios; a follow-up review of the revised files found no new contradiction in the monthly GEO retest route, interview/authorization gates, SEO-to-GEO dependencies or scoring rules. Static checks covered 30 public-candidate Markdown files for UTF-8, code fences, local links and anchors; the 13-file Markdown-only bundle copied byte-identically to a path containing spaces and Chinese characters. These checks did not execute the revised package against a live customer property. During that review, an official `quick_validate.py` run was unavailable because the bundled development Python lacked PyYAML; independent format checks were used instead. The MIT License was selected for the public preview on 2026-10-01; live Shopify/cross-host validation remains open.

## Subsequent private pilots — through 2026-09-30

- A restaurant website was audited from local files and a local preview; a limited first batch of local changes was then checked. This did not establish that the same changes were published or improved search rankings.
- A commerce website was inspected read-only on its public pages. One exploratory Google AI response was recorded, but the full planned multi-platform GEO question set was not completed. No Shopify write was tested.
- These pilots exposed reporting gaps addressed in 0.1.10–0.1.12: per-page title/description evidence, clear Schema status, and consistent Schema/JSON-LD terminology. The first implementation batch also showed that a general instruction to begin work could be mistaken for a choice of business goal and keywords; 0.1.14 requires explicit selection or delegation and a per-priority-page metadata decision before related content edits.
- Customer reports and site files remain outside this public skill package. These observations do not validate other industries, live Shopify writes, long-term AI visibility or ranking lift.

The 0.1.14 package check confirmed 13 Markdown files, resolved relative links, valid skill frontmatter, aligned version labels and the new interview/metadata gates. A workflow walkthrough covered three cases: a broad “开始执行修改” with no keyword choice, complete but unreviewed metadata, and explicit delegation of keyword choice. This is a documentation and logic check, not a second live site pilot.

The 0.1.15 structure check again confirmed the 13-file Markdown bundle, relative links, frontmatter and version labels. The instructions now allow assistant-led batch metadata changes after an explicit business/keyword decision and approved local scope, while preserving page-level before/after evidence and escalating only unresolved page facts or claims. This behavior still needs a live pilot.

The 0.1.16 structure check confirmed the same bundle, links and frontmatter, plus the applicable SEO coverage checklist, fact reconciliation and conditional knowledge-base gate. These are documentation checks; a full website run has not yet validated that every host can perform each check.

The 0.1.17 review removed a customer-specific example and duplicated report directions, corrected the knowledge-base reference, and added a read-only GSC generative AI report/control check after confirming the current official documentation. The new GSC path and streamlined report behavior have not yet been exercised end-to-end on a customer property.

## Baseline without new skill

An independent agent received only three fictional scenarios and was forbidden network/filesystem/customer operations. It correctly computed GEO 3/6 recommendations, 2/6 citations and 1/4 first in ordered lists; it did not count the first item of an unordered answer as first rank.

For partial scoring it reported a provisional 50/100 from earned/applicable, 50% coverage and 100% observed pass rate, but did not show the possible interval. This is not an arithmetic error; it demonstrates the need for one explicit display convention. The new worksheet shows observed score, coverage and possible interval separately.

For the Chinese request over a UK English site it supplied a Chinese review draft, correctly reserving UK English for publication. It did not publish. For Shopify it recognized shared scope but interpreted a vague new request as sufficient extension of authorization; missing concrete object/new copy still blocked action. The new guide ties authorization to actual proposed values and shared-live impact. Do not claim the baseline universally failed.

## Structural checks

- Installable bundle: 13 files, all `.md`; filenames English; relative links resolved; no user-machine absolute paths found.
- Bundled skill-creator quick_validate was attempted; unavailable because its developer Python environment lacks PyYAML. No dependency was installed into the product. An independent frontmatter/structure check is performed separately and will be recorded below.
- Independent skill-enabled behavior and full-package review completed; results follow below.

## Skill-enabled fictional scenarios

Six independent, read-only scenarios were evaluated using the package. No customer files or live services were modified.

1. Chinese operator / UK English SaaS: kept communication and publication languages separate; reported observed 100, coverage 50%, interval 50–100 for the arithmetic fixture; correctly rejected dropping the entire industry budget simply because there is no physical store.
2. AI observations: correctly calculated recommendations 3/6, citations 2/6, ordered-list first 1/4 and all-valid first 1/6. Fictional answers remained examples, not evidence.
3. Shopify: recognized that shared product changes require a concrete change proposal beyond unpublished-theme scope.
4. Hybrid store: allocated Local and Commerce 10 points each, two checks per type at 5 each; bilingual queries depended on confirmed website languages.
5. Customer-folder conflict: stopped customer writes until identity and handoff were resolved.
6. Missing scheduler, browser and GSC access: supplied a manual path and marked unavailable evidence unmeasured; did not claim an automation was created.

## Independent package review and fixes

The full 13-file review found two consequential issues, both corrected:

- U03 previously described newly added content, making the baseline ambiguous. Its condition now evaluates current content identically before and after changes.
- AI attempt validity was conflated with planned-question coverage. The guide and report now distinguish P planned questions, Q unique attempted questions, N attempt records and V valid answers. Retries increase N but not Q; untested questions remain in the plan.

An independent follow-up regression was requested but did not execute because the workspace agent credit was exhausted. It is not reported as passed. Local checks below verify the corrected formulas and document consistency; they do not replace an additional independent behavioral run.

## Final local verification

Executed an ephemeral Python standard-library check on 2026-09-22; no script was added to the product. Exit code 0:

- Exactly 13 installable Markdown files, all ASCII English filenames; no machine-specific absolute paths.
- All 28 workspace Markdown files checked: no broken relative links or non-English filenames.
- Independent frontmatter check: correct delimiters, only name/description, valid folder-matching name, nonempty description within 1,024 characters. This is a substitute structural check, not a pass from the unavailable official validator.
- Parsed actual scoring tables: SEO core 80, GEO 100, visual UX 100. The remaining SEO type budget is 20 as documented.
- Partial-score example verified: observed 100, coverage 50%, interval 50–100. Citation and first-place rounding verified.
- Regression assertions: one attempted question out of ten gives 10% coverage; three valid retries/attempts give 100% attempt validity without increasing question coverage. Both guide and report contain the separate Q/P and V/N fields; U03 uses the corrected current-content condition.

## 0.1.1 follow-up review

See [detailed self-review](self-review-2026-09-22.md). The earlier credit failure above describes the 0.1.0 attempt; this later review successfully ran two independent agents.

- Pre-edit review read all 13 files and simulated three scenarios. It identified insufficient explicit stage guidance, missing per-task manual steps, optional technical signals treated as checklist requirements, condition-level N/A ambiguity and unclear restoration handling.
- After revision, a fresh-context read-only agent evaluated five scenarios: novice Australian English cake shop, direct GEO request without prerequisites, condition-level N/A arithmetic, conflicting index/crawler/automated-query requests, and approved Shopify restoration after rendering failure.
- All five produced supported decisions. The N/A fixture returned A=20, V=10, E=10, observed 100, coverage 50%, possible range 50–100. Missing baseline data did not halt supported preparation; unapproved writes stayed pending; already approved restoration did not request duplicate permission.
- The fresh agent found a residual wording tension between task acceptance and already-live Shopify data. The execution log now explicitly separates task state from publication facts. This final wording clarification received local review, not another independent behavioral run.
- Structural checks and arithmetic passed. Official quick_validate still failed because PyYAML is absent. All simulations used fictional inputs and performed no live writes or queries.

## Remaining live validation as of 2026-09-22

Real customer site crawl/modification, live Shopify authorization or API write, actual ChatGPT/Google/Gemini collection, recurring scheduler, real ranking uplift, other AI hosts and non-Windows installations. Simulated fixtures cannot establish these capabilities.
