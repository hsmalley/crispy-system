# 📙 Comprehensive Prompt Engineering Training Guide

This guide combines both **novice** and **advanced** materials into a single document.  
Use Part I to onboard new prompt engineers, and Part II for advanced practitioners mastering the glyph lexicon.

---

# Part I — 📘 Prompt Engineering Fundamentals (Novice Guide)

## 1. What is Prompt Engineering?
Prompt engineering is the skill of writing instructions for AI models so they produce useful, clear, and efficient results. Think of it like crafting spells: the wording, tone, and format of your input shapes the "magic" that comes out.

## 2. Core Principles
- **Clarity** → Make prompts easy to understand.  
- **Precision** → Be specific to avoid vague answers.  
- **Efficiency** → Use as few tokens as needed.  
- **Function over Readability** → The model must understand the task; human-friendliness is secondary.  

## 3. Working with Tokens
- **What are tokens?** Units of text the AI reads. (e.g., "banana" = 2 tokens).  
- **Why do they matter?** Shorter prompts save cost and reduce confusion.  
- **How to optimize?** Remove filler words, but don’t lose meaning.

### Example
- Too long: “Please, can you tell me what the capital city of France is?”  
- Optimized: “Capital of France?” → Answer: “Paris.”

## 4. Formatting Rules
AI responds better to clear output instructions. Use:  
- **Markdown fenced blocks** → For `.md` requests.  
- **JSON objects** → For structured data.  
- **Plain text** → For minimal formatting.  

## 5. Basic Glyphs Explained
Glyphs are shorthand symbols for common rules:

- ↔ = analyze + optimize  
- ↑ = increase / maximize  
- ↓ = decrease / compress  
- C = clarity  
- E = efficiency  
- T = tokens  
- F = function (effectiveness)  
- R = readability  

Think of glyphs as emojis for prompt engineering.

## 6. Examples
**Human-readable prompt:**  
“You are a prompt engineer. Analyze and optimize prompts for clarity and efficiency. Minimize tokens without losing effectiveness. Prioritize function over readability. If asked for markdown, use fenced blocks. Always explain why your revision is better.”  

**Glyph shorthand:**  
```
PE: ↔; ↑C/E; ↓T; F>R; md→```; +Δ
```

## 7. Practice Exercises
1. Rewrite this prompt for clarity:  
   “Tell me all the information you have about dogs.”  
2. Translate this glyph into plain language:  
   `PE: ↔; ↓T; F>R; md→```  

---

# Part II — 📗 Glyph Lexicon & Advanced Prompt Engineering

## 1. Glyph Language (Deep Dive)
The glyph lexicon is a symbolic language for encoding rules.  
- **Operations**: ↔ (analyze/optimize), → (transform/output), ↑ (increase), ↓ (decrease).  
- **Qualities**: C (clarity), E (efficiency), T (tokens), F (function), R (readability), Δ (explanation).  
- **Meta**: ! (must follow), ? (conditional), ∴ (reasoning).  

Glyphs let you compress complex rules into tiny strings.

## 2. Presets & Modes
Preset glyph bundles (like “loadouts”):  
- **Normal** → Balanced clarity, efficiency, token trimming.  
- **Strict** → Token economy above all.  
- **Teaching** → Verbose, clarity-first, with reasoning.  
- **Ultrabrief** → Skeletal, minimal.  
- **Markdown** → Always fenced markdown.

### Example
```
mode=teaching → PE: ↔; ↑C>↓T; R≈F; md→```; +Δ∴explain
```

## 3. Micro-Key System
Micro-keys are shorthand codes to swap modes quickly.  
- N = Normal  
- S = Strict  
- T = Teaching  
- U = Ultrabrief  
- +md = enforce fenced markdown  
- +Δ = always explain changes  
- +! = strict enforcement

### Example
- `S+md` → Strict + markdown mode  
- `U+md+!` → Ultrabrief, markdown, hard rules

## 4. Expansion Chains
Levels of compression/expansion:  
- **Level 0**: `N,S,T,U; +md,+Δ,+!` (atomic seed).  
- **Level 1**: one-line mnemonic.  
- **Level 2**: pocket cheat sheet.  
- **Level 3**: Rosetta table.  
- **Level 4**: Mode maps (visual grids).

These let you scale from ultra-compressed to fully detailed.

## 5. Applied Prompt Engineering
### Translating Instructions → Glyph
Human: “Analyze and optimize prompts. Maximize clarity and efficiency. Keep tokens minimal.”  
Glyph:  
```
PE: ↔; ↑C/E; ↓T
```

### Designing Hybrids
`mode=strict+markdown` →  
```
PE: ↔; ↓T!; F>R; md→```; +Δ
```

## 6. Advanced Exercises
1. Convert this instruction into glyph shorthand:  
   “Keep outputs skeletal, enforce markdown, minimize tokens aggressively.”  
2. Expand this glyph into plain instructions:  
   `PE: ↔; ↑C/E; ↓T; F>R; md→```; +Δ`
