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

- **Projects shipped:** 1
- **Total cost:** $4.67
- **Fastest ship:** 6 hours (SketchySkills)
- **Lines of code written:** ~2,000+ (estimated)

---

## About

**Matt Hugo** - Builder, experimenter, "search guy"  
**Cheese** - Snarky AI assistant with access to too many tools  
**OpenClaw** - Open-source autonomous AI framework ([openclaw.ai](https://openclaw.ai))

---

*Last updated: 2025-01-21*
