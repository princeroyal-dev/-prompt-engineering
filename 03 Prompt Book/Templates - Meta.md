---
tags: [prompt-engineering, prompt-book, template, meta]
aliases: [Meta Templates, Prompt Improver]
---

# 🔁 Templates: Meta (improving your prompts)

⬅️ [[Prompt Book Index]]

> **Caution:** An AI's explanation of why its own output was bad is a *hypothesis*, not proof. Test any change it suggests (Level 2 loop, Level 9 evals).

---

## 1. Prompt improver
```
Here is my prompt:
<prompt>
[paste prompt]
</prompt>

1) List what is unclear, missing or likely to cause a bad output.
2) Ask me up to 3 questions that would most improve it.
3) Then rewrite the prompt using: Role, Goal, Context, Constraints, Output format.
Keep my original intent. Do not add requirements I did not ask for.
```

## 2. Ask me questions first
```
I want to [GOAL]. Before you answer, ask me up to 5 questions that you need answered to do this well.
Ask them one group at a time. After I answer, produce the result.
```

## 3. Critique an output against my checklist
```
Here is my checklist for a good answer:
<checklist>
1. [CRITERION]
2. [CRITERION]
3. [CRITERION]
</checklist>
<output>
[paste AI output]
</output>
Score the output 1–5 on each criterion with one sentence of evidence. Then list the 2 smallest changes to the prompt that would fix the weakest criterion.
```

## 3b. Why was this output bad? (post-mortem)
```
My prompt:
<prompt>[paste]</prompt>
The output I got:
<output>[paste]</output>
What I wanted instead: [DESCRIBE]
Give 3 hypotheses for why the output missed, ranked by likelihood, and one prompt change to test each.
```

## 4. Three variants
```
Rewrite this prompt in 3 different ways:
A) shortest possible, B) most detailed, C) with 2 examples added.
For each variant, say what it trades off. I will test them on my own inputs.
<prompt>[paste]</prompt>
```

## 5. Vague goal → spec
```
My goal is: "[VAGUE GOAL]".
Turn it into a clear task spec with: the exact deliverable, the audience, success criteria (measurable), constraints, and what information you still need from me.
```

## 6. Make a reusable template
```
Turn this one-off prompt into a reusable template with {{VARIABLES}} for the parts that change.
List the variables and give one filled example.
<prompt>[paste]</prompt>
```
