# Hermes OS — Autonomous AI Personal Agent

> **24/7 AI Agent System** | Powered by Hermes Agent + OpenClaw + Claude Code | [github.com/Weiwei1210/hermes-os](https://github.com/Weiwei1210/hermes-os)

---

## Live Production Deployments

### 🇮🇹 Italian Luxury Watch Dropshipping System

**Autonomous e-commerce pipeline running 24/7 on Mac mini:**

```
TikTok Content → WhatsApp Italy → AI Auto-Reply → Order → Dropshipping

Stack: TikTok Shop + WhatsApp Cloud API + Chatwoot (Docker) + n8n + MiniMax Translation
Market: Italy (luxury watches: Longines, Tissot, TAG Heuer)
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

---

#### 📋 Full Business Plan (from 0 to MVP)

**Core Conclusion:** Start from zero — don't spread across all of Europe at once. Run MVP with "1 country + 3-5 watch styles + 30-50 TikTok videos + WhatsApp/Chatwoot private customer service." Goal: validate that people watch, ask, buy, receive, and after-sales is controllable.

##### 1. Project Positioning

| Element | Recommendation |
|---------|---------------|
| Category | Own-brand fashion watches — daily wear, men's style, gift, couples watches; smart watches postponed (CE, Bluetooth, battery, APP, after-sales complexity) |
| Market | Start with 1 country. UK first, then DE/FR/ES/IT |
| Channel | TikTok for content acquisition → WhatsApp for consultation → Chatwoot for multi-channel aggregation, real-time translation, team collaboration |
| Price Range | First test: €29-99 (impulse buy + gift); later expand to €99-199 premium |
| Core Selling Points | High appearance, outfit matching, gift appeal, waterproof/scratch-resistant/luminous/replaceable strap, affordable |
| Risk Boundaries | Own-brand expression only; no trademarks, logos, packaging, or misleading brand hints; claims match actual specs |

> ⚠️ **Important:** Own-brand fashion watches work in Europe. Smart watches involve CE, Bluetooth, battery, APP, after-sales — postpone to Phase 2.

##### 2. Complete Business Loop

| Goal | Method |
|------|--------|
| Use TikTok to identify which styles, selling points, and audiences respond | Content testing |
| Use WhatsApp to capture high-intent customers, reduce cold traffic drop-off | Private domain |
| Use real-time translation to solve European multilingual customer service | AI translation |
| Use customer tags and response templates to turn one consultation into a repeatable sales process | SOP + CRM |

##### 3. Phase 1 MVP: Run Through, Don't Chase Perfection

| Phase | What | Goal |
|-------|------|------|
| Week 1 | Confirm country, select 3-5 watches, organize selling points, build WhatsApp/Chatwoot pipeline | Can serve customers |
| Week 2 | Shoot/edit 30-50 short videos, establish TikTok account, start organic traffic test | Validate content direction |
| Week 3 | Accumulate comments/DM/WhatsApp consultation scripts, optimize translation, pricing, follow-up flow | Improve consultation conversion |
| Week 4 | Analyze data, eliminate low-feedback styles, keep high-consultation styles, decide whether to scale | Find scalable model |

**What NOT to do first:**
- Don't stock large inventory at the start
- Don't cover all of Europe with multi-language, multi-account, multi-site
- Don't spend heavily on brand packaging — validate product and content first
- Keep own-brand expression unified: brand name, logo, packaging, detail page, customer service scripts

##### 4. Product Selection Strategy

**Prioritize testing:**
- Men's fashion watches
- Vintage leather strap watches
- Minimalist business watches
- Couples gift watches
- Replaceable strap models
- Waterproof, luminous, scratch-resistant (easy to video)

**Be cautious:**
- Smart watches: CE, Bluetooth, battery, APP, after-sales
- Counterfeit/similar-to-brand: high infringement risk in Europe
- Ultra-cheap low-quality: bad reviews and returns will tank the account
- Heavy, fragile packaging: high logistics and after-sales cost

**Product Scoring Matrix:**

| Dimension | Standard | Weight |
|-----------|----------|--------|
| Video Performance | Can it impress via unboxing, wrist shots, outfit matching, close-ups? | High |
| Margin Space | Profit after sourcing, logistics, payment, after-sales, ads? | High |
| Infringement Risk | Looks like a brand? Similar logo, dial, packaging, naming? | High |
| After-sales Risk | Breaks easily? Size disputes? Color differences? Fragile shipping? | High |
| Gift Appeal | Suitable for birthdays, couples, holidays, Father's Day, Christmas? | Medium |
| Supply Stability | Can replenish steadily? Backup suppliers available? | Medium |

##### 5. TikTok Content Strategy

**Principle:** European users prefer authentic, natural, lifestyle content — not hard selling. Watch content should focus on "wrist effect, outfit matching, gift scenarios, price surprise, detail credibility."

**Content Matrix:**

| Type | How to Shoot | Goal |
|------|-------------|------|
| Wrist Outfit Shots | Close-up wrist + full-body outfit, commuting/dating/party/gift scenarios | Plant |
| Unboxing Detail | Packaging, dial, strap, wearing process, close-up details | Build trust |
| Before/After | "Normal outfit vs with watch" visual contrast | Create demand |
| Price Anchor | Emphasize "looks premium, affordable price" — no brand imitation hints | Drive consultation |
| Gift Scenarios | Birthdays, anniversaries, Father's Day, Christmas, couples gifts | Convert |
| Feature Demo | Waterproof, luminous, strap replacement, scratch test — real demos | Reduce hesitation |

**30 Starter Video Topics:**
1-5: Men's daily outfit, before/after wrist shots
6-10: Unboxing details — dial, strap, packaging, wrist effect
11-15: Gift scenarios — for boyfriend/father/friend/self
16-20: Feature demos — waterproof, luminous, strap change, scratch resistance
21-25: Price and value — "premium feel, friendly price"
26-30: FAQ — size, logistics, returns, waterproof, how to buy

##### 6. WhatsApp + Chatwoot Customer Service Architecture

**Phase 1: Manual Private Domain Validation**
- Use standalone phone + WhatsApp Business App to serve customers
- Verify if customers are willing to move from TikTok to WhatsApp
- Accumulate high-frequency questions: price, logistics, material, waterproof, size, after-sales
- Build standard scripts and tag system

**Phase 2: Chatwoot Systematic Customer Service**

| Capability | Description |
|-----------|-------------|
| Multi-agent Collaboration | Multiple agents unified in Chatwoot backend |
| Conversation Management | All WhatsApp consultations in one backend — no missed messages on phone |
| Customer Tags | By country, language, intent, budget, style, order status |
| Notes Accumulation | Record customer needs, purchase preferences, after-sales, repurchase triggers |
| AI Translation | Customer foreign language → Chinese; agent Chinese → customer language |
| Data Asset | Customer data stays in own system — reduce SaaS dependency |

**8 Questions to Validate:**

| # | Question | Current Status |
|---|----------|---------------|
| 1 | Can WhatsApp Business API stably connect to Chatwoot? | Pending validation |
| 2 | Can Meta Business Manager / WABA / phone number be smoothly approved? | Pending prep |
| 3 | Can customer messages in EN/DE/FR/ES/IT auto-translate to Chinese? | Prototype built, pending real API |
| 4 | Can agent Chinese replies be translated to customer language before sending? | Pending real API |
| 5 | Do Chatwoot tags, notes, agent assignment meet daily operations? | Local backend ready, pending business test |
| 6 | Do WhatsApp template messages pass compliance review? | Pending application |
| 7 | Do we need to sync Shopify / standalone site / Feishu spreadsheet? | Pending decision |
| 8 | Do we use VPS + domain + HTTPS for production environment? | Strongly recommended |

##### 7. Customer Service Scripts

**Welcome Message:**
> Hi! Thanks for your interest in our watches. 😊
> Which style are you looking for: daily wear, business, gift, or couple watches?
> You can send me the number/photo of the watch you like, and I'll help you check the price, size and delivery time.

**Internal Chinese Agent Response Logic:**

| Customer Question | Response Key Points |
|------------------|-------------------|
| How much? | Quote + shipping included? First order discount? Payment method |
| How long to deliver? | Target country ETA, tracking provided |
| Waterproof? | Only state actual rating — don't exaggerate. Daily water resistant ≠ swimming/diving |
| What size? | Dial diameter, strap length, suitable wrist range — with wearing photo if possible |
| Can I return? | Clear return window, conditions, who pays return shipping |
| Is it real leather / stainless steel? | Answer truthfully — don't mislabel |
| Good for gifting? | Emphasize packaging, greeting card, couples/birthday/holiday scenarios |

**Follow-up Script:**
> Just a quick note: this style is currently one of our most requested watches.
> If you want, I can reserve one for you today and send the payment link here.

##### 8. Transaction & Fulfillment Prep

| Module | Prep Content | Priority |
|--------|-------------|---------|
| Payment | PayPal, credit card, standalone site payment link. Don't rely solely on private transfer | High |
| Landing Page | At minimum: product photos, price, specs, logistics, returns, contact info | High |
| Logistics | Test with domestic direct shipping first; consider European overseas warehouse when stable | High |
| Returns | Clear return address and policy. European local return address improves conversion | Medium |
| Packaging | Watches suit gift-style packaging — but don't over-invest early | Medium |
| Service SOP | Standardize: consultation → quote → follow-up → payment → shipping → after-sales → review | High |

##### 9. Europe Compliance & Risks

| Risk | Resolution | Priority |
|------|-----------|---------|
| Trademark/appearance infringement | No brand logos, similar dials, or "XX alternative" hints | Critical |
| Smart watch certification | If doing smart watches: confirm CE, RoHS, Bluetooth, battery, manual, APP compliance | High |
| GDPR | Privacy policy stating data usage, storage, deletion, export | High |
| WhatsApp opt-in | Only market after user consent; use compliant templates for mass messages | High |
| Returns | European consumers value transparent after-sales — landing page and scripts must be clear | High |
| Advertising claims | Don't exaggerate material, waterproof, origin, limited stock — only what can be proven | Medium |

##### 10. Budget Recommendations

| Item | Starting Budget | Notes |
|------|----------------|-------|
| Samples | ¥1,000-3,000 | Buy 3-5 styles, shoot content and test quality |
| Shooting | ¥0-3,000 | Phone works early — authenticity and frequency matter more |
| Tools | ¥0-500/month | Chatwoot open-source is free; main costs: server, domain, translation API, WhatsApp API messages |
| Ads | ¥3,000-10,000 | Start with organic traffic; add budget after validating content |
| Logistics/After-sales | 5-15% of order value | Cover resend, returns, damage, disputes |

##### 11. Key Metrics

| Metric | What to Watch | Purpose |
|--------|--------------|---------|
| Video completion rate | Do users watch to the end? | Judge content |
| Comment/DM rate | Are users interested in styles and prices? | Judge demand |
| WhatsApp fan rate | TikTok → private domain conversion efficiency | Judge traffic diversion |
| Effective consultation rate | Do WhatsApp contacts actually ask price/logistics/purchase? | Judge intake |
| Transaction rate | Proportion of effective consultations that convert | Judge scripts + product |
| Average order value | Revenue per order | Judge margin |
| Refund/after-sales rate | Quality, logistics, description issues | Judge supply chain |
| Repurchase/referral | Are old customers buying again or recommending? | Judge private domain value |

##### 12. 30-Day Execution Checklist

- [ ] Confirm first target country (UK recommended — low language barrier, high testing efficiency)
- [ ] Confirm 3-5 own-brand fashion watch samples, avoid counterfeit and smart watch compliance issues
- [ ] For each watch: organize specs (dial diameter, material, waterproof rating, weight, packaging, sourcing price, suggested retail price)
- [ ] Set up WhatsApp Business; prepare to upgrade to WhatsApp Business API
- [ ] Configure Chatwoot — key: verify WhatsApp intake, real-time translation, customer tags, team collaboration, data accumulation
- [ ] Prepare 30-50 TikTok video scripts and start shooting
- [ ] Prepare WhatsApp multilingual scripts: welcome, quote, logistics, after-sales, follow-up, review
- [ ] Build simplest landing page or payment page — ensure customers can pay securely
- [ ] Run 7-14 days organic test — count views, comments, DMs, fans, transactions per style
- [ ] Eliminate low-feedback styles, keep high-feedback styles, decide if ads should scale

> **Most Critical Next Step:** Don't chase brand ambition from day one. Build a testable closed loop first: samples, content, WhatsApp, translation customer service, payment, shipping. As long as first batch of real customers successfully purchase and receive — optimize brand, standalone site, overseas warehouse, and team later.

##### 13. Chatwoot + WhatsApp API Self-Hosted Architecture

**Recommended Stack:**

| Component | Address | Purpose |
|-----------|---------|---------|
| Chatwoot | github.com/chatwoot/chatwoot | Open-source customer service hub: conversations, customers, tags, multi-agent, API, WhatsApp and other channels |
| n8n | github.com/n8n-io/n8n | Automation workflows: follow-up, review requests, data sync, notifications, low-code flows |
| Typebot | github.com/baptisteArno/typebot | Visual chatbot: Q&A guidance, demand collection, preliminary customer filtering |
| WhatsApp Cloud API | Meta official | Official WhatsApp Business API — handles message send/receive and template messages |
| OpenAI / DeepL | API service | Real-time translation between customer language ↔ Chinese, plus sales-assist replies |

**Phase 1 Feature Scope:**
- Deploy Chatwoot as unified customer service backend
- Connect WhatsApp Business API, complete message send/receive
- Build translation middleware: customer foreign language auto-translated to Chinese
- Agent Chinese reply auto-translated to customer language before sending
- Build customer tags: country, language, intent, style, order status
- Accumulate watch sales script templates: quote, size, waterproof, logistics, returns, follow-up
- TikTok: use homepage link/comment/DM to guide to WhatsApp — don't do complex TikTok API initially

**Why Not Full Self-Build:**

| Semi-Self-Built Pros | Notes |
|---------------------|-------|
| More controllable than SaaS | Customer data stays with you |
| Faster than full development | Chatwoot already has backend capabilities |
| Can gradually connect orders, inventory, data dashboards | Step-by-step |

**Local Setup Status:**

| Service | Purpose | Status |
|---------|---------|--------|
| Chatwoot Rails | Customer service backend web service | ✅ Running |
| Sidekiq | Background task queue | ✅ Running |
| Postgres | Database | ✅ Running |
| Redis | Cache and queue dependency | ✅ Running |
| Translation Middleware Prototype | Simulate customer language ↔ Chinese translation flow | ✅ Local test passed |

Local access: **http://localhost:3000**

Common commands:
```bash
cd ~/Documents/跨境私域系统/chatwoot-local
docker compose ps      # View status
docker compose up -d   # Start
docker compose down    # Stop
docker compose logs -f rails  # View logs
```

**Next Steps:**
1. Open http://localhost:3000, create Chatwoot admin account
2. Create test inbox in Chatwoot to simulate customer conversations
3. Connect translation middleware to OpenAI or DeepL for real translation
4. Prepare Meta Business Manager and WhatsApp Business API for real WhatsApp connection
5. If external webhooks needed: use cloudflared/ngrok for temporary tunnel; migrate to VPS + domain + HTTPS for production

---

#### Business Model Summary

- **Product:** Luxury watches (Longines, Tissot, TAG Heuer, etc.)
- **Supply:** Domestic supplier channels, dropshipping model
- **Market:** Italy (high brand recognition for Swiss watches)
- **Pricing:** €500-3000 range, 20-40% margin
- **Logistics:** Italy专线 8-12 days, include customs clearance
- **Tax:** 22% Italian VAT (customer pays), duty declared accurately

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
