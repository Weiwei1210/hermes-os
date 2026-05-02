# Hermes OS Skills

Active skills deployed in production, maintained by Hermes's autonomous self-evolution system.

## 🏃 Core Agent Skills

| Skill | Description | Status |
|-------|-------------|--------|
| `terminal` | Execute shell commands, manage processes | ✅ Active |
| `file` | Read/write/search files, manage knowledge base | ✅ Active |
| `web` | Web search, scraping, HTTP requests | ✅ Active |
| `delegation` | Spawn subagents (OpenClaw, Claude Code, Codex) | ✅ Active |
| `cronjob` | Schedule autonomous tasks | ✅ Active |
| `skills` | Discover, load, and create skills | ✅ Active |
| `session_search` | Search conversation history | ✅ Active |

## 🤖 Delegation Skills

| Skill | Tool | Use Case |
|-------|------|----------|
| `claude-code` | Claude Code CLI | Code writing, PR review |
| `codex` | OpenAI Codex CLI | API integration, scripting |
| `opencode` | OpenCode CLI | General coding tasks |

## 📱 Platform Skills

| Skill | Platform | Capability |
|-------|----------|------------|
| `feishu_doc` | Feishu/Lark | Read/write docs, comments |
| `telegram` | Telegram | Send/receive messages |
| `send_message` | Multi-platform | Unified message delivery |

## 🔧 Operational Skills

| Skill | Description |
|-------|-------------|
| `autonomous-learning` | Daily AI/跨境 feeds monitoring + knowledge base updates |
| `system-update-all` | macOS dev tools update (brew, pip, npm) |
| `hermes-troubleshooting` | Hermes/OpenClaw debugging and recovery |
| `hermes-agent` | Hermes configuration and extension |

## 📊 Data Skills

| Skill | Description |
|-------|-------------|
| `jupyter-live-kernel` | Python REPL with tool integration |
| `huggingface-hub` | Model search/download |
| `notion` | Notion API integration |

## 🌐 Web & Research

| Skill | Description |
|-------|-------------|
| `youtube-content` | Transcripts → summaries |
| `blogwatcher` | RSS/Atom feed monitoring |
| `arxiv` | Academic paper search |

## 🔄 Self-Evolution

Skills are automatically updated every Saturday during the self-review cron job.
New skills are created based on task patterns and failure analysis.

---

*Last updated: 2026-05-01 (auto)*
