# 🌈🎭 Chapter 3: Framing, Context & Role Mastery 🎭🌈

Prompts are not just *what* you ask, but *how you frame it*.  
Framing, roles, and narrative positioning radically change the behavior of an LLM.  
This chapter is about learning to wear masks, set the stage, and wield context like a playwright directing an actor. 🎬✨

---

# 🖼️ 3.1 The Power of Framing

Framing = how you **position the request**.  
The same task, framed differently, yields wildly different results.  

### Example: Quantum Physics  
- 🏛️ “Explain quantum physics.” → Dry textbook prose.  
- 🧒 “Explain quantum physics to a 12-year-old.” → Playful, simple.  
- 👨‍🔬 “You are Richard Feynman. Explain quantum physics.” → Wit, analogies, storytelling.  

🌈 Wizard Note: *The frame is the lens. Change the lens, change the picture.*  

---

# 🎭 3.2 Role Mastery

Roles tell the model **who it is pretending to be**.  
LLMs are improv actors — give them a mask, and they embody it.  

- 🎓 `role:teacher` → patient, step-by-step.  
- ⚖️ `role:lawyer` → formal, cautious.  
- 👩‍🍳 `role:chef` → recipe focus.  
- 🧙 `role:wizard` → flowery, archaic tone.  

### Example Prompt  
“You are a pirate bard. Write a ballad about space travel.”  

🌈 Glyph:  
```
role:pirate_bard; poem:ballad→space_travel
```

---

# 🏗️ 3.3 Context Setting

Models forget easily. Context = **scaffolding** for memory.  

- 🪢 **Background info**: supply key facts.  
- 🎨 **Style guides**: show examples of desired output.  
- 📏 **Constraints**: reinforce rules.  

### Example  
```
Context: You are drafting product descriptions for eco-friendly shoes. 
Style: Concise, persuasive. 
Task: Write 3 bullet points.
```

Glyph:  
```
context:eco_shoes; style:concise+persuasive; md:list3
```

---

# 🔄 3.4 Role + Context Fusion

Combine masks + stage directions.  

Example:  
```
role:professor; context:ancient_Rome; task=lecture→engineering
```

= Formal lecture on Roman aqueducts.  

---

# 💀 3.5 Failure Autopsies

### Failure 1 — Role Drift  
❌ Model forgets it’s a chef after 3 turns.  
Cause: role not reinforced.  
✅ Fix: reassert role instructions.  

### Failure 2 — Context Overload  
❌ Too many irrelevant details = confusion.  
✅ Fix: trim to essentials.  

### Failure 3 — Ambiguous Role  
❌ “Be a critic.” But critic of what?  
✅ Fix: specify: film critic, art critic, policy critic.  

---

# 🧪 3.6 Labs & Solutions

### Lab 1 — Role Variations  
Task: Explain blockchain as…  
- Scientist → technical.  
- Teacher → step-by-step.  
- Comedian → jokes.  

---

### Lab 2 — Context Anchoring  
Task: Summarize Hamlet for “business executives.”  
Expected: themes = leadership, indecision, risk.  

---

### Lab 3 — Role Persistence  
Task: Stay in “chef” role across 3 turns.  
Fix: repeat role reminders.  

---

# 📚 3.7 Case Studies

### A. RPG GM Role  
Prompt: “You are a dungeon master. Narrate a battle.”  
- Output = rich, dramatic, interactive tone.  

### B. Policy Advisor Role  
Prompt: “You are a UN policy advisor. Summarize climate risks.”  
- Output = diplomatic, cautious.  

### C. Startup Coach Role  
Prompt: “You are a VC coach. Critique this pitch.”  
- Output = critical but encouraging.  

---

# 🔤 3.8 Glyphs for Role & Context

- 🎭 **Role**: `role:X`  
- 🏛️ **Context**: `context:Y`  
- 🎨 **Style**: `style:Z`  
- 🔀 **Fusion**: `role+context+style; task`  

🌈 Example:  
```
role:scientist; context:space_exploration; style:concise; md:list5
```

---

# 🧱 3.9 Capstones

1. **Multi-Role Task** — Generate startup pitch, critique it as: investor, customer, regulator.  
2. **Context Rewrite** — Take 1 essay. Rewrite for: child, CEO, activist, historian.  
3. **Glyph Translation** — Compress verbose role+context prompts into glyph shorthand.  

---

# 🌈 Chapter 3 Summary 🌈

- 🖼️ Framing reshapes the **lens of output**.  
- 🎭 Roles = masks the model wears.  
- 🏗️ Context = scaffolding for memory.  
- 💀 Failures often = role drift, overload, ambiguity.  
- 🌈 Glyphs compress role, context, style into shorthand.  

🎓 With framing and roles, you stop asking questions… and start **directing AI as your actor**.  
The next chapters deepen your stagecraft until you command full plays with automated casts. 🎭🔥🌟  
