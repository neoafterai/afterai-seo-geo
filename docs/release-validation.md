# Pre-release validation — AfterAI SEO/GEO 0.1.2

Date: 2026-09-22. Scope: final local candidate, without a customer site, production credentials, publication or paid services. This report supersedes earlier statements that the official validator could not run; historical logs remain accurate for their original attempts.

## User-facing simplification

One installable skill, not 13 skills. Thirteen Markdown files remain so the assistant can load only relevant detail. Users see four steps (assess, plan, implement, review/maintain) and three everyday phrases (start, continue, monthly check). Precise old phrases remain supported.

Templates are created when needed and filled by the assistant. Small changes use compact task descriptions; only complex or manual work needs full cards. Users can request a report at any stage. Full GEO observation still defaults to 30 queries, may be completed in batches, and is not a prerequisite for a technical audit or report. Continue preserves the existing scope, including report-only limits.

## Checks actually performed

| Check | Result and limit |
|---|---|
| Official skill-creator quick_validate | PASS on final skill, including real YAML parsing. Temporary PyYAML installed only in the development temp directory; no dependency added to package |
| Validator positive/negative fixtures | 7 expected outcomes: valid sample passes; missing frontmatter, invalid name, missing description, unsupported field, unfinished TODO and malformed YAML are rejected |
| Package structure | Exactly 13 files, all .md, English filenames, exactly one SKILL.md; no executable or development-skill dependency |
| Local references | Workspace relative file links and ASCII section anchors resolve; installation references remain within the package |
| Markdown and encoding | UTF-8, no replacement/null characters, balanced code fences, consistent table columns |
| Basic publication hygiene | Package scan found no obvious machine paths, private-key blocks or common token patterns; this is not a comprehensive security certification |
| Isolated copy and archive | Copied all 13 files through a path containing spaces and Chinese characters; in-memory ZIP integrity and byte equality passed, with no development docs included |
| Scoring arithmetic | 17,208 combinations of applicable/verified/earned weights respected bounds and zero/full-coverage behavior; 16 condition pairs and all six type-budget allocations checked |
| GEO retry arithmetic | Repeated attempts preserved unique-question coverage; valid-attempt and recommendation denominators remained distinct |
| Source availability | Across this review series, all 22 unique linked sources in the package were opened using the web tool; source access does not establish all claims or permanent availability |
| Independent edge review | Separate agent read 13 files and worked through 10 language, index, scoring, privacy, Shopify and scheduling cases; detailed outcomes below |
| Independent usability review | Separate agent simulated five conversational turns and identified unnecessary visible ceremony and ID ambiguity; corrections applied |
| Local offline artifact test | Six fictional Markdown records generated in a temporary customer folder; baseline hash preserved across a second run, repeated E001 IDs disambiguated by run, report/resume responses respected no-write scope |
| Independent final artifact test | NOT COMPLETED: a fresh agent started but failed due workspace credits. Local artifact checks are not represented as its successful execution |

### Official-validator environment

Initial sandboxed dependency download failed due network restrictions. Approved temporary PyYAML installation succeeded. The sandbox could not read the resulting dependency folder; the approved development-context validator then returned `Skill is valid!`. Seven fixtures also passed their expected outcomes. No global Python environment or installable skill dependency was changed.

### Ten independent edge cases

1. English user: response in English, audit does not authorize edits.
2. Chinese user, site language unknown: ask the target audience language while continuing unrelated supported checks.
3. Two real language versions: inspect intended canonical/hreflang relationships, do not merge just because themes match; two equal-weight pages with one passing give 50% for that item.
4. SaaS without a store: Software module retains the 20-point type budget; illustrative core 80 + W01 10 + W02 5 = 95.
5. No observations: V=0 means unmeasured, not failed; A=0 means not applicable.
6. P=10, Q=3, N=5, V=0: coverage 30%, attempt validity 0%, recommendation/citation/first metrics undefined; another failed retry changes N, not Q.
7. Customer-folder mismatch: resolve identity before customer writes or reuse of facts/approvals.
8. Malicious webpage instructions: treated as content, no upload of customer records.
9. Shopify theme-only approval: does not authorize shared product writes; present concrete field changes first.
10. No scheduler: manual mode, no fabricated schedule or task ID.

### Issues found and corrected

- Cross-run E001/R-ID ambiguity: references now carry run-id, and customer task/keyword/approval IDs are not reused. Question IDs include panel version.
- G09 without comparable third-party evidence: explicitly unmeasured, not half credit or an assumed pass. Rubric advanced to 0.1.2; affected historical comparisons require recalculation or an incomparable label.
- Unbounded failed AI collection: default at most one permitted transient-error retry; no automatic retry around limits, login or CAPTCHA; manual/blocked state remains visible.
- Excessive intake and mandatory-looking templates: record fields are not a customer questionnaire; 1–3 current missing facts, incremental files, concise updates.
- Report-only burden: report current evidence without demanding the remaining workflow or full AI panel.

## Local offline artifact exercise

Used a fictional Sydney custom-cake shop, English website and Chinese operator. Only a short offline title/H1/body/contact-link extract and pickup-only business facts were supplied. No URL was visited. Outputs were profile.md, plan.md, progress.md, one report and two evidence files in a temporary directory, outside the product.

The report kept scores unmeasured because full conditions could not be checked; it did not infer missing whole-site content from a short extract. A single shared SEO/GEO task proposed English title/body improvements without invented pricing, allergens or delivery. Report-only and resume responses retained the no-website-write scope. Original evidence bytes were unchanged after recording the second run. This is a self-simulation and file-integrity exercise, not a live customer outcome or independent model evaluation.

## What remains before public release

- Real-site pilot with an identified, authorized site and actual tools: crawl, preview/visual checks, actual changes and restoration where applicable, then same-scope rescore. No such site or access has been supplied.
- Actual Shopify connection and live/shared-data behavior, actual GSC data handling and manual AI observation where selected. These cannot be established by fictional fixtures.
- Host discovery and execution on other operating systems/products. The package-copy test is portability evidence, not proof of each host's behavior.
- Real recurring scheduler only when available and requested; outcome changes require later observations rather than same-day assertions.
- Owner's public license and GitHub destination. Neither a license grant nor publication is implied by this candidate.

No known unresolved blocking document defect was found in the completed local checks. This is not a zero-bug guarantee. Additional independent final artifact evaluation remains unexecuted due credits; live tests remain unexecuted due missing site/access. Do not mark these passed to make a release checklist look complete.
