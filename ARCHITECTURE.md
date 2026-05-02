# Architecture

```
┌──────────────────────────────────────────────────────────────────┐
│                        User Interface Layer                        │
│         Feishu (primary) │ Telegram (alerts) │ CLI │ TUI         │
└──────────────────────────────┬───────────────────────────────────┘
                               │
┌──────────────────────────────▼───────────────────────────────────┐
│                     Hermes Gateway (WebSocket)                     │
│         Session Management │ Auth │ Platform Adapters │ Hooks       │
└──────────────────────────────┬───────────────────────────────────┘
                               │
┌──────────────────────────────▼───────────────────────────────────┐
│                        AIAgent (Core)                             │
│  ┌─────────────┐ ┌─────────────┐ ┌─────────────┐ ┌─────────────┐ │
│  │   Router    │ │  Context    │ │   Memory    │ │   Tools     │ │
│  │ (Provider  │ │ (Skills +   │ │ (SQLite +   │ │ (50+ built- │ │
│  │  routing)   │ │  History)   │ │  Session)   │ │  in)        │ │
│  └─────────────┘ └─────────────┘ └─────────────┘ └─────────────┘ │
└──────────────────────────────┬───────────────────────────────────┘
                               │
          ┌────────────────────┼────────────────────┐
          │                    │                    │
          ▼                    ▼                    ▼
   ┌────────────┐      ┌────────────┐      ┌────────────┐
   │  Terminal  │      │  File I/O  │      │  Web APIs  │
   │  (local +  │      │ (knowledge │      │ (search +  │
   │   docker)   │      │   base)    │      │  scrape)   │
   └────────────┘      └────────────┘      └────────────┘
          │                    │                    │
          └────────────────────┼────────────────────┘
                               │
                    ┌──────────▼──────────┐
                    │   Delegation Layer   │
                    │  OpenClaw │ Claude  │
                    │  Code │ Codex │ n8n   │
                    └─────────────────────┘
                               │
                    ┌──────────▼──────────┐
                    │  Cron Scheduler      │
                    │  Daily 9AM │ Sat 6PM │
                    └─────────────────────┘
```

## Session Memory

- **Storage**: SQLite with FTS5 full-text search
- **Context Window**: 205k tokens (MiniMax-M2.7)
- **Caching**: 40-80% context cached across sessions
- **Platform Memory**: Per-user, per-chat conversation history

## Autonomous Loop

```
    ┌──────────────────────────────┐
    │   Cron Trigger (9:00 AM)      │
    └──────────────┬───────────────┘
                   │
    ┌──────────────▼───────────────┐
    │   Fetch: AI + 跨境 feeds     │
    └──────────────┬───────────────┘
                   │
    ┌──────────────▼───────────────┐
    │   Summarize + Extract Insights │
    └──────────────┬───────────────┘
                   │
    ┌──────────────▼───────────────┐
    │   Write to Knowledge Base     │
    │   (~/Documents/王威的笔记/)   │
    └──────────────┬───────────────┘
                   │
    ┌──────────────▼───────────────┐
    │   Report via Feishu Bot       │
    └───────────────────────────────┘
```
