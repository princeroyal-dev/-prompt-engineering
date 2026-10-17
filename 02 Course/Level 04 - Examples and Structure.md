---
level: 4
tags: [prompt-engineering, level-4, course]
status: upcoming
---

# Level 04: Examples and Structure

⬅️ [[Level 03 - Role Context and Format]] | ➡️ [[Level 05 - Reasoning and Thinking]]

> **Goal:** Teach the model by showing examples, and keep instructions separate from data using tags/delimiters.
> **Time:** 3–4 days.

---

## 🇬🇧 English

### 1. Zero-shot, one-shot, few-shot
- **Zero-shot:** instructions only.
- **One-shot:** one example.
- **Few-shot:** several examples. Usually 3–5 diverse examples work well.

Examples are very powerful: the model copies their style, length and format. Choose them deliberately.

### 2. Example rules
1. Cover variety (easy, tricky, edge case).
2. Keep format identical across examples.
3. Make examples look like the real input you'll send.
4. Beware accidental copying: if all examples are 10 words long, outputs will be about 10 words long.
5. Label them clearly (`<example>` tags or "Example 1").

```
Classify each message as Positive, Negative or Neutral.

Message: "Yaar ye course zabardast hai!"  → Positive
Message: "App baar baar crash ho raha hai."  → Negative
Message: "Class kal 10 baje hai."  → Neutral

Message: "Delivery late thi par support ne help ki."  →
```

### 3. Delimiters and XML-style tags
Wrap different parts so the model can tell instructions from data:

```
<instructions>Summarize in 3 bullets for a beginner.</instructions>
<document>
...pasted text...
</document>
```

Why: avoids mixing your instruction with the pasted text, makes long prompts easier to read, and lets you refer to parts ("use only the text in <document>"). Tag names are your choice; be consistent.

### 4. Long inputs
When you paste long documents, put the document first and your question/instruction at the end. This usually helps quality on long inputs.

### 5. Templates with variables
Reusable prompts use placeholders: `{{TOPIC}}`, `{{LEVEL}}`, `{{TEXT}}`. Fill them each time. This is the start of "prompt as code" (Levels 7–8).

### 6. Mini-project: notes → flashcards
Prompt takes `<notes>` and returns a table (Question | Answer | Difficulty). Include 3 examples. Test on 2 different note sets. Then remove the examples and compare: what changed?

### 7. Exercises
- **4.1** Few-shot classifier on your own labels (Hinglish messages, error types, or topics).
- **4.2** Same task zero-shot vs 3-shot. Score both on 10 inputs.
- **4.3** Wrap a pasted article in tags and ask for 3 different outputs from it.

### 8. Pass test ✅
- [ ] My few-shot version beats zero-shot on at least 8 of 10 inputs, or I can explain why not.
- [ ] I use tags/delimiters for pasted data.
- [ ] I have one reusable template with `{{variables}}`.

---

## 🇮🇳 Hinglish

### 1. Zero-shot, one-shot, few-shot
- **Zero-shot:** sirf instructions.
- **One-shot:** ek example.
- **Few-shot:** kai examples. Aam taur par 3–5 alag-alag examples acche kaam karte hain.

Examples bahut powerful hote hain: model unka style, length aur format copy karta hai. Soch samajh kar chuno.

### 2. Example ke rules
1. Variety rakho (easy, tricky, edge case).
2. Format sabhi examples mein same ho.
3. Examples asli input jaise dikhein.
4. Galti se copy hone se bacho: agar sab examples 10 shabd ke hain to output bhi lagbhag 10 shabd ka aayega.
5. Clearly label karo (`<example>` tags ya "Example 1").

Upar wale English block mein classifier example dekho. Tum Hinglish messages par bhi same pattern use kar sakte ho.

### 3. Delimiters aur XML-style tags
Alag-alag hisson ko wrap karo, taaki model instructions aur data mein farq samjhe:

```
<instructions>Beginner ke liye 3 bullets mein summarize karo.</instructions>
<document>
...paste kiya hua text...
</document>
```

Kyu: instruction paste kiye hue text se mix nahi hota, lamba prompt padhna aasan hota hai, aur tum hisson ko refer kar sakte ho ("sirf <document> ka text use karo"). Tag ke naam tum chuno, bas consistent rakho.

### 4. Lambe inputs
Lamba document paste karo to document **pehle** rakho aur sawal/instruction **end mein**. Lambe inputs par ye aksar quality badhata hai.

### 5. Variables wale templates
Reusable prompts mein placeholders hote hain: `{{TOPIC}}`, `{{LEVEL}}`, `{{TEXT}}`. Har baar bharo. Ye "prompt as code" ki shuruaat hai (Level 7–8).

### 6. Mini-project: notes → flashcards
Prompt `<notes>` lega aur table dega (Question | Answer | Difficulty). 3 examples shamil karo. 2 alag notes par test karo. Phir examples hata kar compare karo: kya badla?

### 7. Exercises
- **4.1** Apne labels par few-shot classifier (Hinglish messages, error types ya topics).
- **4.2** Wahi task zero-shot vs 3-shot. 10 inputs par dono ko score karo.
- **4.3** Ek article ko tags mein wrap karke us par 3 alag outputs maango.

### 8. Pass test ✅
- [ ] Mera few-shot version 10 mein se kam se kam 8 inputs par zero-shot se behtar hai, ya main bata sakta hoon kyu nahi.
- [ ] Pasted data ke liye tags/delimiters use karta hoon.
- [ ] Mere paas `{{variables}}` wala ek reusable template hai.

➡️ Next: [[Level 05 - Reasoning and Thinking]]
