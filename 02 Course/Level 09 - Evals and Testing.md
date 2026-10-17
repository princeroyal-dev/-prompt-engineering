---
level: 9
tags: [prompt-engineering, level-9, course]
status: upcoming
---

# Level 09: Evals and Testing

⬅️ [[Level 08 - System Prompts and Apps]] | ➡️ [[Level 10 - Agents Context and Safety]]

> **Goal:** Choose the best prompt using evidence (scores), not feeling.
> **Time:** 1 week. This is the biggest difference between hobby and professional prompting.

---

## 🇬🇧 English

### 1. Why evals
"This feels better" is not evidence. A prompt that works on your 2 favourite examples can fail on the 3rd. And prompts can **regress** when you edit them or switch models. An **eval** is a repeatable test: fixed inputs, a scoring rule, and a score you can compare.

### 2. Build a test set
15–30 inputs is a good start:
- **Easy** cases (should always pass)
- **Hard** cases (tricky, long, ambiguous)
- **Edge** cases (empty input, wrong language, very long)
- **Adversarial** cases (inputs that try to break the format or rules)

Write the expected result or a scoring rubric *before* running.

### 3. Scoring methods
| Method | Good for | Watch out |
|---|---|---|
| Exact/programmatic check | JSON validity, labels, word limits | Only checks what you code |
| Rubric by a human (1–5 per criterion) | Writing quality, tutoring | Time-consuming; be consistent |
| LLM-as-judge (another AI scores) | Scaling rubric scoring | Can be biased (e.g., prefers longer answers); **calibrate** against your own scores on a sample |

### 4. A/B test prompts
Change one thing between versions. Run all versions on all test cases. Record score, and also **cost/latency** if relevant. Pick the winner by data. Diagram: [[Diagrams]] (section 8).

### 5. Spreadsheet layout
| Case # | Input (short) | Expected / rubric | v1 score | v2 score | v3 score | Notes |
|---|---|---|---|---|---|---|

### 6. Keep the tests
When you improve a prompt, re-run the old tests. If a previous fix broke, you caught a regression.

### 7. Mini-project
Take your Level 8 system prompt. Make 3 versions. Create 15 test cases. Score all 45 outputs with a 3-criterion rubric (correct, clear, follows format). Pick the winner and explain why.

### 8. Exercises
- **9.1** Write a rubric with 3 criteria and examples of score 1, 3, 5.
- **9.2** Score 10 outputs yourself, then have an AI score the same 10. Where do you disagree?
- **9.3** Add 3 adversarial cases to your test set.

### 9. Pass test ✅
- [ ] I have 15+ test cases with expected results or rubric.
- [ ] I compared 3 versions with scores and chose by data.
- [ ] I know the weaknesses of LLM-as-judge and checked it against my own scoring.

Further learning: Anthropic's `prompt_evaluations` course in [[GitHub Top Resources]].

---

## 🇮🇳 Hinglish

### 1. Evals kyu
"Ye behtar lag raha hai" evidence nahi hai. Jo prompt tumhare 2 favourite examples par chalta hai wo teesre par fail ho sakta hai. Aur prompt edit karne ya model badalne par **regress** (pehle se kharab) ho sakta hai. **Eval** ek repeatable test hai: fixed inputs, scoring rule, aur ek score jise compare kar sako.

### 2. Test set banao
15–30 inputs se shuru karo:
- **Easy** cases (hamesha pass hone chahiye)
- **Hard** cases (tricky, lambe, ambiguous)
- **Edge** cases (khali input, galat language, bahut lamba)
- **Adversarial** cases (aise inputs jo format ya rules todne ki koshish karein)

Run karne se *pehle* expected result ya rubric likho.

### 3. Scoring methods
| Method | Kis kaam ke liye | Dhyan rakho |
|---|---|---|
| Exact/programmatic check | JSON validity, labels, word limits | Sirf wahi check hota hai jo tumne code kiya |
| Human rubric (har criterion 1–5) | Writing quality, tutoring | Time lagta hai; consistent raho |
| LLM-as-judge (doosra AI score de) | Rubric scoring ko scale karna | Biased ho sakta hai (jaise lambe answers pasand kare); apne scores se **calibrate** karo |

### 4. Prompts ka A/B test
Versions ke beech ek cheez badlo. Saare versions saare test cases par chalao. Score likho, aur zarurat ho to **cost/latency** bhi. Data se winner chuno. Diagram: [[Diagrams]] (section 8).

### 5. Spreadsheet layout
Upar English wali table jaisa: Case #, Input, Expected/rubric, v1/v2/v3 score, Notes.

### 6. Tests rakho
Prompt improve karo to purane tests dobara chalao. Agar pichhla fix toot gaya, to regression pakda gaya.

### 7. Mini-project
Apna Level 8 system prompt lo. 3 versions banao. 15 test cases banao. 3-criterion rubric (correct, clear, follows format) se saare 45 outputs score karo. Winner chuno aur wajah likho.

### 8. Exercises
- **9.1** 3 criteria wala rubric likho, score 1, 3, 5 ke examples ke saath.
- **9.2** 10 outputs khud score karo, phir wahi 10 AI se score karwao. Kahan disagree hue?
- **9.3** Apne test set mein 3 adversarial cases add karo.

### 9. Pass test ✅
- [ ] Mere paas 15+ test cases hain, expected results ya rubric ke saath.
- [ ] 3 versions ko scores se compare kiya aur data se chuna.
- [ ] Mujhe LLM-as-judge ki kamzoriyan pata hain aur maine use apni scoring se check kiya.

Aage seekhne ke liye: [[GitHub Top Resources]] mein Anthropic ka `prompt_evaluations` course.

➡️ Next: [[Level 10 - Agents Context and Safety]]
