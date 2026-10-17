---
tags: [prompt-engineering, prompt-book, mistakes]
aliases: [Common Mistakes, Troubleshooting]
---

# ⚠️ Mistakes and Fixes

⬅️ [[Prompt Book Index]]

**EN:** Find your symptom, apply the fix, change one thing at a time.
**Hinglish:** Apna symptom dhundo, fix lagao, ek baar mein ek hi cheez badlo.

| # | Mistake | Why it hurts | Fix | Level |
|---|---|---|---|---|
| 1 | Vague ask ("write about X") | Model guesses audience, length, depth | Add audience, purpose, length, format | [[Level 02 - Clarity and Specificity]] |
| 2 | No context | Model can't know your level or material | Paste real code/text, state your level and goal | [[Level 03 - Role Context and Format]] |
| 3 | Too many jobs in one prompt | Quality drops, hard to debug | Split into a chain | [[Level 07 - Chaining and Complex Tasks]] |
| 4 | No output format | Shape changes every time | Give a skeleton or table columns | [[Level 03 - Role Context and Format]] |
| 5 | Only "don't" instructions | Harder to follow than a positive instruction | Say what TO do ("write 2 paragraphs") | [[Level 02 - Clarity and Specificity]] |
| 6 | Examples that are all alike | Model copies length/style too closely | Use 3–5 varied examples | [[Level 04 - Examples and Structure]] |
| 7 | Pasting data mixed with instructions | Model may confuse data with commands | Wrap data in tags | [[Level 04 - Examples and Structure]] |
| 8 | Assuming it remembers other chats | It only sees the current context (unless the app has memory) | Re-state key context, or use project/custom instructions | [[Level 01 - Foundations]] |
| 9 | Trusting links, citations, numbers | Can be invented | Check in the real source; ground in documents | [[Level 06 - Reliability and Hallucinations]] |
| 10 | "Magic phrases" ("tip $200", "you are a 100x expert") | Unreliable; not a substitute for clear instructions | Spend those words on context and criteria | [[Level 02 - Clarity and Specificity]] |
| 11 | Changing 5 things at once | You can't tell what helped | Change one thing, re-run, compare | [[Level 02 - Clarity and Specificity]] |
| 12 | Judging by 1–2 examples | Prompt may fail on other inputs | Test on 10–15 cases | [[Level 09 - Evals and Testing]] |
| 13 | Contradicting instructions | Model has to guess which wins | Re-read the prompt; remove conflicts | [[Level 02 - Clarity and Specificity]] |
| 14 | Copying prompts without understanding them | Can't fix them when they fail | Know why each line is there | [[Level 08 - System Prompts and Apps]] |
| 15 | Treating outside text as safe | Prompt injection | Label as data, limit tool permissions | [[Level 10 - Agents Context and Safety]] |

## Quick triage

Diagram: [[Diagrams]] (section 6: kaunsa technique kab).
