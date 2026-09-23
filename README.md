# ai-elements

> **Vercel-grade AI UI components** - shadcn-style React component library for AI apps - chat, streams, code blocks, citations, prompts, branches - built by Vercel, mirrored and extended here.

<p align="center"><a href="https://github.com/hmzainjamil/ai-elements">Repository</a> · <a href="https://github.com/hmzainjamil/ai-elements/commits/main">Commits</a> · <a href="https://github.com/hmzainjamil/ai-elements/issues">Issues</a></p>
<p align="center"><img alt="Documentation" src="https://img.shields.io/badge/documentation-deep%20editorial-lightgrey"> <img alt="Lifecycle" src="https://img.shields.io/badge/lifecycle-active-success"></p>

<!-- HMZ DEEP README v1 -->

## At a glance

| Field | Current state |
|---|---|
| Repository | ai-elements |
| Visibility | Public |
| Lifecycle | Active |
| Evidence basis | Current repository documentation and source-visible material |

## Why this exists

**Vercel-grade AI UI components** - shadcn-style React component library for AI apps - chat, streams, code blocks, citations, prompts, branches - built by Vercel, mirrored and extended here.

The README documents the component-library scope and separates repository-local interfaces from behavior supplied by external frameworks, models, or hosting platforms.

## CONCEPTS

| Concept | Location | Description |
|---|---|---|
| **Repo README** | `README.md` | Library overview + install - [Source](https://github.com/hmzainjamil/ai-elements/blob/main/README.md) |
| **Apps workspace** | `apps` | Docs + demo apps - [Source](https://github.com/hmzainjamil/ai-elements/blob/main/apps) |
| **Cursor ultracite** | `.cursor/rules/ultracite.mdc` | Cursor lint + format rules - [Source](https://github.com/hmzainjamil/ai-elements/blob/main/.cursor/rules/ultracite.mdc) |
| **Oxlint config** | `.oxlintrc.json` | Oxlint rule set - [Source](https://github.com/hmzainjamil/ai-elements/blob/main/.oxlintrc.json) |
| **Oxfmt config** | `.oxfmtrc.jsonc` | Oxfmt formatter rules - [Source](https://github.com/hmzainjamil/ai-elements/blob/main/.oxfmtrc.jsonc) |
| **Skills workflow** | `.github/workflows/generate-skills.yml` | Auto-emits Claude Code skill registry - [Source](https://github.com/hmzainjamil/ai-elements/blob/main/.github/workflows/generate-skills.yml) |
| **Release workflow** | `.github/workflows/release.yml` | Changesets publish pipeline - [Source](https://github.com/hmzainjamil/ai-elements/blob/main/.github/workflows/release.yml) |
| **Test workflow** | `.github/workflows/test.yml` | CI test matrix - [Source](https://github.com/hmzainjamil/ai-elements/blob/main/.github/workflows/test.yml) |
| **Claude CLAUDE.md** | `.claude/CLAUDE.md` | Claude Code project guide - [Source](https://github.com/hmzainjamil/ai-elements/blob/main/.claude/CLAUDE.md) |
| **Changeset config** | `.changeset/config.json` | Versioning + release config - [Source](https://github.com/hmzainjamil/ai-elements/blob/main/.changeset/config.json) |

## HOW IT WORKS

```
+---------------------------------------------------------+
|                       INPUT                             |
|   React . Tailwind v4 . shadcn registry conventions |
+--------------------------+------------------------------+
                           v
+---------------------------------------------------------+
|                  ORIENT / PARSE                         |
|   - Validate inputs                                     |
|   - Load skill / agent / tool definitions               |
|   - Resolve config + secrets from .env                  |
+--------------------------+------------------------------+
                           v
+---------------------------------------------------------+
|                  PLAN (Claude Sonnet)                   |
|   - Decompose goal into ordered subtasks                |
|   - Pick model per task (Sonnet / Haiku / Tier-0)       |
+--------------------------+------------------------------+
                           v
+---------------------------------------------------------+
|                  EXECUTE (parallel)                     |
|   - Spawn sub-agents / call tools                       |
|   - Stream tokens, persist artifacts                    |
+--------------------------+------------------------------+
                           v
+---------------------------------------------------------+
|                  VERIFY                                 |
|   - Lint / typecheck / visual diff / QA agent           |
|   - On failure -> re-prompt with error context          |
+--------------------------+------------------------------+
                           v
+---------------------------------------------------------+
|                  SHIP                                   |
|   - Write to disk . commit . PR . upload                |
+---------------------------------------------------------+
```

## Install

```bash
git clone https://github.com/hmzainjamil/ai-elements.git
cd ai-elements

# Per-repo install (try in order):
bash install.sh 2>/dev/null || \
npm install 2>/dev/null || \
bun install 2>/dev/null || \
pip install -r requirements.txt 2>/dev/null || true
```

Environment:

```bash
cp .env.example .env  # if present
# fill ANTHROPIC_API_KEY at minimum
```

## Usage

```bash
# Claude Code skill packs:
/skill-name "your goal"

# CLI / scripts:
python scripts/<script>.py --input ./input --output ./output

# TypeScript projects:
bun run dev    # or npm run dev
```

### Configuration knobs

| Key | Default | Description |
|---|---|---|
| `ANTHROPIC_API_KEY` | - (required) | Claude API key |
| `MODEL` | `claude-sonnet-4-7` | Default LLM |
| `MODEL_FALLBACK` | `claude-haiku-4` | Cheaper fallback |
| `MAX_TOKENS` | `8192` | Per-call ceiling |
| `TEMPERATURE` | `0.2` | Determinism dial |
| `LOG_LEVEL` | `info` | debug / info / warn / error |
| `OUT_DIR` | `./out` | Where artifacts land |
| `CACHE_DIR` | `.cache` | Prompt cache root |
| `PARALLELISM` | `4` | Sub-agent concurrency |
| `RETRY_MAX` | `3` | Per-call retry budget |
| `TIMEOUT_S` | `120` | Per-call timeout |
| `DRY_RUN` | `false` | Plan-only, no side effects |

### Case 3 - DTC brand, ad creative testing

- Before: $2K/month UGC creator retainer, 4 ads/month.
- After: 30+ ad variants/week via Arcads + Claude, A/B-tested.
- Result: 3x creative velocity, 41% lower CAC after 6 weeks.

## Security

- Never commit API keys. `.env` is in `.gitignore` by default.
- Use [git-secret](https://git-secret.io/) or 1Password CLI for team secret sharing.
- Review the QA / safety layer for any tool that writes to disk or runs shells (see `mac_safety.py` style guards).
- Vulnerability reports: open a private GitHub Security Advisory.

## Limitations

- Framework and dependency behavior can change independently of this repository.
- Visual and runtime compatibility claims require actual environment testing.
- Quantitative adoption or performance claims require reproducible measurements.

## Related

- [Claude Code](https://docs.claude.com/en/docs/claude-code) - official docs
- [Anthropic Console](https://console.anthropic.com) - API keys + billing
- [Crawlee](https://crawlee.dev) - web scraping framework
- [hmz-claude-code-best-practice](https://github.com/hmzainjamil/hmz-claude-code-best-practice) - sister repo

## Maintainer

[hmzainjamil](https://github.com/hmzainjamil)