# ai-elements

> **AI elements — reusable Claude Code building blocks for agent workflow composition**

![Status](https://img.shields.io/badge/status-active-brightgreen?style=flat)
![License](https://img.shields.io/badge/license-MIT-blue?style=flat)
![Claude Code](https://img.shields.io/badge/Claude_Code-Skill-FF6B35?style=flat)
![Stars](https://img.shields.io/github/stars/hmzainjamil/ai-elements?style=flat)
![Last Commit](https://img.shields.io/github/last-commit/hmzainjamil/ai-elements?style=flat)

---

## CONCEPTS

| Concept | Description |
|---|---|
| **Element** | Atomic reusable unit of agent capability |
| **Composition** | Combine elements into complex workflows |
| **Input/Output** | Typed contracts between elements |
| **Retry Logic** | Built-in error recovery per element |
| **Caching** | Skip redundant calls with smart cache |
| **Logging** | Trace element execution for debugging |
| **Testing** | Unit-testable element interface |
| **Registry** | Discover available elements via index |

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
- **Founders**: ship blocks features 10x faster
- **Freelancers**: deliver components work with AI precision

---

## Features

- Elements automation
- Blocks automation
- Components automation
- Claude automation
- Agent automation
- Reusable automation

---

## Installation

```bash
git clone https://github.com/hmzainjamil/ai-elements.git
cd ai-elements
```

---

## Usage

```bash
# Activate skill in Claude Code
claude --skill ai-elements "your task here"

# Quick workflow
claude "elements automation task"

# Get help
claude "what can ai-elements do?"
```

---

## Configuration

| Variable | Description | Default |
|---|---|---|
| `API_KEY` | Primary API key | Required |
| `MODEL` | AI model to use | claude-3-5-sonnet |
| `DEBUG` | Enable verbose debug | false |
| `MAX_TOKENS` | Max token budget | 8192 |
| `TIMEOUT` | Request timeout (sec) | 30 |
| `LOG_LEVEL` | Logging verbosity | info |

---

## Architecture

```
ai-elements/
├── README.md           # Documentation
├── SKILL.md            # Claude Code skill definition
├── scripts/            # Automation scripts
├── templates/          # Output templates
├── examples/           # Usage examples
└── docs/               # Extended documentation
```

---

## Examples

### Basic

```bash
# Simple task
claude --skill ai-elements "elements task"

# Verbose
claude --skill ai-elements --verbose "detailed blocks task"
```

### Advanced Pipeline

```bash
# Chain skills
claude --skill ai-elements "step 1" | claude --skill summarize

# Batch run
for item in $(cat list.txt); do
  claude --skill ai-elements "process $item"
done
```

---

## Troubleshooting

| Issue | Cause | Fix |
|---|---|---|
| Auth fails | Invalid API key | Re-export key in shell profile |
| Timeout | Network or large payload | Increase TIMEOUT value |
| Empty output | Prompt too vague | Add more context |
| Rate limit | Too many requests | Add delay between calls |
| Model error | Unsupported version | Update MODEL variable |
| Import error | Missing dependency | Run pip install -r requirements.txt |

---

## Comparison

| Feature | This Skill | Alt A | Alt B |
|---|---|---|---|
| Claude Code native | ✅ | ❌ | ✅ |
| Auto-activation | ✅ | ✅ | ❌ |
| Free to use | ✅ | ❌ | ✅ |
| Production ready | ✅ | ✅ | ❌ |
| Active maintenance | ✅ | ❌ | ❌ |

---

## Changelog

| Version | Changes |
|---|---|
| v2.0 | Claude 4 support, auto-activation |
| v1.5 | Added keyword triggers |
| v1.0 | Initial release |

---

## Contributing

1. Fork → feature branch → commit → PR
2. Follow conventional commits: `feat:`, `fix:`, `docs:`
3. Add tests for new features

---

## ⭐ Star History

[![Star History Chart](https://api.star-history.com/svg?repos=hmzainjamil/ai-elements&type=Date)](https://star-history.com/#hmzainjamil/ai-elements&Date)

---

## 📜 License

MIT — free to use, modify, distribute.

---

Made with ❤️ by [@hmzainjamil](https://github.com/hmzainjamil)
