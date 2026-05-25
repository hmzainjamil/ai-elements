# ai-elements

> **AI elements — reusable Claude Code building blocks for agent workflows**

![Status](https://img.shields.io/badge/status-active-brightgreen?style=flat)
![License](https://img.shields.io/badge/license-MIT-blue?style=flat)
![Claude Code](https://img.shields.io/badge/Claude_Code-Skill-FF6B35?style=flat)
![Stars](https://img.shields.io/github/stars/hmzainjamil/ai-elements?style=flat)
![Last Commit](https://img.shields.io/github/last-commit/hmzainjamil/ai-elements?style=flat)

---

## CONCEPTS

| Concept | Description |
|---|---|
| **Elements** | Core elements capability for ai-elements workflows |
| **Blocks** | Core blocks capability for ai-elements workflows |
| **Components** | Core components capability for ai-elements workflows |
| **Claude** | Core claude capability for ai-elements workflows |
| **Agent** | Core agent capability for ai-elements workflows |
| **Reusable** | Core reusable capability for ai-elements workflows |
| **Workflow** | Core workflow capability for ai-elements workflows |
| **Building** | Core building capability for ai-elements workflows |

---

## 🔥 Hot Commands

```bash
# Activate skill
claude --skill ai-elements 'your task'

# Quick workflow
claude 'elements automation task'

# Get capabilities
claude 'what can ai-elements do?'
```

## ■ tip
> Mention **elements** or **blocks** in your prompt to auto-activate this skill.

---

## ☠️ STARTUPS / BUSINESSES

- **Agencies**: automate elements workflows for clients at scale
- **Founders**: ship blocks features 10x faster with Claude
- **Freelancers**: deliver components work with AI-assisted precision

---

## Features

- Elements automation and orchestration
- Blocks automation and orchestration
- Components automation and orchestration
- Claude automation and orchestration
- Agent automation and orchestration
- Reusable automation and orchestration

---

## Installation

```bash
git clone https://github.com/hmzainjamil/ai-elements.git
cd ai-elements
```

---

## Usage

```bash
# In Claude Code
/ai-elements
claude 'elements task here'
```

---

## Configuration

| Variable | Description | Default |
|---|---|---|
| `API_KEY` | Primary API key for service access | Required |
| `MODEL` | AI model to use | claude-3-5-sonnet |
| `DEBUG` | Enable verbose debug output | false |
| `MAX_TOKENS` | Max token budget per request | 8192 |
| `TIMEOUT` | Request timeout in seconds | 30 |
| `LOG_LEVEL` | Logging verbosity | info |

---

## Architecture

```
ai-elements/
├── README.md           # This file
├── SKILL.md            # Claude Code skill definition
├── scripts/            # Automation and utility scripts
├── templates/          # Output and prompt templates
├── examples/           # Usage examples and demos
├── tests/              # Unit and integration tests
└── docs/               # Extended documentation
    ├── setup.md        # Setup guide
    ├── api.md          # API reference
    └── faq.md          # Frequently asked questions
```

---

## Examples

### Basic Usage

```bash
# Activate in Claude Code
claude --skill ai-elements "your task here"

# With options
claude --skill ai-elements --verbose "detailed task"
```

### Advanced Workflow

```bash
# Chain with other skills
claude --skill ai-elements "step 1" | claude --skill summarize

# Batch processing
for item in list; do
  claude --skill ai-elements "process $item"
done
```

---

## Troubleshooting

| Issue | Cause | Fix |
|---|---|---|
| Auth fails | Invalid/expired API key | Re-export key in shell profile |
| Timeout error | Network latency or large payload | Increase TIMEOUT value |
| Empty output | Prompt too vague | Add more context to request |
| Rate limit hit | Too many requests | Add delay between calls |
| Model error | Unsupported model version | Update MODEL variable |
| Import error | Missing dependency | Run pip install -r requirements.txt |

---

## Comparison

| Feature | This Skill | Alternative A | Alternative B |
|---|---|---|---|
| Claude Code native | ✅ | ❌ | ✅ |
| Auto-activation | ✅ | ✅ | ❌ |
| Free to use | ✅ | ❌ | ✅ |
| Production ready | ✅ | ✅ | ❌ |
| Active maintenance | ✅ | ❌ | ❌ |

---

## Contributing

1. Fork this repo
2. Create feature branch: `git checkout -b feat/your-feature`
3. Commit changes: `git commit -m 'feat: add feature'`
4. Push: `git push origin feat/your-feature`
5. Open PR

---

## Changelog

| Version | Changes |
|---|---|
| v2.0 | Major refactor, Claude 4 support |
| v1.5 | Added auto-activation keywords |
| v1.0 | Initial release |

---

## ⭐ Star History

[![Star History Chart](https://api.star-history.com/svg?repos=hmzainjamil/ai-elements&type=Date)](https://star-history.com/#hmzainjamil/ai-elements&Date)

---

## 📜 License

MIT — free to use, modify, and distribute.

---

Made with ❤️ by [@hmzainjamil](https://github.com/hmzainjamil)
