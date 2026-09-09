# Meta Ads MCP — Facebook & Instagram Ads for Claude, ChatGPT & Cursor

**Create and manage Facebook & Instagram (Meta) ad campaigns from your AI assistant.** Adbloop's Meta Ads MCP server lets Claude, ChatGPT, and Cursor launch, scale, and manage real Meta Ads campaigns — bulk creation, multi-account, spend guardrails, and reporting — through a hosted, one-click connection. No developer app, no API keys, no self-hosting.

[![Meta Verified Tech Provider](https://img.shields.io/badge/Meta-Verified%20Tech%20Provider-1877F2)](https://adbloop.com/mcp/)
[![Works with Claude · ChatGPT · Cursor](https://img.shields.io/badge/works%20with-Claude%20·%20ChatGPT%20·%20Cursor-5A67D8)](https://adbloop.com/mcp/)
[![Free plan](https://img.shields.io/badge/plan-Free%20to%20start-16A34A)](https://adbloop.com/pricing/)
[![License: BSL 1.1](https://img.shields.io/badge/license-BSL%201.1-blue)](./LICENSE)

> **150 Facebook campaigns. Under 2 minutes. Done.** — the same bulk engine, available from your dashboard, Google Sheets, or your AI assistant.

---

## What is this?

The **Adbloop Meta Ads MCP** is a hosted [Model Context Protocol](https://modelcontextprotocol.io) server that connects your AI assistant to the **Meta Marketing API** (Facebook & Instagram Ads). Ask Claude or ChatGPT to build campaigns in plain language — Adbloop handles the Meta API, validation, rate limits, and the 108 real-world failure cases that break naive integrations.

It's the AI door into the same engine behind [adbloop.com](https://adbloop.com): a Meta Verified Tech Provider used by solo advertisers and agencies to launch Facebook & Instagram campaigns in bulk.

**This repo** is the connector's documentation, setup guides, and registry manifest. The Adbloop service runs hosted — nothing to install.

---

## Quick start (2 minutes)

1. **Create a free account** → [app.adbloop.com](https://app.adbloop.com) and connect your Meta (Facebook) ad account. Adbloop reuses this connection, so there are no separate API keys to manage.
2. **Add the MCP to your assistant:**
   - **Claude** (Desktop / web): one-click OAuth — see [docs/connect.md](./docs/connect.md#claude).
   - **ChatGPT** (Developer Mode): add the Adbloop connector — see [docs/connect.md](./docs/connect.md#chatgpt).
   - **Cursor / other MCP clients:** see [docs/connect.md](./docs/connect.md#cursor).
3. **Ask in plain language:** *"Create 20 Facebook conversion campaigns from this Google Sheet, all paused, $10/day each."* → review → launch.

Full setup for every client: **[docs/connect.md](./docs/connect.md)**

---

## What it can do

Grouped by what you'd actually ask for. Full reference: **[docs/tools.md](./docs/tools.md)**.

**Create & launch at scale**
- Create single Facebook/Instagram campaigns end to end (campaign → ad set → ad).
- **Bulk-create** dozens to hundreds of campaigns in one request.
- **Multi-account bulk** — launch across several ad accounts at once (agencies).
- Build ads from creatives in your connected Google Drive folder.

**Stay safe before you spend**
- **Validate** every campaign against Meta's rules before anything goes live.
- **Guardrails** — enforce per-campaign and account spend caps.
- **Capacity & estimate checks** — know batch size and rate-limit headroom up front.
- Everything can be created **paused** so nothing spends until you say so.

**Manage what's running**
- Pause, resume, delete campaigns; update budgets.

**Read & report**
- List accounts, campaigns, ad sets, and ads; pull performance insights, creative library, lead forms, and targeting options.

> Tool descriptions here say *what* each tool does, not *how* — the validation, error-recovery, and rate-limit logic that make bulk Meta Ads reliable run server-side.

---

## Why Adbloop

Most Meta Ads MCP servers only reach people who run an MCP client. Adbloop is the **same campaign engine reachable three ways** — so it fits the whole team, not just the AI power user:

- 🤖 **AI assistants** — Claude, ChatGPT, Cursor (this MCP)
- 📊 **Google Sheets** — a Workspace-Marketplace add-on that bulk-creates 130+ campaigns per batch, for media buyers who live in spreadsheets
- 🖥️ **Web dashboard** — [app.adbloop.com](https://app.adbloop.com)

Plus what makes bulk Meta Ads actually survive contact with the Meta API:

- **Bulk-first** — 150+ Facebook campaigns in under 2 minutes.
- **108 documented Meta API fixes** — hardened against the failures that break naive agents (invalid targeting, rate limits, malformed creatives, partial-batch failures, hallucinated IDs).
- **Multi-account** for agencies (3–10 accounts by plan).
- **Meta Verified Tech Provider.**
- **Flat pricing** — no per-spend fees. Free to start; Pro $19/mo; Agency $49/mo.

---

## Safety

Letting an AI touch a live ad account is a real risk. How Adbloop handles it: **[docs/safety.md](./docs/safety.md)** — paused-by-default creation, pre-flight validation, spend guardrails, and capacity checks.

---

## Links

- 🌐 Product: [adbloop.com](https://adbloop.com) · MCP: [adbloop.com/mcp](https://adbloop.com/mcp/)
- 🚀 Start free: [app.adbloop.com](https://app.adbloop.com)
- 💬 Example prompts: [examples/prompts.md](./examples/prompts.md)
- 🔒 Security policy: [SECURITY.md](./SECURITY.md)

---

## Keywords

Meta Ads MCP · Facebook Ads MCP · Facebook Ads automation · Meta Ads automation · AI Facebook Ads · ChatGPT Facebook Ads · Claude Meta Ads · Facebook Ads API · Meta Marketing API · bulk Facebook Ads · bulk Meta Ads · Instagram Ads automation · MCP server for Facebook Ads

## License

[Business Source License 1.1](./LICENSE) — free to use and self-reference; converts to Apache 2.0 on 2029-01-01. You may not use it to offer a competing hosted Meta Ads MCP service.
