# Hermes OS — Autonomous AI Personal Agent

> **24/7 AI Agent System** | Powered by Hermes Agent + OpenClaw + Claude Code | [github.com/Weiwei1210/hermes-os](https://github.com/Weiwei1210/hermes-os)

---

## Live Production Deployments

### 🇮🇹 Italian Luxury Watch Dropshipping System

**Autonomous e-commerce pipeline running on Mac mini 24/7:**

```
TikTok Content → WhatsApp Italy → AI Auto-Reply → Order → Dropshipping

Stack: TikTok Shop + WhatsApp Cloud API + Chatwoot (Docker) + n8n + MiniMax Translation
Market: Italy (luxury watches: Longines, Tissot,梅花, TAG Heuer)
Model: Dropshipping (zero inventory), domestic supplier → direct to Italian customer
AI Features: Real-time Italian/Chinese translation, automated customer service, order workflow
```

**Operational Architecture:**
```
Italian Customer (WhatsApp)
    ↓ message
WhatsApp Cloud API
    ↓ webhook
Chatwoot (Docker on Mac mini)
    ↓ ticket created
MiniMax Translation Layer (port 8787)
    ↓ AI translates IT→ZH
You reply in Chinese
    ↓ AI translates ZH→IT
Chatwoot → WhatsApp → Italian Customer
```

**Business Model:**
- Product: Luxury watches (Longines, Tissot, TAG Heuer, etc.)
- Supply: Domestic supplier channels, dropshipping model
- Market: Italy (high brand recognition for Swiss watches)
- Pricing: €500-3000 range, 20-40% margin
- Logistics: Italy专线 8-12 days, include customs clearance
- Tax: 22% Italian VAT (customer pays), duty declared accurately

**Key Differentiators:**
| Problem | Solution |
|---------|----------|
| 7-hour time difference | AI auto-reply 24/7, no manual overnight coverage needed |
| Language barrier (Italian) | MiniMax AI real-time translation |
| Inventory risk | Dropshipping, zero stock |
| Trust issues | TikTok content + authentic warranty cards |

**Content Strategy:**
- 40% product close-ups (dial, movement, wrist shots)
- 30% brand stories ("Why Italians love Longines?")
- 20% lifestyle pairings (business/casual/gift)
- 10% logistics transparency ("From China warehouse to your door")

**Italian Timezone Workflow:**
| Beijing Time | Italy Time | Activity |
|---|---|---|
| 09:00-14:00 | 02:00-07:00 | Monitor, occasional |
| **14:00-22:00** | **07:00-15:00** | **Primary reply window ✅** |
| 22:00-24:00 | 15:00-17:00 | Process backlog |

**Tools Deployed:**
- ✅ Docker (Mac mini, auto-start)
- ✅ Chatwoot (localhost:3000)
- ✅ Translation Middleware (localhost:8787, MiniMax API)
- ☐ WhatsApp Cloud API (pending)
- ☐ TikTok account (pending)

---

### 🤖 Multi-Agent Orchestration Platform

**Architecture:**
```
┌─────────────────────────────────────────────────────────────┐
│              Hermes Agent (Main Orchestrator)                  │
│  ┌──────────┐  ┌──────────┐  ┌──────────┐  ┌──────────┐ │
│  │ OpenClaw │  │ Claude   │  │  Hermes  │  │  Hermes  │ │
│  │  Agent   │  │ Code     │  │  Cron    │  │  Memory  │ │
│  └──────────┘  └──────────┘  └──────────┘  └──────────┘ │
│  ┌──────────┐  ┌──────────┐  ┌──────────┐  ┌──────────┐ │
│  │ Session  │  │  Skill   │  │ Platform │  │  File &  │ │
│  │  Memory  │  │ Discovery│  │ (Feishu) │  │Terminal │ │
│  └──────────┘  └──────────┘  └──────────┘  └──────────┘ │
└─────────────────────────────────────────────────────────────┘
```

**Key Stats:**
- 500+ tasks executed autonomously
- 205k token context window (MiniMax-M2.7)
- 40-80% context cached across sessions
- SQLite FTS5 full-text search memory
- Session history: 10+ concurrent sessions

---

### 📊 Autonomous Learning System

**Daily Cron (9:00 AM Beijing):**
```
1. Scrape AI news feeds (web search)
2. Monitor cross-border e-commerce intelligence
3. Summarize → write to knowledge base (90+ notes)
4. Report → Feishu Bot (personal channel)
```

**Weekly Self-Review (Saturday 6:00 PM):**
```
1. Analyze past week's task completion
2. Identify skill gaps and failure patterns
3. Update/extend Hermes skills
4. Generate improvement report
```

**Knowledge Base Topics:**
- AIGC tools and workflows
- TikTok Shop operations
- Italy luxury market intelligence
- Dropshipping logistics
- FPV drone builds
- AI agent best practices

---

### 🚁 FPV Drone Configuration Agent

**Automated research across Taobao/Pinduoduo/Xianyu/1688:**

| Component | Model | Status |
|-----------|-------|--------|
| Flight Controller | GHF435AIO V2 20A | ✅ Researched |
| Motors | HSKRC 1104 7500KV | ✅ Researched |
| Digital VTX | Caddx Turtle | ✅ Researched |
| Frame | Black哥 X20 | ✅ Researched |
| Battery | 3S 550mah ×3 | ☐ Pending |
| Charger | iMAX B6 mini | ☐ Pending |

Output: Comprehensive spec comparison, cross-platform price tracking, shopping list with best deals.

---

## System Stack

| Layer | Technology |
|-------|------------|
| Main Agent | Hermes Agent (NousResearch) |
| Sub-Agents | OpenClaw, Claude Code, Codex |
| Model | MiniMax-M2.5, GLM-4.5V (vision) |
| Memory | SQLite FTS5, persistent sessions |
| Scheduler | Hermes Cron (built-in) |
| Platforms | Feishu (primary), Telegram (alerts) |
| OS | macOS 26.4 arm64 (Mac mini) |
| Docker | Chatwoot, n8n |
| Translation | MiniMax API (IT↔ZH) |
| E-commerce | TikTok Shop, WhatsApp Cloud API |

---

## Repository Structure

```
hermes-os/
├── README.md           # This file — overview + production deployments
├── SKILLS.md           # Active skill catalog (50+ skills)
├── ARCHITECTURE.md     # System design + data flows
└── .github/
    └── workflows/      # CI/CD for knowledge sync
```

---

## Metrics

- **Uptime**: 24/7 autonomous (Mac mini always on)
- **Tasks Executed**: 500+ (zero manual triggers for routine ops)
- **Knowledge Base**: 90+ notes, auto-updated
- **Daily Token Budget**: Optimized via session caching + context compression
- **Self-Evolution**: Skills updated every Saturday autonomously
- **Platform Coverage**: Feishu (primary), Telegram (alerts), CLI (local)

---

## What Makes This Different

Most "AI agents" are one-shot chat tools. Hermes OS is:

1. **Truly Autonomous** — Cron jobs run on schedule, no human in the loop
2. **Self-Evolving** — Learns from failures, updates its own skills
3. **Multi-Agent** — Coordinates OpenClaw + Claude Code + Codex for parallel execution
4. **Production-Grade** — Real e-commerce pipeline handling real customers
5. **MemoryPersistent** — Remembers everything across sessions

---

*Built with [Hermes Agent](https://github.com/NousResearch/hermes-agent) by NousResearch*
