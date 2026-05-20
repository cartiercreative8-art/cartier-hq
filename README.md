# CartierHQ — AI Command Center

> Full-stack React dashboard powering CartierCreative operations. Voice-activated, MCP-connected, and built entirely on an iPad.

---

## What It Is

CartierHQ is the internal operating system for CartierCreative. It's a custom-built React + HTML dashboard that gives me real-time visibility and control over every part of the business — leads, outreach, agents, pipeline, and revenue — all from a single screen.

No templates. No drag-and-drop tools. Built from scratch and live in production.

---

## 8 Functional Tabs

| Tab | Function |
|---|---|
| 🎙️ Voice | Wake word detection — activates Jarvis hands-free |
| 🤖 Jarvis Chat | Live AI assistant powered by Claude API (Anthropic) |
| 👥 Agent Roster | Status board for all 11 named agents |
| 📋 CRM | Live feed from Google Sheets — leads, status, follow-ups |
| 📡 Hermes | Cold outreach control panel — draft, send, track emails |
| 🔭 Watchtower | Pipeline health and alert monitoring |
| 🏆 Milestones | Revenue and client goal tracker |
| ⚙️ Settings | System config and agent toggles |

---

## Tech Stack

- **Frontend:** React · HTML · CSS (CDN + Babel, no build step)
- **AI:** Claude API — `claude-sonnet-4-20250514`
- **Integrations:** n8n MCP · Google Sheets MCP · Slack MCP · Gmail MCP
- **Voice:** Web Speech API (wake word + TTS response)
- **Deployment:** iPad-primary · PWA target: hq.cartiercreative.com

---

## Architecture

```
CartierHQ (React Dashboard)
       │
       ├── Claude API ──────────── Jarvis AI responses
       ├── n8n MCP ─────────────── Trigger / read workflows
       ├── Google Sheets MCP ───── Live CRM data
       ├── Slack MCP ───────────── Send alerts / messages
       └── Gmail MCP ───────────── Hermes email outreach
```

---

## Key Features

- **Voice-first design** — wake word triggers Jarvis without touching the screen
- **Live CRM sync** — leads pull directly from Google Sheets in real time
- **Agent control panel** — 11 named AI agents each with distinct roles and status
- **Hermes outreach** — cold email drafting and sending built into the dashboard
- **Milestone tracker** — revenue goals, client count, MRR progress

---

## Status

✅ Live — running daily on iPad  
🔄 In progress: Bidirectional voice mode, Supabase migration, PWA deployment

---

## Part of CartierOS

CartierHQ is the command layer that sits on top of the full [CartierOS stack](https://github.com/cartiercreative8-art/cartier-os).
