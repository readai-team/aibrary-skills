# Aibrary Skills

Skills for [Claude Code](https://code.claude.com) and [OpenClaw](https://openclaw.ai) powered by [Aibrary](https://aibrary.ai) — the world's first Agentic AI for lifelong learning.

Turn books into actionable knowledge — search, recommend, curate, generate podcast scripts, and plan your growth, all from the command line.

## Installation

### Option 1 — [OpenClaw](https://openclaw.ai)

Read https://www.aibrary.ai/skill.md and follow the instructions to install Aibrary Skills.

### Option 2 — [ClawHub](https://clawhub.ai/)

ClawHub installs skills individually:

```bash
npx clawhub@latest install aibrary-book-search
npx clawhub@latest install aibrary-podcast-summary
```

Available skills: `aibrary-100`, `aibrary-book-search`, `aibrary-book-recommend`, `aibrary-reading-list`, `aibrary-foryou-topic`, `aibrary-growth-plan`, `aibrary-podcast-summary`, `aibrary-podcast-dialogue`, `aibrary-podcast-ideatwin`

### Option 3 — [skills.sh](https://skills.sh/)

```bash
npx skills add readai-team/aibrary-skills
```

### Option 4 — Manual (git clone)

**Add to your project (recommended for teams)**

```bash
git clone https://github.com/readai-team/aibrary-skills.git
cp -r aibrary-skills/skills/* your-project/.claude/skills/
```

Skills committed to `.claude/skills/` are automatically discovered when Claude Code opens that project.

**Add as personal skills (available across all projects)**

```bash
git clone https://github.com/readai-team/aibrary-skills.git
mkdir -p ~/.claude/skills
cp -r aibrary-skills/skills/* ~/.claude/skills/
```

After installation, type `/aibrary-book-search`, `/aibrary-podcast-summary`, etc. in Claude Code to use.

## Skills Overview

### 📖 Book Discovery

| Skill | Command | What it does |
|-------|---------|--------------|
| **Book Search** | `/aibrary-book-search` | Find books matching a scenario, need, or question |
| **Book Recommend** | `/aibrary-book-recommend` | Get personalized 1-3 book recommendations with reading strategies |
| **Reading List** | `/aibrary-reading-list` | Generate a themed, multi-stage reading list with logical order |

### 🎙️ Podcast Generation

| Skill | Command | What it does |
|-------|---------|--------------|
| **Podcast Summary** | `/aibrary-podcast-summary` | Generate a 10-15 min single-narrator summary podcast script |
| **Podcast Dialogue** | `/aibrary-podcast-dialogue` | Generate a 10-15 min host + guest conversational podcast script |
| **Podcast Idea Twin** | `/aibrary-podcast-ideatwin` | Generate a 10-15 min debate podcast between your AI twin and a book expert |

### 🌱 Learning & Growth

| Skill | Command | What it does |
|-------|---------|--------------|
| **ForYou Topic** | `/aibrary-foryou-topic` | Get personalized book topic recommendations based on your profile |
| **Growth Plan** | `/aibrary-growth-plan` | Create a structured, time-bound growth plan with weekly tasks |
| **Aibrary 100** | `/aibrary-100` | Browse the curated 100 must-read books for the AI age |

## Usage Examples

### Find books for a specific challenge

```
/aibrary-book-search I'm leading a team building microservices and we keep running into coordination problems
```

### Get a personalized recommendation

```
/aibrary-book-recommend I'm a senior engineer thinking about moving into management
```

### Generate a podcast script from a book

```
/aibrary-podcast-summary Thinking, Fast and Slow
```

```
/aibrary-podcast-dialogue --book "Atomic Habits" --focus "habit stacking and environment design"
```

### Debate a book's ideas with your AI twin

```
/aibrary-podcast-ideatwin --book "Antifragile" --stance "I think most systems should prioritize stability over antifragility"
```

### Plan your growth

```
/aibrary-growth-plan --goal "Transition from engineer to engineering manager" --duration "12 weeks"
```

### Browse the Aibrary 100

```
/aibrary-100 --category "systems-thinking"
```

## Features

- **Bilingual adaptive output** — responds in the same language as your input (English, Chinese, etc.)
- **Pure prompt mode** — no API keys or external dependencies required
- **Structured output** — every skill produces well-formatted, actionable results
- **Interconnected skills** — use `aibrary-book-search` to find books, `aibrary-podcast-summary` to turn them into audio scripts, and `aibrary-growth-plan` to build a learning roadmap around them

## Repository Structure

```
aibrary-skills/
├── README.md
├── LICENSE
└── skills/
    ├── aibrary-book-search/      # Scenario-based book discovery
    │   └── SKILL.md
    ├── aibrary-book-recommend/   # Personalized book recommendations
    │   └── SKILL.md
    ├── aibrary-reading-list/     # Themed multi-book reading lists
    │   └── SKILL.md
    ├── aibrary-podcast-summary/  # Single-narrator summary podcast scripts
    │   └── SKILL.md
    ├── aibrary-podcast-dialogue/ # Two-person dialogue podcast scripts
    │   └── SKILL.md
    ├── aibrary-podcast-ideatwin/ # AI twin debate podcast scripts
    │   └── SKILL.md
    ├── aibrary-foryou-topic/     # Personalized topic recommendations
    │   └── SKILL.md
    ├── aibrary-growth-plan/      # Structured growth plans
    │   └── SKILL.md
    └── aibrary-100/              # 100 must-read books for the AI age
        └── SKILL.md
```

## About Aibrary

[Aibrary](https://aibrary.ai) is built by [Ouraca Inc.](https://ouraca.com), a Silicon Valley innovator in AI and education technology. Aibrary transforms trusted knowledge — from best-selling books to expert insights — into personalized learning experiences through AI podcasts, an Idea Twin debate companion, and a dedicated AI growth team.

## License

[MIT](LICENSE) — Ouraca Inc.
