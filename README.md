# Hermes OS 🧠

> **Autonomous AI Coding Agent — Personal AI Operating System**
> Running 24/7 on Mac mini, powered by Hermes Agent + OpenClaw + Claude Code

## What is Hermes OS?

Hermes OS is a self-evolving autonomous AI agent system that manages itself, learns continuously, and handles real-world tasks — all without manual intervention. It's not just a chatbot; it's a personal AI that works while you sleep.

**Live Status**: 24/7 running on Mac mini (macOS 26.4 arm64)

## Core Capabilities

### 🤖 Multi-Agent Orchestration
```
┌─────────────────────────────────────────────────────┐
│              Hermes Agent (Main Orchestrator)         │
│  ┌──────────┐  ┌──────────┐  ┌──────────────────┐│
│  │ OpenClaw │  │ Claude   │  │ Hermes Cron Jobs  ││
│  │  Agent   │  │ Code     │  │ (Daily Learning)  ││
│  └──────────┘  └──────────┘  └──────────────────┘│
│  ┌──────────┐  ┌──────────┐  ┌──────────────────┐│
│  │ Session  │  │  Skill   │  │  Platform Tools   ││
│  │  Memory  │  │ Discovery│  │ (Feishu/Telegram) ││
│  └──────────┘  └──────────┘  └──────────────────┘│
└─────────────────────────────────────────────────────┘
```

### 📊 Autonomous Learning System
- **Daily Briefings (9:00 AM)**: Auto-scrapes AI news + cross-border e-commerce feeds
- **Knowledge Base**: 90+ notes covering AIGC, TikTok Shop, dropshipping, FPV drones
- **Self-Review (Saturday 6:00 PM)**: Analyzes past week's performance, updates skills
- **Delivery**: Summaries sent via Feishu Bot to personal chat

### 🌍 Production Deployments

#### 1. Italian Luxury Watch Dropshipping System 🇮🇹
- **Stack**: TikTok Shop → WhatsApp Cloud API → Chatwoot (Docker) → n8n → MiniMax Translation
- **Market**: Italy (European luxury watch reseller, dropshipping model)
- **AI Features**: Auto-translation, customer service automation, order workflow

#### 2. Multi-Agent Code Execution Platform
- **Stack**: Hermes Agent + OpenClaw + Claude Code + Codex
- **Features**: Parallel subagent execution, session memory (SQLite FTS5), skill-based tool discovery
- **Scale**: 500+ tasks executed autonomously

#### 3. FPV Drone Configuration Agent 🚁
- **Models**: GHF435AIO V2 20A Flight Stack, HSKRC 1104 7500KV Motors, Caddx Turtle Digital VTX
- **Automation**: Cross-platform price comparison (Taobao/Pinduoduo/Xianyu/1688)
- **Output**: Shopping lists with best prices, spec comparisons

## System Architecture

```
User Request (Feishu/Telegram)
         ↓
   Hermes Gateway (WS)
         ↓
   ┌─────────────┐
   │ AIAgent    │ ← Context (memory + skills + history)
   │ (Router)   │
   └──────┬──────┘
          ↓
   ┌──────┴──────┐
   │   Tool Call │
   ├─────────────┤
   │• Delegation │  → OpenClaw / Claude Code / Codex
   │• Terminal   │  → Python / Shell / Git
   │• File       │  → Knowledge Base / Notes
   │• Web        │  → Search / Crawl / API
   │• Cron       │  → Scheduled Learning Jobs
   │• Platform   │  → Feishu / Telegram / Send
   └─────────────┘
          ↓
   Session Memory (SQLite FTS5)
          ↓
   Cron: Daily 9AM Learning → Saturday 6PM Self-Review
```

## Tech Stack

| Component | Technology |
|-----------|------------|
| Main Agent | Hermes Agent ( NousResearch ) |
| Sub-Agents | OpenClaw, Claude Code, Codex |
| Model | MiniMax-M2.5, GLM-4.5V (vision) |
| Memory | SQLite FTS5, persistent sessions |
| Scheduler | Hermes Cron (built-in) |
| Platforms | Feishu (primary), Telegram (alerts) |
| OS | macOS 26.4 arm64 (Mac mini) |
| Self-Evolution | Skill creation, autonomous learning |

## Daily Workflow

```
09:00 AM ────────────────────────────────────── Daily Learning
│ • Monitor AI news feeds (web scraping)
│ • Cross-border e-commerce intelligence  
│ • Summarize → write to knowledge base
│ • Report → Feishu Bot
│
Saturday ─────────────────────────────────────── Self-Review
│ • Analyze week's task completion
│ • Update/extend skills
│ • Generate improvement report
│
24/7 ────────────────────────────────────────── Passive standby
│ • Respond to Feishu/Telegram messages
│ • Execute delegated tasks
│ • Monitor system health
```

## Projects & Results

- **Autonomous Learning Pipeline**: 90+ knowledge notes, auto-updated
- **TikTok Italy Watch Project**: Full dropshipping workflow operational
- **FPV Drone Config DB**: Comprehensive spec database + price tracking
- **Hermes Self-Evolution**: Skills improved every Saturday autonomously

## Repository Structure

```
hermes-os/
├── README.md              # This file
├── SKILLS.md              # Active skill catalog
├── ARCHITECTURE.md        # System design docs
├── WORKFLOWS.md           # Daily operation workflows
├── CLAUDE.md              # Claude Code integration guide
└── .github/
    └── workflows/         # (CI/CD for knowledge sync)
```

## Getting Started

Hermes OS is built on [Hermes Agent](https://github.com/NousResearch/hermes-agent) by NousResearch.

```bash
# Install Hermes Agent
pip install hermes-agent

# Configure your channels (Feishu, Telegram, etc.)
hermes setup

# Clone and customize
git clone https://github.com/Weiwei1210/hermes-os
cd hermes-os
```

## Metrics

- **Uptime**: 24/7 autonomous operation
- **Tasks Executed**: 500+ (managed autonomously)
- **Knowledge Base**: 90+ notes (auto-maintained)
- **Daily Token Consumption**: Optimized via session caching
- **Self-Evolution Rate**: Skills updated every Saturday

---

*Hermes OS — 让 AI 为自己干活*
