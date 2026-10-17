---
tags: [prompt-engineering, roadmap]
aliases: [Roadmap, Levels]
---

# 🗺️ 10-Level Roadmap

⬅️ [[00 START HERE]]

**EN:** Each level builds on the last. Do the mini-project and the pass test before moving on.
**Hinglish:** Har level pichhle level par bana hai. Mini-project aur pass test karne ke baad hi aage badho.

```mermaid
flowchart LR
  L1["L1 Foundations"] --> L2["L2 Clarity"] --> L3["L3 Role Context Format"] --> L4["L4 Examples Structure"] --> L5["L5 Reasoning"]
  L5 --> L6["L6 Reliability"] --> L7["L7 Chaining"] --> L8["L8 System Prompts"] --> L9["L9 Evals"] --> L10["L10 Agents Context Safety"]
  classDef here fill:#fde68a,stroke:#b45309,color:#000
  class L1,L2 here
```

📍 Yellow = tum abhi yahan ho (Level 1–2).

---

## Level table

| # | Level | Core skill | Mini-project | Pass test (short) |
|---|---|---|---|---|
| 1 | [[Level 01 - Foundations]] | 4-part prompt: Task, Context, Constraints, Format | 3 purane prompts rewrite karo | 4 parts bina dekhe bata sako |
| 2 | [[Level 02 - Clarity and Specificity]] | Vague → measurable, iteration loop | Ek task ke 3 versions compare karo | v3 checklist par v1 se behtar ho |
| 3 | [[Level 03 - Role Context and Format]] | Role, context, output format control | "AI tutor" prompt (fixed format) | Output har baar same shape mein aaye |
| 4 | [[Level 04 - Examples and Structure]] | Few-shot, XML tags/delimiters | Notes → flashcards (3 examples ke saath) | Examples se format/accuracy improve ho |
| 5 | [[Level 05 - Reasoning and Thinking]] | Step-by-step, verify, decomposition | Debugging prompt (hypotheses + check) | Multi-step problem par answer verify kar sako |
| 6 | [[Level 06 - Reliability and Hallucinations]] | Grounding, "not found", quote-first | Document Q&A with refusal | Unanswerable questions par "not found" de |
| 7 | [[Level 07 - Chaining and Complex Tasks]] | Prompt chains, templates | Outline → draft → critique → final | Chain single prompt se behtar ho (proof ke saath) |
| 8 | [[Level 08 - System Prompts and Apps]] | System prompts, prompt library, versioning | Hinglish tutor system prompt + GitHub prompt library | Prompt ka v1, v2 changelog ke saath ho |
| 9 | [[Level 09 - Evals and Testing]] | Test set, rubric, A/B | 3 versions × 15 cases scoring | Data se winner chuno, feeling se nahi |
| 10 | [[Level 10 - Agents Context and Safety]] | Tools, RAG, context engineering, injection safety | Capstone: ek chhota tool-using assistant | Risky actions ke liye guardrails ho |

---

## Level kaise cross karte hain

1. Lesson padho (English ya Hinglish).
2. Saare exercises karo aur [[My Progress]] mein log likho.
3. Mini-project banao.
4. Pass test ke saare checkboxes tick ho jayein, tab hi agla level.

## Tumhare liye suggestion (Level 1–2 par ho)

- **Level 1:** 1 din. Tum thoda jaante ho, bas 4-part structure pakka karo.
- **Level 2:** 3–4 din. Yahi sabse bada jump deta hai, kyunki zyadatar kharab outputs ki wajah vague prompts hoti hain.
- **Level 3–4:** 1 hafta. Format aur examples se output ki quality predictable ho jati hai.
- Level 5 ke baad "pro" territory shuru hoti hai: reliability, chains, evals.

Visual version: [[Learning Map.canvas|Learning Map]] aur [[Diagrams]].
