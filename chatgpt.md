# SEO Prompts — ChatGPT Context

This file contains instructions for using this SEO prompt library with ChatGPT Projects.

## Setup (one time)

1. Create a new **ChatGPT Project**
2. Go to the project **Instructions** and paste the contents of this file
3. Upload the skill files you need from the `skills/` folder into the project **Knowledge**
4. Optionally upload your `brand-voice.md` to the project Knowledge so it applies automatically

## How to run a prompt

Once the skill files are in the project Knowledge, reference them by name and provide your context:

```
Use the robots-txt-audit skill and audit this robots.txt file:
[paste robots.txt here]
```

```
Use the ga4-organic-traffic-analysis skill.
The GA4 data is attached. Site: acme.com. Period: last 3 months vs prior 3 months.
```

```
Use the write-blog-post skill.
Primary keyword: "project management software", audience: SMB owners, site: acme.com
```

## Available skills by category

### Technical SEO
- `robots-txt-audit` — audit robots.txt for blocked resources, syntax errors, and crawl issues
- `xml-sitemap-audit` — audit XML sitemaps for non-200 URLs and structural issues
- `schema-markup-generator` — generate valid JSON-LD for any schema type
- `canonical-tags-audit` — audit canonical tags for chains and conflicts
- `hreflang-audit` — audit hreflang annotations for missing return links and incorrect codes
- `core-web-vitals-diagnosis` — diagnose LCP, INP, and CLS failures with code-level fixes
- `redirect-map-generator` — generate redirect maps and server config rules
- `internal-linking-audit` — audit internal link structure for orphaned pages
- `check-server-app-logs` — analyze server logs for 404s, crawl waste, and Googlebot anomalies
- `crawl-budget-analysis` — analyze crawl budget waste and produce a prioritized crawl efficiency action plan

### On-Page SEO
- `title-tag-rewrite` — rewrite title tags for improved CTR and keyword placement
- `heading-structure-audit` — audit H1–H3 structure and produce an optimized outline
- `image-alt-text-generator` — generate SEO-optimized, accessibility-compliant alt text
- `content-brief` — create a detailed, writer-ready content brief
- `content-refresh` — produce a section-by-section content refresh plan
- `faq-section-generator` — generate PAA-targeted FAQ sections with FAQPage JSON-LD
- `thin-content-rewrite` — diagnose and rewrite thin content pages
- `write-meta-descriptions` — generate click-optimized meta descriptions

### Content & Link Building
- `keyword-research` — full keyword research with intent classification and cluster suggestions
- `write-blog-post` — write a 1,200–1,800 word SEO-optimized blog post
- `pillar-page-writer` — write a 2,500–4,000 word pillar page
- `topic-cluster-planner` — design a complete topic cluster with internal linking map
- `content-calendar` — build an SEO content calendar in markdown table format
- `comparison-article` — write a commercial comparison article with head-to-head table
- `outreach-email-template` — write outreach sequences for 6 link building campaign types
- `unlinked-brand-mention-pitch` — write pitches to convert unlinked mentions into backlinks
- `press-release` — write a 400–600 word AP-style press release
- `write-a-backlink-article` — write an editorial article with a natural backlink placement

### Local SEO
- `google-business-profile-description` — write 3 GBP description variants
- `local-landing-page-writer` — write a local landing page for a service + city combination
- `review-response-templates` — generate 12 review response templates

### E-commerce SEO
- `product-description-writer` — write product descriptions in three formats
- `category-page-content-writer` — write above- and below-the-fold category page content
- `product-schema-generator` — generate complete Product JSON-LD

### Analytics & Data
- `ga4-organic-traffic-analysis` — analyze GA4 organic traffic trends and landing page quality
- `ga4-conversion-analysis` — identify which organic pages drive the most conversions
- `ga4-content-performance` — map content into a traffic × engagement matrix
- `gsc-indexing-audit` — diagnose GSC Coverage report exclusions
- `gsc-links-report-analysis` — analyze GSC link data for equity distribution

### Reporting & Analysis
- `competitor-analysis` — full competitive intelligence report with 3-month action plan
- `content-gap-analysis` — identify keyword and topic gaps with a prioritized content roadmap
- `google-search-console-analysis` — analyze GSC performance data with top 10 action items
- `monthly-report-writer` — write a client-ready monthly SEO report
- `penalty-diagnosis` — diagnose traffic drops with a recovery action plan

### GEO & LLM Optimization
- `geo-content-audit` — audit a page across 7 GEO dimensions with a GEO Readiness Score
- `geo-content-rewrite` — rewrite a page to maximize AI citation chances
- `geo-entity-definition` — create a complete entity definition package with JSON-LD
- `geo-brand-visibility-checker` — generate a brand visibility test set across AI tools
- `geo-ai-citation-analysis` — analyze AI citation sources and find content opportunities

## Brand voice

If `brand-voice.md` is uploaded to the project Knowledge, apply its tone, vocabulary, and language to all content output automatically.

## Important notes

- Always review AI output before publishing, deploying, or sending to a client.
- Never share client data without explicit client permission.
- Placeholders in output are marked `[PLACEHOLDER: description]` — search for `[` before treating any output as final.
