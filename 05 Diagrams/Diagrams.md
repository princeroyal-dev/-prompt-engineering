---
tags: [prompt-engineering, diagrams, mermaid]
aliases: [Diagrams, Maps, Visuals]
---

# 🖼️ Diagrams & Maps

⬅️ [[00 START HERE]]

**EN:** All diagrams use Obsidian's built-in Mermaid. If a block shows an error, tell me and I'll fix it.
**Hinglish:** Saare diagrams Mermaid mein hain. Obsidian mein apne aap render honge. Visual canvas map: [[Learning Map.canvas|Learning Map]].

---

## 1. Poora topic ek nazar mein (mind map)

```mermaid
mindmap
  root((Prompt Engineering))
    Basics
      Task
      Context
      Constraints
      Format
    Core techniques
      Be specific
      Role
      Examples
      Tags and delimiters
    Thinking
      Step by step
      Verify
    Reliability
      Ground in sources
      Allow not found
    Systems
      Chaining
      System prompts
      Evals
      Tools and RAG
      Injection safety
```

## 2. Ek prompt ke hisse (Level 1–3)

```mermaid
flowchart TB
  T["Task: kya karna hai"] --> P
  C["Context: background, kiske liye, kyu"] --> P
  K["Constraints: length, tone, kya avoid karna"] --> P
  F["Format: list, table, JSON, code"] --> P
  E["Examples: 2 to 5 (optional)"] --> P
  P{{"Final Prompt"}} --> M["Model"]
  M --> O["Output"]
```

## 3. Model ko kya dikhta hai (context window)

```mermaid
flowchart LR
  subgraph Ctx["Model ko sirf ye dikhta hai (context window)"]
    S["System prompt"]
    H["Pichhle messages"]
    D["Pasted documents / data"]
    X["Examples"]
    Q["Tumhara question"]
  end
  Ctx --> M["Model"] --> A["Answer"]
```

**Takeaway:** jo cheez context mein nahi, wo model ke liye exist nahi karti (jab tak app memory/tools na de).

## 4. Chat ka flow (roles)

```mermaid
sequenceDiagram
  participant S as System prompt
  participant U as You
  participant M as Model
  S->>M: Rules, role, format (standing)
  U->>M: Request + data
  M-->>U: Answer
  U->>M: Feedback / fix
  M-->>U: Improved answer
```

## 5. Iteration loop (Level 2, sabse zaruri habit)

```mermaid
flowchart LR
  A["Write prompt v1"] --> B["Run it"]
  B --> C{"Output good enough?"}
  C -- "Yes" --> D["Save in Prompt Library"]
  C -- "No" --> E["Diagnose: missing context? vague? wrong format?"]
  E --> F["Change ONE thing"]
  F --> B
```

## 6. Kaunsa technique kab (decision tree)

```mermaid
flowchart TD
  S["Output mein kya galat hai?"] --> A{"Vague ya off-topic?"}
  A -- "Haan" --> A1["Context + specific criteria add karo (L2)"]
  A -- "Nahi" --> B{"Format ya tone galat?"}
  B -- "Haan" --> B1["Format skeleton, role, examples do (L3, L4)"]
  B -- "Nahi" --> C{"Multi-step problem mein galat answer?"}
  C -- "Haan" --> C1["Step-by-step reasoning + verify (L5)"]
  C -- "Nahi" --> D{"Facts bana raha hai?"}
  D -- "Haan" --> D1["Source do, 'not found' allow karo (L6)"]
  D -- "Nahi" --> E{"Kaam ek prompt ke liye bada hai?"}
  E -- "Haan" --> E1["Chain mein todo (L7)"]
  E -- "Nahi" --> F["Bahut inputs par test karo: evals (L9)"]
```

## 7. Prompt chain (Level 7)

```mermaid
flowchart LR
  I["Input: raw notes"] --> P1["Step 1: Key points nikalo"]
  P1 --> P2["Step 2: Draft likho"]
  P2 --> P3["Step 3: Checklist se critique"]
  P3 --> P4["Step 4: Revise"]
  P4 --> O["Final output"]
```

## 8. Eval loop (Level 9)

```mermaid
flowchart TD
  A["Define karo 'good' kya hai: rubric"] --> B["15-30 test inputs banao"]
  B --> C["Prompt v1, v2, v3 chalao"]
  C --> D["Har output ko score karo"]
  D --> E{"Winner clear hai?"}
  E -- "Nahi" --> F["Prompts improve karo ya test cases badhao"]
  F --> C
  E -- "Haan" --> G["Use karo + tests regression ke liye rakho"]
```

## 9. Safety: trusted vs untrusted text (Level 10)

```mermaid
flowchart LR
  U["Tumhara instruction (trusted)"] --> M["Model"]
  W["Web page / email / file (untrusted)"] --> M
  M --> T{"Tool call ya risky action?"}
  T -- "Haan" --> H["Human approval + least privilege"]
  T -- "Nahi" --> O["Answer"]
```

**Takeaway:** untrusted text mein chhupe instructions model ko bhatka sakte hain. Sirf prompt likhkar ye problem poori tarah solve nahi hoti; permissions aur approvals bhi chahiye.
