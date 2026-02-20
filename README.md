# seo-ai-tool

50+ professional SEO prompt commands for Claude Code. Install once, use everywhere.

## Install

```bash
npm install -g seo-ai-tool
seo-ai-tool install
```

That's it. All commands are now available as Claude Code slash commands from any folder.

## Requirements

- [Node.js](https://nodejs.org) 16+
- [Claude Code](https://www.npmjs.com/package/@anthropic-ai/claude-code) — `npm install -g @anthropic-ai/claude-code`

Run `seo-ai-tool check` to verify both are installed.

## Available commands

| Category | Commands |
|---|---|
| Technical SEO | `/robots-audit` `/sitemap-audit` `/schema-generator` `/canonical-audit` `/hreflang-audit` `/cwv-diagnosis` `/redirect-map` `/internal-links` `/server-logs` `/crawl-budget` |
| On-Page SEO | `/title-rewrite` `/headings-audit` `/alt-text` `/content-brief` `/content-refresh` `/faq-generator` `/thin-content` `/meta-descriptions` |
| Content & Links | `/keyword-research` `/write-blog` `/pillar-page` `/topic-cluster` `/content-calendar` `/comparison-article` `/outreach-email` `/brand-mention-pitch` `/press-release` `/backlink-article` |
| Local SEO | `/gbp-description` `/local-landing` `/review-responses` |
| E-commerce | `/product-description` `/category-page` `/product-schema` |
| Analytics | `/ga4-traffic` `/ga4-conversions` `/ga4-content` `/gsc-indexing` `/gsc-links` `/gsc-performance` |
| Reporting | `/competitor-analysis` `/content-gap` `/monthly-report` `/penalty-diagnosis` |
| GEO / LLM | `/geo-audit` `/geo-rewrite` `/geo-entity` `/geo-visibility` `/geo-citations` |
| Agents | `/agent-monthly-report` |

Run `seo-ai-tool list` to see all commands in the terminal.

## Customize prompts per project

Global prompts work everywhere, but sometimes you need a client-specific version of a prompt. The local override system makes this easy.

### How it works

Claude Code reads commands in this priority order:

```
.claude/commands/write-blog.md     ← local (wins if exists)
~/.claude/commands/write-blog.md   ← global (fallback)
```

### Set up local overrides

```bash
# In your client project folder
cd ~/projects/acme-client
seo-ai-tool init

# Copy the prompt you want to customize
cp ~/.claude/commands/write-blog.md .claude/commands/write-blog.md

# Edit it to match the client's tone, brand, or requirements
```

Commit `.claude/commands/` to git and your whole team shares the same customized prompts automatically.

## CLI reference

```
seo-ai-tool install     Copy all prompts to ~/.claude/commands/ (global)
seo-ai-tool update      Update global prompts to the latest version
seo-ai-tool init        Create .claude/commands/ in current project
seo-ai-tool list        List all prompts by category
seo-ai-tool check       Check if Claude Code and Gemini CLI are installed
seo-ai-tool uninstall   Remove all prompts from ~/.claude/commands/
seo-ai-tool help        Show help
```

## Update

```bash
npm update -g seo-ai-tool
seo-ai-tool update
```

## Tips

- Place a `brand-voice.md` file in your project root — content commands will read it automatically and match the brand's tone
- Store client data exports in a `data/` folder — audit commands will find them there
- Save outputs to an `outputs/` folder with descriptive filenames for easy reference

## License

MIT
