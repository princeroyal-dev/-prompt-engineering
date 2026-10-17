---
level: 8
tags: [prompt-engineering, level-8, course]
status: upcoming
---

# Level 08: System Prompts and Apps

⬅️ [[Level 07 - Chaining and Complex Tasks]] | ➡️ [[Level 09 - Evals and Testing]]

> **Goal:** Write standing instructions for assistants and manage prompts like real project files (versions, library, changelog).
> **Time:** 1 week.

---

## 🇬🇧 English

### 1. System prompt vs user prompt
- **System prompt:** standing rules, role, tone, format, boundaries. Applies to the whole conversation.
- **User prompt:** this request and its data.

In chat apps, similar features appear as custom instructions, project instructions or preferences. See [[Diagrams]] (section 4).

### 2. Anatomy of a good system prompt
1. **Role and audience** (who you are, who you serve)
2. **Goal** (what a good result looks like)
3. **Rules** (do / don't, with reasons when helpful)
4. **Tone and format**
5. **When unsure:** ask a question, or say "I don't know", don't guess
6. **Boundaries:** what is out of scope

Explain the *why* behind important rules; models follow rules better when they understand the purpose.

### 3. Example: Hinglish C tutor (starter)
```
You are a patient C programming tutor for a beginner who writes in Hinglish
(Hindi in Roman script) and understands simple English.

Goal: help the student really understand, not just get answers.

Rules:
- Explain in simple Hinglish; keep technical terms in English.
- Teach from zero to advanced: start with an analogy, then a small example, then a harder one.
- After each explanation, ask 1 check question and wait for the answer.
- If the student's code has a bug, point to the likely cause first and let them try before giving the fix.
- If you are not sure, say so. Never invent functions or behaviour.

Format: short sections with headings; code in fenced blocks with comments.
```

### 4. Prompts are files: version them
- Keep each prompt in its own `.md` file.
- Name versions: `v1`, `v2`, `v3`.
- Keep a **changelog**: what changed, why, and what the test results were.
- Store them in Git/GitHub. Good prompts become your portfolio.

### 5. Prompt library repo (suggested structure)
```
prompt-library/
  README.md            # what this is, how to use
  prompts/
    tutor-c/
      v1.md  v2.md  CHANGELOG.md
    debugging/
      v1.md
  examples/            # good inputs and outputs
  tests/               # your eval cases (Level 9)
```

### 6. Mini-project
Write a system prompt for an assistant you'd actually use (tutor, code reviewer, note-taker). Test it on 5 inputs. Create v2 fixing the worst failure. Save both in a `prompt-library` repo with a changelog.

### 7. Exercises
- **8.1** Write a system prompt with all 6 parts. Remove one part at a time and see what breaks.
- **8.2** Add a "when unsure" rule and test with a question the AI can't know.
- **8.3** Publish your repo on GitHub with a README.

### 8. Pass test ✅
- [ ] I have a system prompt with role, rules, tone, format, unsure-rule and boundaries.
- [ ] I have v1 and v2 with a changelog explaining why v2 exists.
- [ ] My prompts live in a Git repo.

---

## 🇮🇳 Hinglish

### 1. System prompt vs user prompt
- **System prompt:** hamesha ke rules, role, tone, format, boundaries. Poori conversation par lagta hai.
- **User prompt:** is baar ka request aur uska data.

Chat apps mein ye custom instructions, project instructions ya preferences jaise features hote hain. Diagram: [[Diagrams]] (section 4).

### 2. Accha system prompt kaise banta hai
1. **Role aur audience** (tum kaun ho, kiski madad karte ho)
2. **Goal** (accha result kaisa dikhta hai)
3. **Rules** (kya karna / nahi karna, jahan zaruri ho wajah ke saath)
4. **Tone aur format**
5. **Pata na ho to:** sawal pucho ya "pata nahi" bolo, guess mat karo
6. **Boundaries:** kya scope se bahar hai

Important rules ki *wajah* batao. Model rules ko behtar follow karta hai jab use purpose samajh aata hai.

### 3. Example: Hinglish C tutor
Upar English block mein starter system prompt hai. Use copy karke apne hisaab se badlo.

### 4. Prompts bhi files hain: version karo
- Har prompt ki alag `.md` file.
- Versions ke naam: `v1`, `v2`, `v3`.
- **Changelog** rakho: kya badla, kyu badla, aur test results kya the.
- Git/GitHub mein rakho. Acche prompts tumhara portfolio ban jate hain.

### 5. Prompt library repo (structure upar English block mein)
`prompts/`, `examples/`, `tests/` folders aur ek README. Tests Level 9 mein banenge.

### 6. Mini-project
Aisa assistant ka system prompt likho jo tum sach mein use karoge (tutor, code reviewer, note-taker). 5 inputs par test karo. Sabse badi failure fix karke v2 banao. Dono ko changelog ke saath `prompt-library` repo mein save karo.

### 7. Exercises
- **8.1** 6 parts wala system prompt likho. Ek-ek part hatakar dekho kya toot-ta hai.
- **8.2** "Pata na ho to" rule add karo aur aisa sawal pucho jo AI jaan hi nahi sakta.
- **8.3** Apna repo README ke saath GitHub par publish karo.

### 8. Pass test ✅
- [ ] Mere paas role, rules, tone, format, unsure-rule aur boundaries wala system prompt hai.
- [ ] v1 aur v2 hain, changelog ke saath jo batata hai ki v2 kyu bana.
- [ ] Mere prompts ek Git repo mein hain.

➡️ Next: [[Level 09 - Evals and Testing]]
