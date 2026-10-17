---
level: 2
tags: [prompt-engineering, level-2, course]
status: you-are-here
---

# Level 02: Clarity and Specificity

⬅️ [[Level 01 - Foundations]] | ➡️ [[Level 03 - Role Context and Format]]

> **Goal:** Turn vague requests into measurable ones, and learn the iteration loop.
> **Time:** 3–4 days. This level gives the biggest jump: most bad outputs come from vague prompts.

---

## 🇬🇧 English

### 1. The colleague test
Show your prompt to a smart new colleague who knows nothing about your situation. If they would be confused, the model will be too. Models do not know your goals, your audience, or your preferences unless you say so.

### 2. Replace vague words with measurable ones

| Vague | Specific |
|---|---|
| "short" | "under 120 words" |
| "good code" | "readable, with comments, handles empty input, no global variables" |
| "simple" | "for a Class 10 student, no jargon, one analogy" |
| "a few examples" | "exactly 3 examples, one easy and one tricky" |

### 3. State audience and purpose
"Explain TCP" and "Explain TCP to a first-year student who will present it tomorrow" produce different answers. Say **who it is for** and **why you need it**.

### 4. Say what TO do
"Don't use bullet points" is weaker than "Write in 2 flowing paragraphs." Positive instructions are easier to follow than only prohibitions.

### 5. Order and steps
If order matters, number the steps. If the task has parts, name them (Part A, Part B) so you can point to them in follow-ups.

### 6. Let the AI ask you questions
Add: "If anything is unclear or missing, ask me up to 3 questions before answering." Great when you are not sure what the AI needs.

### 7. The iteration loop (your most important habit)
Draft → run → **diagnose** (missing context? vague? wrong format?) → change **one** thing → run again. See [[Diagrams]] (section 5).

### 8. Worked example
❌ `Make a study plan for Docker.`

✅ `Make a 7-day study plan to learn Docker basics. I know basic Linux commands but have never used containers. I can study 1 hour per day. For each day give: goal, 2 things to read or watch, 1 hands-on task, and a 2-question self-check. Output as a table with columns Day, Goal, Learn, Practice, Self-check. At the end, list 3 common beginner mistakes.`

### 9. Exercises
- **2.1** Take 5 vague prompts (write them fast, like you normally would). Make each specific using sections 2–4.
- **2.2** Pick one task. Write v1 (quick), v2 (add context), v3 (add criteria + format). Define a 5-point checklist first, then score each output.
- **2.3** Add the "ask me questions first" line to a prompt. Answer the questions, then compare with a version where you guessed.

### 10. Pass test ✅
- [ ] My v3 beats v1 on a checklist I wrote *before* running.
- [ ] I replaced at least 5 vague words with measurable ones.
- [ ] I change one thing at a time when iterating.
- [ ] I log my experiments in [[My Progress]].

---

## 🇮🇳 Hinglish

### 1. Colleague test
Apna prompt kisi smart naye colleague ko dikhao jo tumhari situation nahi jaanta. Agar wo confuse ho jaye, to model bhi hoga. Model tumhara goal, audience ya preference tab tak nahi jaanta jab tak tum bolo nahi.

### 2. Vague words ko measurable banao

| Vague | Specific |
|---|---|
| "chhota" | "120 words ke andar" |
| "accha code" | "readable, comments ke saath, empty input handle kare, global variables nahi" |
| "simple" | "Class 10 ke student ke liye, jargon nahi, ek analogy" |
| "kuch examples" | "exactly 3 examples, ek easy aur ek tricky" |

### 3. Audience aur purpose batao
"TCP samjhao" aur "TCP first-year student ko samjhao jo kal presentation dega" alag answers dete hain. Batao **kiske liye** aur **kyu chahiye**.

### 4. Kya KARNA hai wo bolo
"Bullet points mat use karo" se behtar hai "2 flowing paragraphs mein likho." Sirf mana karne se positive instruction follow karna aasan hota hai.

### 5. Order aur steps
Order important ho to steps number karo. Task ke parts ho to naam do (Part A, Part B), taaki follow-up mein point kar sako.

### 6. AI se sawal poochne do
Ye line add karo: "Agar kuch unclear ya missing ho to jawab dene se pehle mujhse max 3 sawal pucho." Jab pata na ho ki AI ko kya chahiye, tab kaam aata hai.

### 7. Iteration loop (sabse zaruri habit)
Draft → run → **diagnose** (context missing? vague? format galat?) → **ek** cheez badlo → dobara run. Diagram: [[Diagrams]] (section 5).

### 8. Worked example
❌ `Docker ka study plan banao.`

✅ `Docker basics seekhne ka 7 din ka study plan banao. Mujhe basic Linux commands aate hain par containers kabhi use nahi kiye. Roz 1 ghanta de sakta hoon. Har din ke liye do: goal, padhne/dekhne ki 2 cheezein, 1 hands-on task, aur 2 sawal ka self-check. Output table mein do: Day, Goal, Learn, Practice, Self-check. End mein beginners ki 3 common galtiyan likho.`

### 9. Exercises
- **2.1** 5 vague prompts likho (jaldi mein, jaise aadat hai). Section 2–4 se har ek ko specific banao.
- **2.2** Ek task chuno. v1 (quick), v2 (context add), v3 (criteria + format add). Pehle 5-point checklist banao, phir har output ko score karo.
- **2.3** "Pehle mujhse sawal pucho" line add karo. Sawalon ke jawab do, phir us version se compare karo jahan tumne guess kiya tha.

### 10. Pass test ✅
- [ ] Mera v3, run karne se *pehle* likhi checklist par v1 se behtar hai.
- [ ] Maine kam se kam 5 vague words ko measurable banaya.
- [ ] Iterate karte waqt ek baar mein ek hi cheez badalta hoon.
- [ ] Apne experiments [[My Progress]] mein log karta hoon.

➡️ Next: [[Level 03 - Role Context and Format]]
