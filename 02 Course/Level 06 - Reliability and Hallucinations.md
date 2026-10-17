---
level: 6
tags: [prompt-engineering, level-6, course]
status: upcoming
---

# Level 06: Reliability and Hallucinations

⬅️ [[Level 05 - Reasoning and Thinking]] | ➡️ [[Level 07 - Chaining and Complex Tasks]]

> **Goal:** Reduce made-up answers and build prompts you can trust more.
> **Time:** 3–4 days.

---

## 🇬🇧 English

### 1. What a hallucination is
A fluent answer that is wrong or invented: fake facts, fake citations, wrong numbers, functions or libraries that don't exist. It is most likely on obscure facts, exact numbers, quotes, links, and recent events.

### 2. Prompt-level fixes
1. **Give the source** and restrict: "Answer using only the text in `<document>`."
2. **Allow "I don't know":** "If the answer is not in the document, reply exactly: NOT FOUND."
3. **Quote first, answer second:** "First copy the 1–3 sentences that support your answer inside `<quotes>`, then answer."
4. **Ask what to verify:** "List any claims here that I should double-check, and why."
5. **Ask for confidence by claim,** not as a vague overall feeling.
6. **Use search or tools** for current or exact facts, when your app offers them.
7. **Lower randomness** (temperature) for factual extraction, where the tool lets you set it.

### 3. Things never to trust blindly
Links and URLs, citations, paper titles, package/function names, version numbers, legal/medical/financial specifics, and anything high-stakes. Check them in the real source.

### 4. Make outputs checkable
Ask for structured output (JSON/table) so you can verify with a script or a quick scan. For code: run it, test it.

### 5. Worked example (grounded Q&A)
```
<document>
...paste text...
</document>

Answer the question using only the document.
Steps: 1) copy supporting sentences into <quotes>. 2) write the answer in <answer>.
If the document does not contain the answer, write NOT FOUND in <answer> and nothing else.

Question: ...
```

### 6. Mini-project: document Q&A
Take a 1-page text. Ask 3 questions that **are** in it and 3 that **aren't**. Success = correct answers for the first 3, and NOT FOUND for the other 3.

### 7. Exercises
- **6.1** Ask the AI for 3 sources/links on an obscure topic. Check each in a browser. How many exist?
- **6.2** Run the mini-project with and without the NOT FOUND rule. Compare.
- **6.3** Take an AI answer and fact-check 5 claims against real sources. Write what you found in [[My Progress]].

### 8. Pass test ✅
- [ ] My Q&A prompt says NOT FOUND for unanswerable questions (at least 2 of 3).
- [ ] I check links, citations and numbers myself.
- [ ] I know when to use search/tools instead of trusting memory.

---

## 🇮🇳 Hinglish

### 1. Hallucination kya hai
Fluent lekin galat ya banaya hua answer: fake facts, fake citations, galat numbers, aise functions ya libraries jo exist hi nahi karte. Ye sabse zyada obscure facts, exact numbers, quotes, links aur recent events par hota hai.

### 2. Prompt-level fixes
1. **Source do** aur limit lagao: "Sirf `<document>` ke text se jawab do."
2. **"Pata nahi" allow karo:** "Agar answer document mein nahi hai to exactly likho: NOT FOUND."
3. **Pehle quote, phir answer:** "Pehle answer ko support karne wale 1–3 sentences `<quotes>` mein copy karo, phir answer do."
4. **Verify kya karna hai pucho:** "Kaunse claims mujhe double-check karne chahiye aur kyu?"
5. **Confidence har claim ke liye maango,** ek vague overall feeling nahi.
6. **Search ya tools use karo** current ya exact facts ke liye, agar app deta hai.
7. **Randomness (temperature) kam rakho** factual extraction ke liye, jahan tool set karne deta hai.

### 3. Jin par andhvishwas mat karo
Links/URLs, citations, paper titles, package/function names, version numbers, legal/medical/financial details, aur kuch bhi high-stakes. Asli source mein check karo.

### 4. Output ko checkable banao
Structured output (JSON/table) maango taaki script ya quick scan se verify kar sako. Code ho to run karo, test karo.

### 5. Worked example (grounded Q&A)
Upar English wala prompt copy karo. Hinglish mein bhi chalega, bas "NOT FOUND" jaisa exact phrase fix rakho.

### 6. Mini-project: document Q&A
1 page ka text lo. 3 sawal aise pucho jo usme **hain** aur 3 aise jo usme **nahi hain**. Success = pehle 3 ke sahi answers, aur baaki 3 par NOT FOUND.

### 7. Exercises
- **6.1** AI se kisi obscure topic par 3 sources/links maango. Har ek browser mein kholo. Kitne asli nikle?
- **6.2** Mini-project NOT FOUND rule ke saath aur bina uske chalao. Compare karo.
- **6.3** Ek AI answer ke 5 claims asli sources se fact-check karo. Jo mila wo [[My Progress]] mein likho.

### 8. Pass test ✅
- [ ] Mera Q&A prompt unanswerable sawalon par NOT FOUND deta hai (3 mein se kam se kam 2).
- [ ] Links, citations aur numbers main khud check karta hoon.
- [ ] Mujhe pata hai kab search/tools use karne hain, memory par bharosa nahi karna.

➡️ Next: [[Level 07 - Chaining and Complex Tasks]]
