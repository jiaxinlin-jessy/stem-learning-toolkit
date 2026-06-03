# How to Install a Skill

Claude Skills extend what Claude can do in a conversation. Here's how to install one from this repo.

---

## On Claude.ai (recommended)

1. Download the `.skill` file from the [`skills/`](../skills/) folder to your computer
2. Go to [claude.ai](https://claude.ai) and sign in
3. Click your avatar (top right) → **Settings**
4. Navigate to the **Skills** tab
5. Click **Install from file** and select the `.skill` file you downloaded
6. The skill is now active — it will trigger automatically when relevant

> **Tip:** You can have multiple skills installed at once. Claude will use whichever one fits the task.

---

## Verifying it works

After installing `stem-note`, try this in a new chat:

```
Here's a short lecture excerpt. Please make study notes.

Lecture: Introduction to Eigenvalues
An eigenvalue of a matrix A is a scalar λ such that Av = λv for some 
non-zero vector v. The vector v is called the eigenvector. To find 
eigenvalues, we solve det(A - λI) = 0, known as the characteristic equation.
```

You should see structured notes with the concept, formula, and a definition block — not just a plain summary.

---

## Uninstalling

Settings → Skills → click the skill → **Remove**.

---

## Using via API

If you're building on the Claude API, skills are provided as system prompt content. Extract the `SKILL.md` from the `.skill` file (it's a zip) and include it in your system prompt.

```python
import zipfile

with zipfile.ZipFile("stem-note.skill", "r") as z:
    skill_md = z.read("SKILL.md").decode("utf-8")

# Then include skill_md in your system prompt
```
