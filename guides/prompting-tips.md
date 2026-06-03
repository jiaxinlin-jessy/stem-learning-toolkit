# Prompting Tips for STEM Notes

The `stem-note` skill handles most things automatically, but small tweaks in how you prompt Claude can significantly improve the output.

---

## Basic usage

Just upload your file and say something like:

```
Here's my lecture on thermodynamics. Make study notes.
```

That's often enough. But here are ways to get more targeted output.

---

## Specify the subject area

If Claude guesses the wrong domain, just tell it:

```
This is a circuits lecture (EE). Focus on the transfer functions and 
Bode plot interpretation, not general math.
```

---

## Ask for exam focus

```
I have an exam on this in 3 days. Flag the high-yield concepts and 
any common exam traps.
```

---

## Request a specific output section

```
Skip the derivations — I just need the final formulas and one worked example per concept.
```

Or the opposite:

```
I need the full proofs, not just the results. I'm a math major.
```

---

## Multi-lecture synthesis

Once `stem-note` v1.1 is released, you'll be able to combine multiple lectures. For now, you can do it manually:

```
Here are notes from Week 3 and Week 4 [paste both]. 
Can you write a combined summary that shows how the concepts build on each other?
```

---

## Language

```
Please write the notes in Chinese (Simplified). Keep all math notation in LaTeX.
```

---

## What not to do

- Don't paste the entire lecture as plain text if you can upload the file — the file gives Claude better structure to work with
- Don't ask for "a complete rewrite of the lecture" — the skill is for *notes*, not reproductions
- Don't expect perfect LaTeX rendering in Claude.ai chat — copy to Obsidian or Overleaf for that
