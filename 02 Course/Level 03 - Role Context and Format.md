---
level: 3
tags: [prompt-engineering, level-3, course]
status: next
---

# Level 03: Role, Context and Format

⬅️ [[Level 02 - Clarity and Specificity]] | ➡️ [[Level 04 - Examples and Structure]]

> **Goal:** Control who the AI "is", what it knows about your situation, and the exact shape of its output.
> **Time:** 3–4 days.

---

## 🇬🇧 English

### 1. Role (persona)
"You are a patient C tutor for a beginner" sets tone, focus and depth. **Honest limit:** a role changes style and focus; it does not add knowledge the model lacks. Don't expect "act as a genius" to make answers more correct.

### 2. Context = facts the model cannot guess
Give: your level, what you tried, error messages, the code, constraints, the goal. Paste real material instead of describing it vaguely.

### 3. Format control
Tell it the shape: headings, bullets, table with named columns, JSON with named fields, word limits, order of sections. Best trick: **give a skeleton** of the output.

```
Output format:
## Concept (2 sentences)
## Analogy (1 sentence)
## Code (max 10 lines, commented)
## Common mistakes (3 bullets)
## Quiz (2 questions, answers at the end)
```

### 4. Tone and length
"Friendly but precise", "formal email, 120 words", "explain like I'm 12" all work. Put hard limits as numbers.

### 5. The ROLE / TASK / CONTEXT / CONSTRAINTS / FORMAT template

```
ROLE: [who the AI should be]
TASK: [one clear job]
CONTEXT: [my level, background, material]
CONSTRAINTS: [length, tone, what to avoid, what to do if unsure]
OUTPUT FORMAT: [skeleton or fields]
```

More in [[Anatomy and Master Template]].

### 6. Mini-project: "AI tutor" prompt
Write a reusable prompt for a topic you are learning (e.g., C pointers, Docker volumes). Output must always have the same 5 sections (Concept, Analogy, Code, Mistakes, Quiz). Test it on 3 different topics. The format should stay the same each time.

### 7. Exercises
- **3.1** Ask the same question with 3 different roles (teacher, interviewer, reviewer). Note how tone and depth change.
- **3.2** Ask for the same content as: (a) bullets, (b) table, (c) JSON. Which suits which job?
- **3.3** Do the mini-project above.

### 8. Pass test ✅
- [ ] My tutor prompt gives the same section structure on 3 different topics.
- [ ] I can explain what a role can and cannot do.
- [ ] I give real context (code/errors/level), not only descriptions.

---

## 🇮🇳 Hinglish

### 1. Role (persona)
"Tum ek patient C tutor ho jo beginner ko sikha raha hai" se tone, focus aur depth set hota hai. **Honest limit:** role style aur focus badalta hai, wo knowledge add nahi karta jo model ke paas nahi hai. "Genius ban jao" bolne se answers zyada sahi nahi ho jate.

### 2. Context = wo facts jo model guess nahi kar sakta
Do: tumhara level, kya try kiya, error messages, code, constraints, goal. Describe karne ki jagah asli material paste karo.

### 3. Format control
Shape batao: headings, bullets, named columns wali table, named fields wala JSON, word limit, sections ka order. Best trick: output ka **skeleton** de do.

```
Output format:
## Concept (2 sentences)
## Analogy (1 sentence)
## Code (max 10 lines, commented)
## Common mistakes (3 bullets)
## Quiz (2 questions, answers end mein)
```

### 4. Tone aur length
"Friendly but precise", "formal email, 120 words", "aise samjhao jaise main 12 saal ka hoon", ye sab kaam karte hain. Hard limits numbers mein likho.

### 5. ROLE / TASK / CONTEXT / CONSTRAINTS / FORMAT template

```
ROLE: [AI kaun bane]
TASK: [ek clear kaam]
CONTEXT: [mera level, background, material]
CONSTRAINTS: [length, tone, kya avoid karna, pata na ho to kya karna]
OUTPUT FORMAT: [skeleton ya fields]
```

Aur detail: [[Anatomy and Master Template]].

### 6. Mini-project: "AI tutor" prompt
Jo topic seekh rahe ho (jaise C pointers, Docker volumes) uske liye reusable prompt likho. Output mein hamesha wahi 5 sections hon (Concept, Analogy, Code, Mistakes, Quiz). 3 alag topics par test karo. Format har baar same rehna chahiye.

### 7. Exercises
- **3.1** Ek hi sawal 3 alag roles (teacher, interviewer, reviewer) ke saath pucho. Tone aur depth ka farq likho.
- **3.2** Ek hi content (a) bullets, (b) table, (c) JSON mein maango. Kaun sa kis kaam ke liye theek hai?
- **3.3** Upar wala mini-project karo.

### 8. Pass test ✅
- [ ] Mera tutor prompt 3 alag topics par same section structure deta hai.
- [ ] Main bata sakta hoon ki role kya kar sakta hai aur kya nahi.
- [ ] Main real context (code/errors/level) deta hoon, sirf description nahi.

➡️ Next: [[Level 04 - Examples and Structure]]
