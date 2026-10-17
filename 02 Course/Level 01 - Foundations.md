---
level: 1
tags: [prompt-engineering, level-1, course]
status: you-are-here
---

# Level 01: Foundations

⬅️ [[10-Level Roadmap]] | ➡️ [[Level 02 - Clarity and Specificity]]

> **Goal:** Understand what you are talking to, and what a prompt contains.
> **Time:** 1–2 days (1 day is enough if you already know the basics).

---

## 🇬🇧 English

### 1. What you are talking to
A large language model (LLM) is trained on huge amounts of text. It writes a response one *token* (a word-piece) at a time, choosing likely continuations. Result: it is very good at language, patterns, code and explanations, but it does **not read your mind**, and it can be **fluent and wrong**.

### 2. What a prompt is
Everything you send: your instruction, pasted text, examples, and the earlier messages in the chat. The model only works with what is inside its **context window** (the maximum amount of text, measured in tokens, it can handle at once). It cannot see your screen, your files or your intentions unless you put them in (or the app gives it tools).

### 3. The 4-part prompt

| Part | Question it answers | Example |
|---|---|---|
| **Task** | What should it do? | "Explain C pointers" |
| **Context** | Who is it for, why, what do I already know? | "I'm a beginner. I know variables and loops." |
| **Constraints** | Limits and rules | "Max 300 words, simple language, no jargon" |
| **Format** | Shape of the answer | "3 headings, 1 code example, 2 quiz questions" |

### 4. Chat app vs API (1-minute idea)
Chat apps may already contain hidden instructions. With an API you write the **system prompt** (standing rules) and the **user message** (this request) yourself. The same principles work in both. See the diagram: [[Diagrams]] (section 4).

### 5. Bad → Good
❌ `Explain pointers`

✅ `I am a beginner in C (I know variables, loops, functions). Explain pointers in simple language in under 300 words. Use one real-life analogy, one 8-line code example with comments, and end with 2 quiz questions.`

### 6. Exercises
- **1.1** Pick 3 prompts you wrote earlier. Rewrite each using the 4 parts.
- **1.2** Run old vs new in any AI chat. Write 2 differences you notice.
- **1.3** In one sentence each, define: token, context window, system prompt.
- **1.4** Ask the AI: "What information would help you answer this better?" for one of your prompts. Add what it asks for and run again.

### 7. Pass test ✅
- [ ] I can name the 4 parts without looking.
- [ ] My rewritten prompts give visibly better output.
- [ ] I know the model can be wrong, and I check important facts.

---

## 🇮🇳 Hinglish

### 1. Tum kisse baat kar rahe ho
LLM (Large Language Model) bahut saare text par train hota hai. Wo jawab ek *token* (shabd ka tukda) ek ke baad ek chunke likhta hai, jo sabse likely lagta hai. Isliye wo language, patterns, code aur explanation mein bahut accha hai, lekin wo **tumhara dimaag nahi padh sakta**, aur wo **confident hokar galat bhi bol sakta hai**.

### 2. Prompt kya hai
Jo bhi tum bhejte ho: instruction, paste kiya hua text, examples, aur chat ke pichhle messages. Model sirf apni **context window** ke andar jo hai usse kaam karta hai (context window = ek baar mein kitna text, tokens mein, wo handle kar sakta hai). Tumhari screen, files ya irada wo tab tak nahi dekh sakta jab tak tum use de na do (ya app use tools na de).

### 3. 4-part prompt

| Hissa | Kya batata hai | Example |
|---|---|---|
| **Task** | Kya karna hai? | "C pointers samjhao" |
| **Context** | Kiske liye, kyu, mujhe kya aata hai? | "Main beginner hoon. Variables aur loops aate hain." |
| **Constraints** | Limits aur rules | "300 words max, simple language, jargon nahi" |
| **Format** | Answer ka shape | "3 headings, 1 code example, 2 quiz questions" |

### 4. Chat app vs API
Chat app mein pehle se hidden instructions ho sakte hain. API mein tum khud **system prompt** (hamesha ke rules) aur **user message** (is baar ka kaam) likhte ho. Principles dono mein same hain. Diagram: [[Diagrams]] (section 4).

### 5. Bad → Good
❌ `pointers samjhao`

✅ `Main C mein beginner hoon (variables, loops, functions aate hain). Pointers simple Hinglish mein 300 words ke andar samjhao. Ek real-life analogy do, 8 line ka commented code example do, aur end mein 2 quiz questions do.`

### 6. Exercises
- **1.1** Apne 3 purane prompts uthao. Har ek ko 4 parts mein dobara likho.
- **1.2** Purana aur naya, dono kisi AI chat mein chalao. 2 farq likho.
- **1.3** Ek-ek line mein likho: token, context window, system prompt.
- **1.4** AI se pucho: "Is prompt ka behtar jawab dene ke liye tumhe kaunsi information chahiye?" Jo bole wo add karke dobara chalao.

### 7. Pass test ✅
- [ ] 4 parts bina dekhe bata sakta hoon.
- [ ] Rewritten prompts ka output clearly behtar hai.
- [ ] Mujhe pata hai model galat ho sakta hai, aur zaruri facts main check karta hoon.

➡️ Next: [[Level 02 - Clarity and Specificity]]
