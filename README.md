# 🔬 STEM Learning Toolkit — Study with Claude

> A collection of Claude skills and guides for STEM undergraduates.  
> Upload your lecture slides. Get structured, exam-ready notes.

---

## What is this?

**STEM Learning Toolkit** is an open-source collection of [Claude Skills](https://docs.claude.com) designed for undergraduate students in science, engineering, math, and computer science.

Each skill is a plug-in for Claude that teaches it *how to think* about your study materials — not just summarize them, but organize them the way your brain actually needs: theorems separated from derivations, example problems with annotated reasoning, key formulas highlighted, and exam cues flagged.

### Current Skills

| Skill | Description | Status |
|-------|-------------|--------|
| [`stem-note`](./skills/) | Upload a lecture PDF/PPT → get structured study notes | ✅ v1.0 |
| [`stem-homework`](./skills/) | Practice Helper → Higher-Quality Exams/Assignments | ✅ v1.0 |

More coming — see [Roadmap](#roadmap).

---

## Quick Start

### 1. Install a skill

Download the `.skill` file from the [`skills/`](./skills/) folder, then install it in Claude:

1. Open [claude.ai](https://claude.ai) → **Settings** → **Skills**
2. Click **Install from file** and select the `.skill` file
3. Done — Claude now has the skill available in all your chats

### 2. Use `stem-note`

Once installed, just upload your lecture file and ask:

```
Here's my lecture on Fourier Transforms. Can you make study notes?
```

Claude will automatically apply the `stem-note` skill and return structured notes with:
- Core concepts and definitions
- Key theorems and proofs
- Worked examples with annotated reasoning
- Exam tips and common pitfalls
- A summary cheat sheet at the end

### Supported file types
PDF, PPTX, DOCX, plain text. Images (scanned slides) work too, though text-based files give better results.

---

## Skills

### `stem-note` — Lecture Note Organizer

> **Best for:** Any STEM lecture with theory, proofs, and worked examples

What it does:
- Detects the subject domain (math, physics, CS, engineering, chem/bio) and adjusts note structure accordingly
- Separates **concepts** from **derivations** from **examples** — no more wall-of-text summaries
- Flags exam-relevant content with ⚠️ markers
- Outputs clean Markdown you can paste into Obsidian, Notion, or any note app
- Handles LaTeX-style math notation in output

**Install:** [`skills/stem-note.skill`](./skills/stem-note.skill)

---

## Guides

| Guide | Description |
|-------|-------------|
| [How to install a skill](./guides/install-skill.md) | Step-by-step for Claude.ai and Claude API |
| [Prompting tips for STEM notes](./guides/prompting-tips.md) | Get better notes with small prompt tweaks |
| [Contributing a skill](./guides/contributing.md) | How to add your own skill to this repo |

---

## Roadmap

### v1.x — Note-taking
- [x] `stem-note` — lecture → structured notes
- [ ] `stem-note` v1.1 — multi-lecture synthesis (combine a whole week's lectures)
- [ ] `stem-note` v1.2 — bilingual output support (EN/ZH)

### v2.0 — Active Recall
- [ ] `stem-quiz` — auto-generate practice questions from notes
- [ ] `stem-flashcard` — Anki-compatible flashcard export
- [ ] `stem-explain` — "explain this concept to me like I'm a first-year"

### v3.0 — Problem Solving
- [ ] `stem-solver` — walk through problem sets step-by-step
- [ ] `stem-checker` — upload your solution, get feedback
- [ ] `stem-similar` — find analogous example problems

### Long-term ideas
- Subject-specific skill variants (`stem-note-circuits`, `stem-note-orgo`, ...)
- Integration with Obsidian plugin
- CLI wrapper for batch processing a whole semester's slides

> Have an idea? [Open an issue](../../issues/new?template=feature_request.md) or start a [Discussion](../../discussions).

---

## Contributing

Contributions are very welcome — especially if you're a STEM student with real lecture materials to test against.

**Ways to contribute:**
- 🐛 [Report a bug](../../issues/new?template=bug_report.md) — skill gave bad output on your lecture
- 💡 [Request a feature](../../issues/new?template=feature_request.md) — something you wish Claude could do
- 🛠️ [Submit a skill](./guides/contributing.md) — built your own? Open a PR
- 📚 Add example lectures to [`examples/`](./examples/) for testing

Please read [CONTRIBUTING.md](./CONTRIBUTING.md) before submitting a PR.

---

## License

MIT — free to use, modify, and redistribute. See [LICENSE](./LICENSE).

---

<p align="center">
  Made for students, by students &nbsp;·&nbsp; 
  <a href="../../discussions">Join the discussion</a> &nbsp;·&nbsp;
  <a href="../../issues">Report an issue</a>
</p>
