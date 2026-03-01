# 🦞 Claw Kits — Pre-Built OpenClaw Setups

> Drop-in workspace configurations that turn OpenClaw into a specialized employee.

## What Is OpenClaw?

[OpenClaw](https://github.com/openclaw/openclaw) is an open-source AI agent that runs on your own machine. It connects to Telegram, WhatsApp, Slack, Discord and actually *does things* — browses the web, writes code, manages files, runs on a schedule, and remembers everything between sessions. Think of it as an autonomous AI employee, not a chatbot.

## What Are Claw Kits?

OpenClaw is powerful but takes hours to configure properly. Claw Kits are pre-built workspace setups for specific use cases. Each kit includes:

- **SOUL.md** — Personality, behavior rules, and domain expertise
- **AGENTS.md** — Workflow, memory system, correction loop
- **HEARTBEAT.md** — Automated daily routines and proactive checks
- **TOOLS.md** — Domain-specific workflows, templates, and file structures
- **IDENTITY.md** — Agent name, role, and character
- **USER.md** — Template for your personal info
- **MEMORY.md** — Long-term memory starter (curated by the agent over time)

## Available Kits

### ✍️ Content Creator
Turn your agent into a full content operation. Monitors trends, drafts posts in your voice, manages a content calendar, and repurposes across platforms.
**Best for:** Creators, influencers, thought leaders, ghostwriting clients

### 💪 Fitness Coach
Your agent becomes a personal trainer + nutritionist + accountability partner. Food photo macro tracking, workout programming, streak tracking, and three coaching modes (supportive, drill sergeant, data nerd).
**Best for:** Fitness enthusiasts, personal trainers managing clients, anyone building health habits

### 🛠️ Dev Team
Your agent becomes an engineering department. Reads codebases, builds features, runs tests, manages deployments. Spawns sub-agents for parallel development.
**Best for:** Solo founders, indie hackers, agencies, non-technical builders

### 🔍 SEO Agency
Fully autonomous SEO operation. Keyword research, content generation, internal linking, outreach emails, performance tracking. Runs 24/7.
**Best for:** Content sites, affiliate marketers, agencies scaling without hiring

### 🎯 Sales Rep · 📋 Executive Assistant · 🔬 Research Analyst
*Premium kits — same quality, deeper domains. Available at [apiforchads.com](https://apiforchads.com).*
*More niches coming. Drop requests in [Issues](https://github.com/chadbot0x/claw-kits/issues).*

## Quick Start

### 1. Pick Your Kit
```bash
# First, copy the base files (shared across all kits)
cp claw-kits/base/* ~/.openclaw/workspace/

# Then copy your chosen kit (overwrites SOUL.md with the specialized version)
cp -r claw-kits/content-creator/* ~/.openclaw/workspace/
# Or: fitness-coach, dev-ops, agency-seo

# Create required directories
mkdir -p ~/.openclaw/workspace/memory

# Kit-specific directories (create the one matching your kit):
# Content Creator:
mkdir -p ~/.openclaw/workspace/content/{drafts,templates}
# Fitness Coach:
mkdir -p ~/.openclaw/workspace/fitness/log
# Dev Team:
mkdir -p ~/.openclaw/workspace/projects
# SEO Agency:
mkdir -p ~/.openclaw/workspace/seo/{content,reports}
```

### 2. Customize
Edit the `<!-- FILL IN -->` sections in each file:
- `USER.md` — Your name, timezone, preferences
- `IDENTITY.md` — Name your agent
- `HEARTBEAT.md` — Configure your specific niche/goals
- `SOUL.md` — Adjust the vibe to match your style
- `TOOLS.md` — Add your API keys and workarounds as you go

Each kit also includes a starter template for its working files (content calendar, fitness plan, SEO keywords, etc.) — copy these into the appropriate directory to give your agent a head start.

### 3. Start OpenClaw
```bash
openclaw gateway start
```

Your agent reads the workspace files on first message and becomes the specialist you configured.

> **Tip:** Enable heartbeats for the best experience. Heartbeats let your agent run background checks on a schedule (trend scanning, fitness reminders, git status, etc.). Set `heartbeat.enabled: true` and `heartbeat.intervalMs` in your OpenClaw config. See [OpenClaw docs](https://docs.openclaw.ai) for details.

## Building Your Own Kit

Every kit follows the same structure. To create a custom kit:

1. Start with `base/` templates
2. Write a domain-specific `SOUL.md` (personality + expertise + rules)
3. Design a `HEARTBEAT.md` (what should it check automatically?)
4. Create a `TOOLS.md` (workflows, file structures, templates)
5. Test it for a week and iterate based on corrections

The best kits come from deep domain knowledge. If you understand a niche's daily workflow, you can build a kit that replaces 10+ hours of manual work per week.

## Philosophy

> "The people who will win aren't the best engineers. They're the ones who understand the buyer's daily workflow better than the buyer does."

Claw Kits bridge the gap between OpenClaw's power and the average user's patience. The technology is free. The configuration is the product.

---

Built by [@chadbot0x](https://x.com/chadbot0x) | [apiforchads.com](https://apiforchads.com)
