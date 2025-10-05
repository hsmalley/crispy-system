# 🌈✍️ Chapter 2: Language, Framing, and Instruction Design ✍️🌈

Prompts live and die by **language**.  
The same idea, framed differently, can summon brilliance — or babble.  
This chapter teaches you the **art of framing**, **clarity of instruction**, and the hidden **psychology of word choice**.  

---

## 2.1 Why Language Matters
- 🗣 Words carry frames → subtle cues guide model behavior.  
- ⚖️ Precise language = reproducibility.  
- 🎭 Tone shifts outputs (polite vs blunt vs formal).  

🌈 Wizard Note: *Language is not neutral. Every word is a spell that frames a world.*  

---

## 2.2 Framing Effects  
- Frame A: “Explain simply.” → Child-level.  
- Frame B: “Explain concisely.” → Professional summary.  
- Frame C: “Explain like a professor.” → Dense academic tone.  

---

## 2.3 Failures in Framing
- ❌ Ambiguity → inconsistent outputs.  
- ❌ Overloaded prompts → confusion.  
- ❌ Cultural mismatch → irrelevant tone.  

✅ Fix with explicit framing:  
```
frame:clear{tone=professor, scope=concise}
```  

---

## 2.4 Labs

**Lab 1: Rewrite Ambiguity**  
Broken: “Explain this.” → vague.  
Fix: “Explain to a 5-year-old, using analogies.”  

**Lab 2: Tone Shifting**  
Input → write in formal tone vs casual tone. Compare.  

**Lab 3: Multilingual Framing**  
Prompt in English vs Spanish → analyze cultural shifts.  

---

## 2.5 Case Studies
- Writing assistants.  
- Multilingual tutors.  
- UX copywriters.  

---

## 2.6 Capstones
- Cross-cultural instructional prompts.  
- Multilingual optimization system.  
- Style-shifting assistants.  

---

# 🌈🎭 Chapter 3: Modes of Prompting — Creative, Technical, Reflective 🎭🌈

Prompts come in **modes**, each shaping the model’s “mindset.”  

---

## 3.1 Modes
- 🎨 Creative (`mode:creative`) → stories, poems, art.  
- 💻 Technical (`mode:technical`) → coding, math.  
- 🔍 Reflective (`mode:reflective`) → analysis, critique.  
- 🧪 Evaluative (`mode:evaluative`) → checklists, rubrics.  

---

## 3.2 Failures
- ❌ Mode drift: starts technical → ends creative.  
- ❌ Tone mismatch: legal doc in poetic mode.  

✅ Fix: lock modes explicitly.  
```
mode:technical; style=formal
```  

---

## 3.3 Labs
- Input: “Explain quantum computing.” Run in all modes. Compare.  
- Lab: Create hybrid mode (`creative+technical`).  

---

## 3.4 Case Studies
- Poetry vs Legal Docs.  
- RPG GM vs QA Engineer.  

---

## 3.5 Capstones
- Build hybrid prompts (creative+technical).  
- Create “AI Mood Boards” mixing styles.  

---

# 🌈⚙️ Chapter 4: Advanced Prompt Structures & Strategies ⚙️🌈

Now we go **beyond basics**: scaffolding, roles, and world simulations.  

---

## 4.1 Advanced Structures
- **System prompts**: define high-level behavior.  
- **Role prompts**: “You are a GM.”  
- **Scaffolds**: multi-step structured templates.  

🌈 Glyphs:  
```
role:system; scaffold:multi{outline→essay}
simulate:world{RPG}
```  

---

## 4.2 Failures
- ❌ Prompt bloat → brittle.  
- ❌ Over-constraint → stifled creativity.  
- ❌ Conflicting roles.  

---

## 4.3 Labs
- Build multi-step scaffold for essays.  
- Debug bloated prompts → simplify.  
- RPG GM prompt → debug contradictions.  

---

## 4.4 Case Studies
- Long-form research writers.  
- Simulation GMs.  
- Corporate report templates.  

---

## 4.5 Capstones
- Build simulation prompts.  
- Full role-play pipelines.  
- Hybrid worldbuilders.  

---

# 🌈🧪 Chapter 5: Evaluation, Testing & Debugging Prompts 🧪🌈

No discipline is complete without **testing**.  
This chapter turns you into a **prompt debugger**.  

---

## 5.1 Why Evaluation Matters
- Ensures **quality + reliability**.  
- Builds **trust**.  
- Enables **scaling**.  

---

## 5.2 Evaluation Techniques
- Rubrics.  
- Checklists.  
- Benchmarks.  

🌈 Glyph:  
```
eval:rubric{clarity,accuracy}
checklist{bias,safety,scope}
```  

---

## 5.3 Failures
- ❌ Hallucination.  
- ❌ Drift.  
- ❌ Overconfidence.  

---

## 5.4 Labs
- Evaluate essay output with rubric.  
- Debug hallucinated fact.  
- Build checklist for tone + safety.  

---

## 5.5 Case Studies
- QA bots.  
- Tutors.  
- Safety evaluators.  

---

## 5.6 Capstones
- Design debugging pipeline.  
- Build reflection + evaluation loop.  
- QA system for RPG campaigns.  

---
