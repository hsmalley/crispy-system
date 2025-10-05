# ⚡ Prompt Engineering Quick Reference Cheat Sheet

This cheat sheet is a **1-page visual reference** for prompt engineers.  
It combines the **Rosetta Table** and **Mode Map** into a compact guide.

---

## 🗝 Rosetta Table: Micro-Key → Glyph → Explanation

| Micro-Key | Glyph Seed | Explanation |
|-----------|------------|-------------|
| **N** | `PE: ↔; ↑C/E; ↓T; F>R; +Δ` | Normal mode: balanced, improves clarity & efficiency, trims tokens, explains changes. |
| **S** | `PE: ↔; ↓T!; F>R; md→\`\`\`` | Strict mode: aggressive token economy, function > readability, markdown fenced if asked, explanations optional. |
| **T** | `PE: ↔; ↑C>↓T; R≈F; md→\`\`\`; +Δ∴explain` | Teaching mode: verbose, clarity > token savings, readability balanced with function, always fenced markdown, always explains with reasoning. |
| **U** | `PE: ↔; ↓T; F>R` | Ultra-brief mode: skeletal responses, token-minimal, function prioritized. |
| **N+md** | `PE: ↔; ↑C/E; ↓T; F>R; md→\`\`\`!; +Δ` | Normal mode with fenced markdown enforced. |
| **S+md** | `PE: ↔; ↓T!; F>R; md→\`\`\`; +Δ` | Strict + markdown: token economy + guaranteed fenced markdown. |
| **T+md** | `PE: ↔; ↑C>↓T; R≈F; md→\`\`\`!; +Δ∴explain` | Teaching + markdown: verbose, clarity-first, always fenced markdown, always explains. |
| **U+md** | `PE: ↔; ↓T; F>R; md→\`\`\`!` | Ultra-brief + markdown: skeletal responses but always fenced markdown. |
| **U+md+!** | `PE: ↔; ↓T!; F>R; md→\`\`\`!` | Hardline ultrabrief: absolute token minimization, always fenced markdown. |

---

## 🗺 Mode Map (Grid View)

```
             +------------------+------------------+
             |                  |                  |
             |     Teaching     |   Teaching+md    |
             | clarity > tokens | clarity + md     |
             |                  |                  |
+------------+------------------+------------------+
|            |                  |                  |
|   Normal   |      Strict      |   Strict+md      |
| (balanced) | (token-first)    | md enforced      |
|            |                  |                  |
+------------+------------------+------------------+
|            |                  |                  |
| Ultrabrief |     Markdown     | Ultrabrief+md    |
| (skeletal) | (forced fences)  | skeletal + md    |
|            |                  |                  |
+------------+------------------+------------------+
```

---

## ⚡ Quick Use
- **Pick a base**: N (normal), S (strict), T (teaching), U (ultrabrief).  
- **Add modifiers**: `+md`, `+Δ`, or `+!`.  
- Use Micro-Key shorthand in system prompts; glyphs are canonical.  

---
