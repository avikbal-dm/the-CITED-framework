# The CITED Master Checklist

**Get found, trusted, and cited by AI search: ChatGPT, Gemini, Perplexity, Copilot, and Google AI Overviews.**

This is the open, run-it-yourself companion to the book *CITED: The Growth Operating System for the Age of AI Search* by Avik Bal. It takes the book's master checklist and expands every item with a how-to, named tools, and a test for done, so a team can audit its whole AI-search posture in one pass and know exactly what to do next.

Search stopped being a list of links. On a growing share of queries an engine reads the web, writes one answer, and names a few sources. The prize is a citation inside that answer, and it is won differently from a ranking. CITED is the system for winning it.

---

## What is in here

```
cited-checklist/
├── checklist/                 The 26 checks, expanded, one file per layer
│   ├── C-citation-surface.md
│   ├── I-information-architecture.md
│   ├── T-technical-foundation.md
│   ├── E-evidence-rich-extraction.md
│   └── D-demand-capture.md
├── docs/
│   ├── TOOLS.md               Every tool, grouped by job, free or paid
│   ├── SCORING.md             What your score means, and the two override rules
│   └── GLOSSARY.md            Plain definitions
├── templates/
│   ├── robots-ai-crawlers.txt AI crawler allow/deny policy, ready to adapt
│   ├── llms.txt               Optional, clearly labeled as emerging
│   ├── schema/                Organization, Article, FAQ JSON-LD
│   └── tracking/              Citation and buyer-question CSV sheets
├── tool/
│   ├── index.html             Interactive self-assessment, scores you by layer
│   └── cited_checklist.py     Terminal scorer, no dependencies
└── workbook/
    ├── CITED_Checklist.xlsx   Fillable workbook with status, notes, dashboard
    └── build_workbook.py      Rebuilds the workbook from source
```

---

## The five layers

Read top to bottom, C to D. The order is a dependency: fix what blocks the engines first.

| Code | Layer | The question it answers | Checks |
|---|---|---|---|
| **C** | [Citation Surface](checklist/C-citation-surface.md) | Where do the sources engines read talk about you? | 6 |
| **I** | [Information Architecture](checklist/I-information-architecture.md) | Is your knowledge organized into retrievable units? | 5 |
| **T** | [Technical Foundation](checklist/T-technical-foundation.md) | Can bots reach, read, and parse your pages? | 5 |
| **E** | [Evidence-Rich Extraction](checklist/E-evidence-rich-extraction.md) | Is every key claim quotable, sourced, and attributed? | 5 |
| **D** | [Demand Capture](checklist/D-demand-capture.md) | Does a citation turn into measured pipeline? | 5 |

---

## Quick start

Pick one. They all cover the same 26 checks.

**Read and tick.** Start with [`checklist/`](checklist/) and work each layer in order.

**Self-assess in the browser.** Open `tool/index.html`. Tick items, watch the per-layer and overall score update, and export your result. It saves your progress in your browser, so nothing leaves your machine. Works on GitHub Pages if you publish it.

**Score in the terminal.**
```bash
python tool/cited_checklist.py          # interactive, saves progress
python tool/cited_checklist.py --report # print a scored markdown report
```

**Fill the workbook.** Open `workbook/CITED_Checklist.xlsx`. Set each row's status, add notes, and the dashboard tab scores you live.

---

## What your score means

26 checks. Your score is how many you can honestly tick. Full detail in [docs/SCORING.md](docs/SCORING.md).

| Complete | Band |
|---|---|
| 0 to 20% | Absent |
| 21 to 45% | Reactive |
| 46 to 70% | Present |
| 71 to 90% | Cited |
| 91 to 100% | Compounding |

Two rules override the raw number. If **Technical Foundation** is incomplete, fix it first, because a page a bot cannot read cannot be cited. And your **lowest layer is your next move**, because the weakest layer caps the whole system.

---

## The evidence

The why-it-matters lines are grounded, not asserted. Key figures and their sources:

- Around **68 percent** of United States Google searches were zero-click in early 2026 (SparkToro and Datos).
- Earned, third-party sources draw roughly **325 percent** more AI citations than brand-owned pages (Chen and Koudas, 2025, arXiv:2509.08919).
- Adding statistics, quotations, or cited sources raised generative visibility by **30 to 41 percent** (Aggarwal et al., GEO, ACM SIGKDD 2024, arXiv:2311.09735).
- Pages with expert quotes average **4.1** citations against **2.4** without (SE Ranking via Foglift, 2026).
- ChatGPT and Perplexity overlap on only about **11 percent** of cited domains for the same prompts (Averi and Superlines, 2026).

Full source list is in the book's evidence appendix.

---

## Contributing

AI search moves fast, so tools and crawler names go stale. Fixes are welcome. See [CONTRIBUTING.md](CONTRIBUTING.md).

## License

MIT. See [LICENSE](LICENSE). Attribution to Avik Bal is appreciated.

## About

Built by **Avik Bal**, B2B digital growth strategist.
Book: *CITED: The Growth Operating System for the Age of AI Search*.
Web: [avikbal.com](https://avikbal.com) · LinkedIn: [in/avikbal](https://www.linkedin.com/in/avikbal)

If this saved your team time, a star helps others find it.
