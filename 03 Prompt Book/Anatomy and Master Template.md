---
tags: [prompt-engineering, prompt-book, template]
aliases: [Master Template, Anatomy]
---

# 🧬 Anatomy and Master Template

⬅️ [[Prompt Book Index]]

Diagram: [[Diagrams]] (section 2: ek prompt ke hisse).

## 🇬🇧 The 7-part master template

```
ROLE: [who the AI should act as]
GOAL: [what a good result looks like, and why I need it]
CONTEXT: [my level, background, what I tried, constraints]
INPUT:
<input>
[paste text / code / data here]
</input>
CONSTRAINTS: [length, tone, language, what to avoid, what to do if unsure]
OUTPUT FORMAT: [skeleton, table columns, JSON fields]
QUALITY CHECK: Before answering, check that every requirement above is met.
If information is missing, ask me up to 3 questions first.
```

**Use only the parts you need.** A simple question needs 2 parts; a complex task needs most of them.

## 🇮🇳 Hinglish version

```
ROLE: [AI kaun bane]
GOAL: [accha result kaisa ho, aur mujhe kyu chahiye]
CONTEXT: [mera level, background, kya try kiya, limits]
INPUT:
<input>
[yahan text / code / data paste karo]
</input>
CONSTRAINTS: [length, tone, language, kya avoid karna, pata na ho to kya karna]
OUTPUT FORMAT: [skeleton, table columns, JSON fields]
QUALITY CHECK: Jawab dene se pehle check karo ki upar ki har requirement poori hui.
Agar information kam ho to pehle mujhse max 3 sawal pucho.
```

## ✍️ Filled example

```
ROLE: Patient Linux and Docker tutor.
GOAL: I want to understand Docker volumes well enough to explain them in a viva.
CONTEXT: I know basic Linux commands and have run `docker run` a few times. I have not used volumes.
CONSTRAINTS: Simple Hinglish, technical terms in English, max 400 words. If you are unsure about a detail, say so.
OUTPUT FORMAT:
## Concept (3 lines)
## Analogy (1 line)
## Hands-on (3 commands, each with a one-line explanation)
## Common mistakes (3 bullets)
## Viva questions (3, answers at the end)
QUALITY CHECK: Make sure every command is safe to run and explain what it changes.
```

## Quick self-check before you press Enter

- [ ] Kya ek naya colleague bhi samajh jayega ki kya karna hai?
- [ ] Context diya (level, material, goal)?
- [ ] Format batayi?
- [ ] Limits numbers mein hain?
- [ ] Data tags mein hai, instruction se alag?
