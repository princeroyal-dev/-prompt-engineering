---
tags: [prompt-engineering, prompt-book, cheatsheet]
aliases: [Cheatsheet, Quick Reference]
---

# 🧾 Cheat Sheet (1 page)

⬅️ [[Prompt Book Index]]

## 4 parts of a prompt
**Task** → **Context** → **Constraints** → **Format**
(Kya karna hai → Kiske liye/kyu → Limits → Output ka shape)

## 10 golden rules
1. Colleague test: kya ek naya smart colleague samjhega?
2. Vague words ko numbers se badlo ("short" → "under 120 words").
3. Audience + purpose batao.
4. Kya KARNA hai bolo, sirf kya nahi.
5. Real material paste karo (code, error, text).
6. Output ka skeleton do.
7. 3–5 varied examples jab format/style important ho.
8. Data ko tags mein rakho, instruction se alag.
9. Multi-step problem: pehle reasoning, phir final answer, phir verify.
10. Ek baar mein ek cheez badlo, aur log karo.

## Starter lines (copy-paste)
- `If anything is unclear, ask me up to 3 questions first.`
- `Answer using only the text in <document>. If it's not there, write NOT FOUND.`
- `Think step by step, then give the final answer in <answer> tags.`
- `Before answering, check that every requirement above is met.`
- `If you are not sure, say so. Do not invent facts, links or functions.`
- `Output as a table with columns: ...`
- `Explain in simple Hinglish; keep technical terms in English.`

## Technique picker
| Problem | Try |
|---|---|
| Vague / off-topic | More context + criteria (L2) |
| Wrong tone / format | Role, skeleton, examples (L3–4) |
| Wrong on multi-step | Step-by-step + verify (L5) |
| Makes up facts | Ground in source, NOT FOUND rule (L6) |
| Task too big | Chain (L7) |
| Works only sometimes | Evals (L9) |

## After you get the output
- [ ] Correct? (facts, numbers, code run)
- [ ] Complete? (all requirements met)
- [ ] Right format?
- [ ] What ONE change would improve the prompt?

Related: [[Anatomy and Master Template]], [[Mistakes and Fixes]], [[Glossary]]
