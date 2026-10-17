---
tags: [prompt-engineering, prompt-book, template, coding]
aliases: [Coding Templates]
---

# 💻 Templates: Coding

⬅️ [[Prompt Book Index]]

> **Safety rule:** AI-written code and commands can be wrong. Read them, understand them, and test in a safe place before using them. Be extra careful with delete/format/permission commands.

---

## 1. Explain code line by line
```
Explain this [LANGUAGE] code to a beginner, line by line.
For each line or block: what it does, and why it is needed.
End with the 3 most important ideas in this code.
<code>
[paste code]
</code>
```

## 2. Debug
```
My [LANGUAGE] program does not work.
Expected behaviour: [WHAT SHOULD HAPPEN]
Actual behaviour: [WHAT HAPPENS]
What I already tried: [TRIED]
<code>
[paste code]
</code>
<error>
[paste exact error output]
</error>
Give 3 likely causes, most likely first. For each: why, and a 1-line check I can run.
Do not rewrite my whole program. Tell me which check to do first.
```

## 3. Code review
```
Review this [LANGUAGE] code as a senior reviewer.
Check: correctness, edge cases (empty input, big input), readability, security, memory/resource handling.
Output a table: Severity (high/med/low) | Line or area | Problem | Suggested fix.
End with the single most important change.
<code>
[paste code]
</code>
```

## 4. Write a function + tests
```
Write a [LANGUAGE] function that [WHAT IT DOES].
Inputs: [INPUTS]. Output: [OUTPUT]. Edge cases to handle: [EDGE CASES].
Include 5 test cases (normal, edge, and invalid input).
Add comments that explain the logic. Explain the time complexity in one line.
```

## 5. Explain an error message
```
Explain this error in simple words: what it means, the 3 most common causes, and how to fix each.
Context: [WHAT I WAS DOING]
<error>
[paste error]
</error>
```

## 6. Linux / Docker command helper (safe version)
```
I am on [OS] with [TOOL, e.g. Docker] installed. I want to [GOAL].
Give the commands step by step. For each command: what it does, what it changes, and whether it is safe to undo.
Clearly flag anything destructive (e.g. rm, prune, --force, overwriting files) and ask me to confirm before I run it.
If you are unsure about an option or flag, say so instead of guessing.
```

## 7. Refactor with limits
```
Refactor this code for readability without changing behaviour.
Rules: keep the same function names and outputs; no new libraries; explain each change in one line.
<code>
[paste code]
</code>
```

## 8. Learn from my mistake
```
Here is my code and the corrected version. Explain what concept I was missing, why my version failed, and give me 2 similar practice problems.
<my_code>
[paste]
</my_code>
<fixed_code>
[paste]
</fixed_code>
```
