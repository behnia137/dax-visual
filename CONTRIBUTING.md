# 🤝 Contributing to DAX — Visual Edition

Thanks for wanting to help! The goal of this repo is to make DAX concepts immediately obvious to anyone — beginner or experienced analyst. Every contribution should make something clearer, not just longer.

---

## 🧭 What makes a good pattern

Each pattern file must follow the exact five-section format used throughout this repo:

```markdown
# {EMOJI} {Title}

> **🧒 Explain Like I'm 5:** {One friendly sentence analogy.}

## 🖼️ The Picture

```mermaid
...
```

{One sentence caption}

## 🔧 How it actually works

{2-3 short paragraphs, plain language, jargon explained inline}

## 🌍 Real-world example

{One concrete paragraph}

## 🔗 Related

- [Concept Name](filename.md)
```

All diagrams must use the Tailwind color palette defined in the README. No custom colors.

---

## 📁 File location and naming

- All pattern files go in the `/patterns` folder
- Use lowercase kebab-case filenames: `context-transition.md`, `selected-value.md`
- One concept per file — don't combine two unrelated functions into one file

---

## ✅ Checklist before submitting a PR

- [ ] File is in `/patterns` and named in kebab-case
- [ ] All five sections are present and in order
- [ ] The ELI5 analogy is a single sentence and uses no DAX jargon
- [ ] The Mermaid diagram uses only the four approved colors from the README palette
- [ ] "How it actually works" is 2-3 short paragraphs — not a bullet list, not a wall of text
- [ ] The real-world example is concrete (specific table names, specific numbers)
- [ ] At least one Related link points to an existing file in `/patterns`
- [ ] The README table has been updated with the new pattern in the correct section

---

## 💡 Good first additions

These patterns don't have files yet — pick one and go:

- `SWITCH` — the readable alternative to nested IF
- `IF` — conditional logic and how it interacts with BLANK
- `COALESCE` — return the first non-blank value from a list
- `EARLIER` — referencing an outer row context from inside a nested iterator
- `KEEPFILTERS` — add a filter without replacing the existing one
- `SELECTEDVALUE` — return a single selected value or a default
- `ISINSCOPE` — detect which level of a hierarchy is visible
- `HASONEVALUE` — check whether a column has exactly one value in context
- `CROSSJOIN` — combine two tables into every possible row pairing

---

## 🎨 Mermaid color palette

Use **only** these four colors:

| Role | Fill | Stroke | Text |
|------|------|--------|------|
| Blue — input / neutral | `#dbeafe` | `#3b82f6` | `#1f2937` |
| Yellow — key / central node | `#fef3c7` | `#f59e0b` | `#1f2937` |
| Green — output / positive | `#dcfce7` | `#22c55e` | `#1f2937` |
| Red — error / warning | `#fee2e2` | `#ef4444` | `#7f1d1d` |

---

## 🚀 How to submit

1. Fork the repo
2. Create a branch: `git checkout -b pattern/your-pattern-name`
3. Add your file to `/patterns`
4. Update the README table
5. Open a PR with a one-line description of what the pattern does

That's it. No tests, no build step — just markdown and diagrams.
