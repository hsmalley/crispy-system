# 🌈✨ Chapter 4: Formatting Magic — Forcing Structure & Shape ✨🌈

Words alone are spells — but structured words are **rituals**.  
In this chapter, you’ll learn how to force outputs into specific **formats, shapes, and containers**: Markdown, JSON, tables, XML, hybrids.  
This is the difference between vague scribbles and professional-grade artifacts.  

---

# 🎨 4.1 The Art of Structure

Formatting = control over how words appear.  
Why it matters:  
- 📖 **Humans**: clarity, readability, aesthetics.  
- 🤖 **Machines**: consistency, parse-ability, automation.  

🌟 Wizard Note: *LLMs are like clay. Without format, you get blobs. With format, you get sculptures.*  

---

# 📝 4.2 Markdown Mastery

Markdown = lightweight format loved by humans + machines.  

- Lists (`- item`, `1.`).  
- Tables (`| col1 | col2 |`).  
- Code blocks (```).  

### Case Study  
❌ **Failure:**  
Prompt: “Make a table of 3 planets.”  
Output: messy, broken pipes.  

✅ **Repair:**  
“Make a Markdown table with 3 rows: Planet, Size, Atmosphere.”  

🌈 Glyph:  
```
md:table{cols=3,rows=3,headers=[Planet,Size,Atmosphere]}
```

---

# 🗄️ 4.3 JSON Discipline

JSON = lingua franca of structured data.  

- ✅ Easy for machines to parse.  
- ⚠️ Fragile: one missing comma = invalid.  

### Common Failures  
- Trailing commas.  
- Missing brackets.  
- Wrong nesting.  

### Labs  
1. Prompt model: “Output JSON {name, hp, abilities[3]}.”  
2. Validate in a parser.  
3. Repair broken JSON.  

🌈 Glyph:  
```
json→{name,hp,abilities[3]}
```

---

# 📊 4.4 Table Wizardry

Tables = compact knowledge containers.  

### Example: NPC Roster  
Prompt: “Make a roster of 5 NPCs with Name, Role, Quirk.”  

✅ Markdown Table:  
```
| Name   | Role   | Quirk          |
|--------|--------|----------------|
| Lira   | Mage   | Speaks in song |
| Kade   | Thief  | Afraid of gold |
| Orin   | Healer | Collects rocks |
```

🌈 Glyph:  
```
md:table{rows=5,cols=3,headers=[Name,Role,Quirk]}
```

---

# 🌀 4.5 Hybrid Formats

Sometimes you need **story + data**.  

- 📖 Narrative with inline JSON.  
- 🗂️ XML tags with prose.  

### Example  
```
Story: The hero enters a cave.  
JSON: {"enemy": "goblin", "hp": 12, "loot": "dagger"}
```

🌈 Glyph:  
```
hybrid→narrative+json
```

---

# 💀 4.6 Failure Atlas

### Failure 1 — Wrong Format  
❌ Output prose instead of JSON.  
✅ Repair: Reinforce “ONLY output JSON.”  

### Failure 2 — Broken Nesting  
❌ Mismatched brackets.  
✅ Repair: Add rule “Validate JSON before answering.”  

### Failure 3 — Partial Truncation  
❌ JSON cut off mid-object.  
✅ Repair: Use shorter prompts, chunk tasks.  

---

# 🔤 4.7 Glyphs for Formatting

- 📋 Lists: `md:listN`  
- 📊 Tables: `md:table{cols,rows}`  
- 🗄️ JSON: `json→{schema}`  
- 📦 XML: `xml→{tags}`  
- 🌀 Hybrid: `hybrid→X+Y`  

🌈 Glyph Example:  
```
json→character{name,role,hp,abilities[3]}
```

---

# 🧪 4.8 Labs & Autopsies

### Lab 1: Broken JSON  
❌ Output missing comma.  
✅ Repair with validation rule.  

### Lab 2: Misaligned Table  
❌ Markdown pipes not lined up.  
✅ Add “align table correctly.”  

### Lab 3: Force XML  
Prompt: “Output character sheet in XML.”  
✅ Glyph: `xml→character{name,hp,skills[3]}`  

---

# 📚 4.9 Case Studies

### Case Study A: GM Encounter Table  
Prompt: “Generate 6 random encounters.”  
✅ Markdown table with Monster, Difficulty, Loot.  

---

### Case Study B: Resume in JSON  
Prompt: “Output resume JSON {name, skills[5], jobs[3]}.”  
✅ Machine-parseable resume.  

---

### Case Study C: API Docs Hybrid  
Prompt: “Write endpoint description + example JSON.”  
✅ Markdown section + JSON block.  

---

# 🧱 4.10 Capstones

1. **JSON Resume** — Full schema with jobs, education, skills.  
2. **GM Encounter Table** — Markdown, 10 rows, glyph shorthand.  
3. **Hybrid Story Doc** — Narrative + embedded JSON glossary.  

---

# 🌈 Chapter 4 Summary 🌈

- Formatting = ritualized control.  
- Markdown = human-friendly.  
- JSON = machine-friendly.  
- Tables = compact clarity.  
- Hybrids = story + data fusion.  
- Failures = wrong format, broken nesting, truncation.  
- Glyphs = fast shortcuts for structural magic.  

🎓 You now command the **shapes of prompts**.  
From here, you’ll learn how to chain them into **systems of spells**. 🌌✨  
