# Contributing to STEM Learning Toolkit

Thanks for wanting to contribute! This project is community-driven — the more subject areas and real lecture materials we cover, the better it works for everyone.

---

## How to contribute a skill

A Claude skill is a `.skill` file (which is a zipped folder containing a `SKILL.md` and optional supporting files). If you've built one, here's how to get it into this repo:

1. Fork the repository
2. Add your `.skill` file to the `skills/` directory
3. Add a row to the skills table in `README.md`
4. Open a Pull Request with:
   - A short description of what the skill does
   - At least one example input + output (can be anonymized lecture content)
   - Which STEM subjects you've tested it on

### Skill quality bar

Before submitting, please check:
- [ ] Skill handles at least two STEM domains (e.g. math + CS, or physics + engineering)
- [ ] Output is clean Markdown with correct math notation
- [ ] Tested on at least 3 different real lecture files
- [ ] No hardcoded assumptions about a single course or professor's style

---

## How to report a bug

Use the [bug report template](../../issues/new?template=bug_report.md). Include:
- Which skill you used
- What file type (PDF / PPTX / etc.)
- What the output looked like vs. what you expected
- Attach the lecture file if you can (or a public equivalent)

---

## How to suggest a feature

Use the [feature request template](../../issues/new?template=feature_request.md). Be specific about the use case — "I want a skill that does X when I upload Y" is more useful than "make it smarter."

---

## Adding example lectures

The `examples/sample-lectures/` folder is for anonymized or public-domain lecture materials used for testing. Good examples:
- MIT OpenCourseWare materials (openly licensed)
- Your own lecture notes (with identifying info removed)
- Any CC-licensed academic slides

---

## Code of conduct

Be kind. This is a tool for students — many contributors will be undergrads learning to code and collaborate for the first time. Constructive feedback only.
