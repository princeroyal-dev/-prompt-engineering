---
level: 7
tags: [prompt-engineering, level-7, course]
status: upcoming
---

# Level 07: Chaining and Complex Tasks

⬅️ [[Level 06 - Reliability and Hallucinations]] | ➡️ [[Level 08 - System Prompts and Apps]]

> **Goal:** Split big jobs into steps, where each step has one clear job and passes its result to the next.
> **Time:** 4–5 days.

---

## 🇬🇧 English

### 1. One prompt = one job
When a single prompt asks for research + writing + formatting + checking, quality drops and it is hard to debug. Splitting into a **chain** makes each step simpler and testable.

### 2. Common chain patterns

| Pattern | Steps |
|---|---|
| Write & improve | Outline → Draft → Critique against checklist → Revise |
| Extract & transform | Extract facts → Clean/normalize → Format as table/JSON |
| Classify & route | Classify the request → Use a different prompt per class |
| Generate & verify | Generate answer → Separate prompt checks it against the source |

Diagram: [[Diagrams]] (section 7).

### 3. Passing data between steps
Use tags: put step 1's output inside `<outline>…</outline>` in step 2's prompt. Say exactly what to do with it ("expand each bullet into one paragraph").

### 4. Add gates
Between steps, check: is the output in the right format? Is anything missing? You can do this by eye, with a small script, or with a "checker" prompt.

### 5. When NOT to chain
Simple tasks. Chains add time, cost and more places to fail. Start with a single good prompt. Chain only when a single prompt keeps failing on a specific part.

### 6. Manual chain (no code needed)
You can run a chain by hand in a chat: copy each output into the next prompt. Later (Level 8–10) you can automate it with code.

### 7. Note on "prefill"
Some APIs let you start the assistant's reply to force a format (e.g., begin with `{` for JSON). Support differs by model and provider, so check the current docs before relying on it.

### 8. Mini-project: 4-step writer
Pick a topic you want to explain (for example a chapter of a beginner guide you're writing). Steps: (1) outline from your notes, (2) draft each section, (3) critique with a 5-point checklist, (4) revise. Save each prompt as a template with `{{variables}}`.

### 9. Exercises
- **7.1** Do the same task as one prompt vs a 3-step chain. Score both with your checklist.
- **7.2** Add a "checker" step that compares a draft with the source notes and lists unsupported claims.
- **7.3** Write one routing prompt that decides: "bug question / concept question / project idea", and a different template for each.

### 10. Pass test ✅
- [ ] My chain beats the single prompt on my checklist (with scores logged).
- [ ] Each step has one clear job and a defined output format.
- [ ] I can explain when a chain is *not* worth it.

---

## 🇮🇳 Hinglish

### 1. Ek prompt = ek kaam
Jab ek hi prompt research + writing + formatting + checking maangta hai, quality girti hai aur debug karna mushkil hota hai. **Chain** mein todne se har step simple aur testable ho jata hai.

### 2. Common chain patterns

| Pattern | Steps |
|---|---|
| Likho aur sudharo | Outline → Draft → Checklist se critique → Revise |
| Nikalo aur badlo | Facts extract → Clean/normalize → Table/JSON mein format |
| Classify aur route | Request classify → Har class ke liye alag prompt |
| Banao aur verify karo | Answer banao → Alag prompt source se check kare |

Diagram: [[Diagrams]] (section 7).

### 3. Steps ke beech data kaise do
Tags use karo: step 1 ka output step 2 ke prompt mein `<outline>…</outline>` ke andar rakho. Saaf bolo ki uska kya karna hai ("har bullet ko ek paragraph mein expand karo").

### 4. Gates lagao
Steps ke beech check karo: format sahi hai? Kuch missing hai? Ye aankh se, chhote script se ya "checker" prompt se kar sakte ho.

### 5. Kab chain NAHI banana
Simple tasks mein. Chain se time, cost aur fail hone ki jagah badhti hain. Pehle ek accha single prompt likho. Chain tabhi banao jab single prompt kisi specific hisse par baar baar fail ho.

### 6. Manual chain (code nahi chahiye)
Chat mein haath se chain chala sakte ho: har output ko agle prompt mein copy karo. Baad mein (Level 8–10) code se automate kar sakte ho.

### 7. "Prefill" ka note
Kuch APIs assistant ka jawab shuru karne dete hain taaki format fix ho (jaise JSON ke liye `{` se shuru). Support model aur provider ke hisaab se alag hai, isliye rely karne se pehle current docs dekho.

### 8. Mini-project: 4-step writer
Koi topic lo jo samjhana hai (jaise kisi beginner guide ka chapter jo tum likh rahe ho). Steps: (1) notes se outline, (2) har section ka draft, (3) 5-point checklist se critique, (4) revise. Har prompt ko `{{variables}}` wale template ke roop mein save karo.

### 9. Exercises
- **7.1** Ek hi task single prompt aur 3-step chain, dono se karo. Apni checklist se score karo.
- **7.2** "Checker" step add karo jo draft ko source notes se compare karke unsupported claims list kare.
- **7.3** Ek routing prompt likho jo decide kare: "bug question / concept question / project idea", aur har ek ke liye alag template.

### 10. Pass test ✅
- [ ] Mera chain meri checklist par single prompt se behtar hai (scores log ke saath).
- [ ] Har step ka ek clear kaam aur defined output format hai.
- [ ] Main bata sakta hoon ki chain kab *worth nahi* hai.

➡️ Next: [[Level 08 - System Prompts and Apps]]
