# Aibrary Skills

Skills for [Claude Code](https://code.claude.com) and [OpenClaw](https://openclaw.ai) powered by [Aibrary](https://aibrary.ai) — the world's first Agentic AI for lifelong learning.

Turn books into actionable knowledge — search, recommend, curate, generate podcast scripts, and plan your growth, all from the command line.

## Skills Overview

### 📖 Book Discovery

| Skill | Command | What it does |
|-------|---------|--------------|
| **Book Search** | `/book-search` | Find books matching a scenario, need, or question |
| **Book Recommend** | `/book-recommend` | Get personalized 1-3 book recommendations with reading strategies |
| **Reading List** | `/reading-list` | Generate a themed, multi-stage reading list with logical order |
| **Aibrary 100** | `/aibrary100` | Browse the curated 100 must-read books for the AI age |

### 🎙️ Podcast Generation

| Skill | Command | What it does |
|-------|---------|--------------|
| **Podcast Summary** | `/podcast-summary` | Generate a 10-15 min single-narrator summary podcast script |
| **Podcast Dialogue** | `/podcast-dialogue` | Generate a 10-15 min host + guest conversational podcast script |
| **Podcast Idea Twin** | `/podcast-ideatwin` | Generate a 10-15 min debate podcast between your AI twin and a book expert |

### 🌱 Learning & Growth

| Skill | Command | What it does |
|-------|---------|--------------|
| **ForYou Topic** | `/foryou-topic` | Get personalized book topic recommendations based on your profile |
| **Growth Plan** | `/growth-plan` | Create a structured, time-bound growth plan with weekly tasks |

## Usage Examples

### Find books for a specific challenge

```
/book-search I'm leading a team building microservices and we keep running into coordination problems
```

### Get a personalized recommendation

```
/book-recommend I'm a senior engineer thinking about moving into management
```

### Generate a podcast script from a book

```
/podcast-summary Thinking, Fast and Slow
```

```
/podcast-dialogue --book "Atomic Habits" --focus "habit stacking and environment design"
```

### Debate a book's ideas with your AI twin

```
/podcast-ideatwin --book "Antifragile" --stance "I think most systems should prioritize stability over antifragility"
```

### Plan your growth

```
/growth-plan --goal "Transition from engineer to engineering manager" --duration "12 weeks"
```

### Browse the Aibrary 100

```
/aibrary100 --category "systems-thinking"
```

## Features

- **Bilingual adaptive output** — responds in the same language as your input (English, Chinese, etc.)
- **Pure prompt mode** — no API keys or external dependencies required
- **Structured output** — every skill produces well-formatted, actionable results
- **Interconnected skills** — use `book-search` to find books, `podcast-summary` to turn them into audio scripts, and `growth-plan` to build a learning roadmap around them

## Installation

### Claude Code

Add this repository as a skills source in your Claude Code configuration:

```bash
# Clone the repository
git clone https://github.com/readai-team/aibrary-skills.git

# Add to your Claude Code skills directory
cp -r aibrary-skills/skills/* ~/.claude/skills/
```

### OpenClaw

Point your OpenClaw configuration to this repository's `skills/` directory. See [OpenClaw docs](https://docs.openclaw.ai/tools/skills) for details.

## Repository Structure

```
aibrary-skills/
├── README.md
├── LICENSE
└── skills/
    ├── book-search/        # Scenario-based book discovery
    │   └── SKILL.md
    ├── book-recommend/     # Personalized book recommendations
    │   └── SKILL.md
    ├── reading-list/       # Themed multi-book reading lists
    │   └── SKILL.md
    ├── podcast-summary/    # Single-narrator summary podcast scripts
    │   └── SKILL.md
    ├── podcast-dialogue/   # Two-person dialogue podcast scripts
    │   └── SKILL.md
    ├── podcast-ideatwin/   # AI twin debate podcast scripts
    │   └── SKILL.md
    ├── foryou-topic/       # Personalized topic recommendations
    │   └── SKILL.md
    ├── growth-plan/        # Structured growth plans
    │   └── SKILL.md
    └── aibrary100/         # 100 must-read books for the AI age
        └── SKILL.md
```

## About Aibrary

[Aibrary](https://aibrary.ai) is built by [Ouraca Inc.](https://ouraca.com), a Silicon Valley innovator in AI and education technology. Aibrary transforms trusted knowledge — from best-selling books to expert insights — into personalized learning experiences through AI podcasts, an Idea Twin debate companion, and a dedicated AI growth team.

## License

[MIT](LICENSE) — Ouraca Inc.
