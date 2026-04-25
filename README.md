# Content Engine — AI-Powered Skill Graph

A folder of 17 interconnected markdown files that replaces a content team. One topic in → 10 platform-native posts out.

> **Credit:** This system is based on the full breakdown by [@DeRonin_](https://x.com/DeRonin_/status/2042604279077237170). All file structures, workflows, and concepts originate from that post.

> **AI agents:** Skip this file. Start at [`index.md`](./index.md) — that is the command center, node map, and execution instructions for this system.

---

## How It Works

Instead of giving an AI a blank prompt, you give it a **skill graph** — a network of linked `.md` files that encode your brand voice, audience, platform rules, hook formulas, and repurposing logic. When you point Claude (or any AI) at this folder and give it a topic, it reads the connected nodes and produces platform-native content before writing a single word.

The key distinction: each platform version **rethinks** the topic — different angle, hook, tone, and format — not just reformatted text.

---

index.md — the entry point. The briefing document your AI agent reads first. Most important file in the entire system
platforms/ — one file per platform with the rules, format, character limits, posting frequency, content style. Everything the agent needs to write NATIVELY for that platform
voice/ — your brand voice DNA and how it adapts per platform. This is what stops your content from sounding like a robot generated it
engine/ — the operational backbone. Hook formulas, the repurposing chain, scheduling rules, content type definitions
audience/ — who you're actually talking to. Different audience segments get different angles on the same topic

---

## Structure

```
content-engine/
├── index.md                  ← command center, start here
├── platforms/
│   ├── x.md
│   ├── linkedin.md
│   ├── instagram.md
│   ├── tiktok.md
│   ├── youtube.md
│   ├── threads.md
│   ├── facebook.md
│   └── newsletter.md
├── voice/
│   ├── brand-voice.md        ← your content DNA
│   └── platform-tone.md     ← how voice adapts per platform
├── engine/
│   ├── hooks.md              ← scroll-stopping opener formulas
│   ├── repurpose.md          ← 1 idea → 8 platform posts chain
│   ├── scheduling.md         ← posting calendar + best times
│   └── content-types.md     ← format definitions
└── audience/
    ├── builders.md
    └── casual.md
```

---

## Setup

**Step 1 — Fill in your identity (required before anything works)**

Open `index.md` and update:
- `Brand:` your name or brand
- `Niche:` your specific topic area

Open `voice/brand-voice.md` and write your core personality (3-5 sentences). This is the most important file in the system.

**Step 2 — Choose how to run it**

**Option A: Claude Projects (recommended)**
1. Create a new Project in Claude
2. Upload all 17 `.md` files into the project knowledge base
3. Give it a topic and Claude reads the full graph automatically

**Option B: Paste context**
1. Copy `index.md` + `voice/brand-voice.md` into any AI chat
2. Also paste whichever platform files you need
3. Give a topic and ask it to follow the execution instructions in `index.md`

**Option C: Claude Code / Cursor (most powerful)**
1. Point the agent at this local folder
2. It reads and follows wikilinks directly from the file system
3. It can also update `hooks.md` with new winners over time

---

## Usage

Give the AI a topic and it will:
1. Check niche alignment
2. Read `brand-voice.md` for core personality
3. Select the best hook formula from `hooks.md`
4. Follow the `repurpose.md` chain (X first, then each platform in order)
5. Output one ready-to-publish post per platform — each one rethought, not reformatted

---

## Maintenance

- **Weekly:** update `engine/hooks.md` — remove underperformers, add new winners
- **As you grow:** refine `voice/platform-tone.md` based on what sounds right
- **When ready:** add new platform files following the same structure as existing ones
