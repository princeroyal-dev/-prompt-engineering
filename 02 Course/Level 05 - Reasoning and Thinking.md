---
level: 5
tags: [prompt-engineering, level-5, course]
status: upcoming
---

# Level 05: Reasoning and Thinking

⬅️ [[Level 04 - Examples and Structure]] | ➡️ [[Level 06 - Reliability and Hallucinations]]

> **Goal:** Get better answers on multi-step problems (logic, math, debugging, planning) and learn to verify them.
> **Time:** 3–4 days.

---

## 🇬🇧 English

### 1. Why step-by-step helps
On multi-step problems, a model that writes out intermediate steps often does better than one forced to jump straight to the answer. The steps give it room to work.

### 2. Techniques
1. **Ask for reasoning first:** "Think step by step, then give the final answer."
2. **Separate thinking from answer** with tags so you can read the answer fast:
   ```
   Reason inside <thinking></thinking>, then give only the final result inside <answer></answer>.
   ```
3. **Decompose:** "First list what we know, then what we need, then solve."
4. **Self-check:** "Before the final answer, verify it against each requirement. List any mismatch."
5. **Ranked hypotheses (debugging):** "List 3 possible causes, most likely first, and how to test each."

### 3. Reasoning models and "thinking" modes
Some models reason internally (often called extended thinking or reasoning mode) before answering. With these, give the **goal and constraints clearly** rather than dictating every step. Over-specifying the steps can get in the way. Reasoning costs more time and tokens, so use it for hard problems, not simple ones. Behaviour varies by model; test both styles on your task.

### 4. Important caveat
Written reasoning is a useful tool, but it is **not a guaranteed true account** of how the model reached its answer. It can look convincing and still be wrong. **Always verify** the final answer (re-compute, run the code, check against the source).

### 5. Worked example (debugging)
```
I'm learning C. This program crashes with "Segmentation fault".

<code>
...paste code...
</code>
<error>
...paste exact output...
</error>

Give 3 likely causes, most likely first. For each: why it would cause this crash, and a 1-line check I can run. Do not rewrite my whole program. Then tell me which check to do first.
```

### 6. Mini-project: debugging prompt
Build a reusable debugging prompt with slots for code, error, expected behaviour, and what you already tried. It should return ranked hypotheses + a quick test for each. Try it on 2 real bugs.

### 7. Exercises
- **5.1** Take a 3-step word problem. Run it with and without "step by step". Compare.
- **5.2** Add a self-check step. Does the AI catch its own error? Try on a problem with a trap.
- **5.3** Intentionally ask a question with a wrong assumption. See if your "verify against requirements" step catches it.

### 8. Pass test ✅
- [ ] I can write a prompt that asks for reasoning, then a separate final answer.
- [ ] I verify answers independently (re-run, re-compute, check source).
- [ ] I know why over-specifying steps can hurt with reasoning models.

---

## 🇮🇳 Hinglish

### 1. Step-by-step kyu kaam karta hai
Multi-step problems mein jo model beech ke steps likhta hai, wo aksar seedha answer likhne wale se behtar karta hai. Steps usse sochne ki jagah dete hain.

### 2. Techniques
1. **Pehle reasoning maango:** "Step by step socho, phir final answer do."
2. **Thinking aur answer alag karo** tags se, taaki answer jaldi padh sako:
   ```
   Reasoning <thinking></thinking> mein likho, aur sirf final result <answer></answer> mein do.
   ```
3. **Todo:** "Pehle jo pata hai wo likho, phir kya chahiye, phir solve karo."
4. **Self-check:** "Final answer se pehle har requirement se verify karo. Koi mismatch ho to likho."
5. **Ranked hypotheses (debugging):** "3 possible causes likho, sabse likely pehle, aur har ek ko test karne ka tareeka."

### 3. Reasoning models aur "thinking" modes
Kuch models answer dene se pehle andar hi andar reason karte hain (extended thinking ya reasoning mode). Inke saath **goal aur constraints clearly** do, har step dictate mat karo. Zyada micro-manage karne se kabhi-kabhi nuksan hota hai. Reasoning mein time aur tokens zyada lagte hain, isliye mushkil problems ke liye use karo, simple ke liye nahi. Behaviour model ke hisaab se alag hota hai, isliye apne task par dono tareeke test karo.

### 4. Zaruri caveat
Likha hua reasoning ek kaam ka tool hai, lekin wo **ye guarantee nahi deta** ki model ne asal mein aise hi socha. Wo convincing dikhkar bhi galat ho sakta hai. Final answer ko **hamesha verify** karo (dobara calculate karo, code run karo, source se match karo).

### 5. Worked example (debugging)
Upar English mein wala prompt copy karo aur apna code/error paste karo. Hinglish version bhi chalega.

### 6. Mini-project: debugging prompt
Reusable debugging prompt banao jisme code, error, expected behaviour aur "ab tak kya try kiya" ke slots hon. Ye ranked hypotheses + har ek ka quick test de. 2 asli bugs par try karo.

### 7. Exercises
- **5.1** 3-step word problem lo. "step by step" ke saath aur bina uske chalao. Compare karo.
- **5.2** Self-check step add karo. Kya AI apni galti pakadta hai? Aisi problem par try karo jisme trap ho.
- **5.3** Jaanbujhkar galat assumption wala sawal pucho. Dekho tumhara "requirements se verify" step ise pakadta hai ya nahi.

### 8. Pass test ✅
- [ ] Main aisa prompt likh sakta hoon jo pehle reasoning aur phir alag final answer maange.
- [ ] Answers ko independently verify karta hoon (re-run, re-compute, source check).
- [ ] Mujhe pata hai reasoning models ke saath steps over-specify karna kyu nuksan kar sakta hai.

➡️ Next: [[Level 06 - Reliability and Hallucinations]]
