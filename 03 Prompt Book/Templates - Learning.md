---
tags: [prompt-engineering, prompt-book, template, learning]
aliases: [Learning Templates]
---

# 🎓 Templates: Learning

⬅️ [[Prompt Book Index]]

Replace `[BRACKETS]`. Hinglish ya English, jo tumhe comfortable ho, wahi language set karo.

---

## 1. Zero → Pro teacher
```
You are a patient teacher. Teach me [TOPIC] from zero to pro in 5 stages:
Stage 0 Zero: an analogy, no jargon.
Stage 1 Basics: key terms and one small example.
Stage 2 Intermediate: how it works, and common mistakes.
Stage 3 Advanced: edge cases and design trade-offs.
Stage 4 Pro: how experts think, best practices, and what to build to master it.

My current level: [LEVEL, e.g. "beginner, I know variables and loops"].
Language: simple Hinglish; keep technical terms in English.
After each stage, ask 2 check questions and STOP. Wait for my answers before going on.
If you are unsure about a fact, say so. Do not invent.
```

## 2. Quiz me
```
Quiz me on [TOPIC]. Ask one question at a time, starting easy and getting harder.
After each answer: say correct/incorrect, explain why in 2 lines, then ask the next question.
After 8 questions, list my weak areas and what to revise.
```

## 3. Gap finder (I explain, you check)
```
I will explain [TOPIC] in my own words. Do NOT correct me while I explain.
After I finish, list: (1) what I got right, (2) what is wrong or missing, (3) 3 follow-up questions an examiner might ask.
My explanation:
<explanation>
[paste your explanation]
</explanation>
```

## 4. Notes → flashcards
```
Convert my notes into flashcards.
Output as a table: Question | Answer (max 25 words) | Difficulty (easy/medium/hard).
Make 10 cards. Use only information in the notes; if the notes are unclear, skip that point.
<notes>
[paste notes]
</notes>
```

## 5. Study plan
```
Make a [N]-day study plan to learn [TOPIC]. I can study [X] minutes per day.
I already know: [KNOWN]. My goal: [GOAL, e.g. "write a small program using it"].
Table columns: Day | Goal | Learn | Practice | Self-check.
Finish with 3 common beginner mistakes.
```

## 6. Compare A vs B
```
Compare [A] and [B] for [PURPOSE].
Table with columns: Aspect | A | B | When to choose. Max 6 rows.
Then give one-line advice: which to pick if [MY SITUATION].
```

## 7. Misconception check
```
List the 5 most common misconceptions beginners have about [TOPIC].
For each: the wrong idea, why it feels right, and a 1-line test that shows it's wrong.
```

## 8. Explain at 3 levels
```
Explain [TOPIC] at three levels: (1) like I'm 12, (2) beginner college student, (3) practitioner.
Each level max 80 words. Then say what to learn next.
```
