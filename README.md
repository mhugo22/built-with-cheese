# Built with Cheese 🧀

Projects shipped with OpenClaw + Claude Sonnet.

---

## Live Projects

### SketchySkills (2025-01-21) ✅
**Security scanner for ClawHub malicious skills**

- 🌐 **Live:** https://sketchyskills.vercel.app
- 📦 **Repo:** https://github.com/mhugo22/sketchyskills
- 🔍 **What it does:** Automated security analysis of ClawHub skills - detects malware, data exfiltration, prompt injection
- 📊 **Results:** 93 skills analyzed, found HIGH severity malware in `clawhub-publish` skill
- 💰 **Cost:** $4.67 total (Claude Opus 4.6 API)
- ⏱️ **Timeline:** Idea → deployed production app in ~6 hours
- 🎯 **Key Learning:** Progressive testing (10 → 41 → 94 skills) caught issues early; exponential backoff retry logic = 88% improvement in reliability
- 🏆 **Status:** Shipped, deployed, done. No ongoing maintenance planned.

**Tech Stack:** Next.js 15, Claude Opus 4.6, Vercel, ClawHub CLI

### Gabby Gmail Monitor (2026-02-15) ✅
**Automated school/scouts email monitoring with calendar & Telegram integration**

- 📦 **Repo:** https://github.com/mhugo22/gabby-gmail (private)
- 🔍 **What it does:** Monitors a Gmail inbox for school and scouts updates, auto-categorizes emails, extracts event dates into iCloud calendar, and sends digests to a dedicated Telegram channel
- ⏱️ **Timeline:** Idea → fully automated in ~1 hour
- 🔄 **Schedule:** Runs 4x daily (7am, 1pm, 5pm, 9pm CST)
- 🏆 **Status:** Shipped, running via OpenClaw cron

**Tech Stack:** Node.js, Gmail API (OAuth 2.0), macOS Calendar (AppleScript/iCloud), Telegram, OpenClaw Cron

### Cheese Brain (2026-02-17) ✅
**DuckDB-powered knowledge management system for AI agents and humans**

- 🌐 **Repo:** https://github.com/mhugo22/cheese-brain
- 🔍 **What it does:** Sub-millisecond keyword & full-text search across 22+ entity types (projects, contacts, tools, decisions, email accounts, workflows, etc.) - designed as a persistent knowledge base for AI agents to recall context across sessions
- 📊 **Results:** 44 entities populated, <1ms search performance, 2-9x Parquet compression, automated daily backups
- ⏱️ **Timeline:** Design → production-ready in 2 days (Phase 1 complete)
- 🎯 **Key Learning:** DuckDB's native JSON/array support + FTS extension = perfect fit for unstructured knowledge bases; Pydantic v2 `@field_serializer` pattern for clean UUID/datetime serialization
- 🏆 **Status:** Shipped, production-ready, in daily use

**Tech Stack:** Python 3.11+, DuckDB 1.4.4+, Pydantic v2, Click CLI, pytest, OpenClaw Cron (backups)

---

## What is this?

This repo tracks projects built collaboratively with **Cheese** (AI assistant) via **OpenClaw** (autonomous AI framework).

Each project includes:
- Live demo link (when applicable)
- Source repo
- Build timeline & cost
- Key technical wins/learnings
- Current status

---

## Stats

- **Projects shipped:** 3
- **Total cost:** $4.67 + minimal (Gabby Gmail, Cheese Brain)
- **Fastest ship:** ~1 hour (Gabby Gmail)
- **Lines of code written:** ~3,500+ (estimated)

---

## About

**Matt Hugo** - Builder, experimenter, "search guy"  
**Cheese** - Snarky AI assistant with access to too many tools  
**OpenClaw** - Open-source autonomous AI framework ([openclaw.ai](https://openclaw.ai))

---

*Last updated: 2026-02-17*
