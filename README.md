# AI Sentia — Global AI Intelligence Dashboard

> *sentia (sen-tee-uh) • awareness*

A free, real-time AI news aggregator that monitors 35+ global sources daily, filters noise using LLMs, and surfaces what actually matters in AI.

🌐 **Live Dashboard:** [aisentia.pages.dev](https://aisentia.pages.dev)
📩 **Daily Newsletter:** [AI Daily Signal on Substack](https://aiforanalyticsandads.substack.com/s/ai-daily-signal)

---

## What It Does

Every day while your LinkedIn feed is flooded with the same viral AI story told 10 different ways, AI Sentia quietly monitors 35+ global sources and shows you everything else that happened.

- Aggregates 35+ sources across Big Tech, Research, Healthcare, Legal, YouTube and GitHub
- Uses Google Gemini LLMs to filter non-AI content automatically
- Routes every story to the right audience (Developer, Researcher, Enterprise, Healthcare, Startup and more)
- Shows trending signals using the Hacker News gravity formula
- Rebuilds automatically every 24 hours via GitHub Actions
- Zero hosting cost — Cloudflare Pages + GitHub Actions

---

## Sources Covered

| Category | Sources |
|---|---|
| Big Tech | OpenAI, Anthropic, Google DeepMind, Meta AI, NVIDIA, Microsoft Research, AWS, Apple ML |
| Research | ArXiv AI, MIT, Stanford, Berkeley, Hugging Face, DeepLearning.AI |
| YouTube | Andrej Karpathy, Two Minute Papers, AI Explained, Fireship |
| Startup & VC | Y Combinator, Sarvam AI, Synced, TII Falcon |
| Developer | GitHub Trending, PyTorch, LangChain |
| Healthcare | NEJM AI, STAT News, MobiHealthNews, Healthcare IT |
| Legal & Policy | Artificial Lawyer, Legal Dive, ABA Journal |
| News | TechCrunch AI, VentureBeat, The Verge AI, Wired AI |

---

## Tech Stack

- **Python** — RSS parsing, GitHub API, YouTube Data API, ArXiv API
- **Google Gemini** — LLM filtering, summarisation, persona routing
- **GitHub Actions** — daily automation, zero infrastructure
- **Cloudflare Pages** — free static hosting, global CDN
- **Alpine.js** — reactive UI without a build step
- **Tailwind CSS** — responsive design

---

## How It Works

```
GitHub Actions (daily cron)
    ↓
daily_build.py fetches 35+ sources
    ↓
Deduplication (URL + title similarity)
    ↓
Google Gemini filters non-AI content
    ↓
Gemini enriches: summary + persona + CTA
    ↓
Saves to database.json
    ↓
Cloudflare Pages auto-deploys
    ↓
Newsletter generated → Substack
```

---

## Personas

Every story is routed to one of 8 audience personas:

- 💻 Developer
- 💼 Enterprise
- 🔬 Research
- 🚀 Startup
- 🎨 Creator
- 📚 Education
- 🏥 Healthcare
- ⚖️ Policy & Law

---

## Newsletter

Subscribe to **AI Daily Signal** — the last 24 hours of AI news delivered to your inbox every morning, organised by audience.

[Subscribe on Substack](https://aiforanalyticsandads.substack.com/s/ai-daily-signal)

---

## Feedback & Feature Requests

Found a bug or want a new source added? [Submit feedback here](https://tally.so/r/lbyYXX)

---

*Built for myself. Shared for everyone. Free forever.*# aisentia-site
