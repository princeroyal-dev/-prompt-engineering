---
tags: [prompt-engineering, resources, github]
aliases: [GitHub Resources, Top Repos]
---

# 🐙 GitHub: Top Prompt Engineering Resources

⬅️ [[00 START HERE]] | See also: [[Free Courses and Docs]]

**Checked on:** 2026-10-17. Star counts change, so treat them as a rough size signal.
**✅ Opened** = I opened the GitHub page and read it. **📎 Listed** = found through search results or another curated list; I did not open the page, so check it yourself.

---

## Core picks (start here)

| Repo | What it is | Free? / License | Stars | Check |
|---|---|---|---|---|
| [anthropics/prompt-eng-interactive-tutorial](https://github.com/anthropics/prompt-eng-interactive-tutorial) | Anthropic's hands-on tutorial: 9 chapters + appendix (beginner → advanced) with exercises and an answer key | Free to read. Running notebooks needs an API key (pay-per-use) | ~38.6k | ✅ Opened |
| [anthropics/courses](https://github.com/anthropics/courses) | 5 courses in order: API fundamentals → prompt engineering tutorial → real-world prompting → prompt evaluations → tool use | Free to read; API key for notebooks | ~22.3k | ✅ Opened |
| [dair-ai/Prompt-Engineering-Guide](https://github.com/dair-ai/Prompt-Engineering-Guide) | Big open guide: techniques, applications, prompt hub, risks, papers, 1-hr lecture + notebook. Web version: [promptingguide.ai](https://www.promptingguide.ai/) | Free guide, MIT license (the same team also sells paid courses; the guide itself is free) | ~77.4k | ✅ Opened |
| [promptslab/Awesome-Prompt-Engineering](https://github.com/promptslab/Awesome-Prompt-Engineering) | Curated list of papers, tools, courses, communities. Has a 5-step "Start Here" path | Free list, Apache-2.0 | ~6.3k | ✅ Opened |
| [thinkingjimmy/Learning-Prompt](https://github.com/thinkingjimmy/Learning-Prompt) | Free beginner course (site: [learningprompt.wiki](https://learningprompt.wiki/)): ChatGPT + Midjourney tutorials. Teaches *why*, not just prompt lists | Free, CC BY-NC 4.0 (non-commercial) | ~5.3k | ✅ Opened |

## More useful repos

| Repo | What it is | Check |
|---|---|---|
| [openai/openai-cookbook](https://github.com/openai/openai-cookbook) | Official OpenAI example notebooks (prompting, function calling, RAG, evals). Needs an API key for most examples | 📎 Listed |
| [NirDiamant/Prompt_Engineering](https://github.com/NirDiamant/Prompt_Engineering) | Hands-on Jupyter notebook tutorials (the Awesome list describes 22 notebooks) | 📎 Listed |
| [f/awesome-chatgpt-prompts](https://github.com/f/awesome-chatgpt-prompts) (also known as Prompts.chat) | Very large open prompt library. Quality varies; learn the *patterns*, don't copy blindly | 📎 Listed |
| [snwfdhmp/awesome-gpt-prompt-engineering](https://github.com/snwfdhmp/awesome-gpt-prompt-engineering) | Older curated list (techniques, prompt examples, communities). Some links may be outdated | 📎 Listed |
| [breatheco-de/prompt-engineering-exercise-course](https://github.com/breatheco-de/prompt-engineering-exercise-course) | Free interactive beginner course by 4Geeks (runs in Codespaces/LearnPack) | 📎 Listed |

---

## How to map them to your levels

| Your level | Do this alongside the vault |
|---|---|
| L1–L2 | Anthropic tutorial Ch.1 (Basic structure) and Ch.2 (Clear and direct) |
| L3 | Ch.3 (Assigning roles), Ch.5 (Formatting output) |
| L4 | Ch.4 (Separating data from instructions), Ch.7 (Examples) |
| L5 | Ch.6 (Thinking step by step); dair-ai Guide: Techniques → Chain-of-Thought |
| L6 | Ch.8 (Avoiding hallucinations) |
| L7–L8 | Ch.9 (Complex prompts), Appendix: chaining; `anthropics/courses` → real-world prompting |
| L9 | `anthropics/courses` → prompt evaluations |
| L10 | Tool use course, Appendix: tool use + search & retrieval; OpenAI Cookbook |

## Honest caveats (read these)

1. **"Free" has two meanings.** Reading is free. Running the official notebooks needs an API key and costs a little (the tutorial deliberately uses a cheap model). **Free workaround:** copy the exercise prompts into any free AI chat; you'll learn the same concepts, just without the notebook's automatic checks.
2. **Older models.** The Anthropic tutorial and courses say they use an older low-cost model (Claude 3 Haiku). The concepts still hold, but exact outputs differ on newer models.
3. **Google Sheets version.** The tutorial's README recommends its Google Sheets version as more user-friendly; it uses the "Claude for Sheets" extension.
4. **Hinglish.** I did not find a verified Hinglish GitHub prompt course. This vault's Hinglish notes fill that gap. If you find one, add it here.
5. **Prompt libraries** (like awesome-chatgpt-prompts) are good for inspiration, not as a substitute for Levels 2–4.

## 💡 New ideas for you

- **Fork and annotate:** fork `anthropics/prompt-eng-interactive-tutorial` or the dair-ai guide and add your own Hinglish notes in a `hinglish/` folder. That is a real, useful open-source contribution.
- **Own repo:** build `prompt-library` (see [[Level 08 - System Prompts and Apps]]) and link it in your GitHub profile README.
- **Weekly challenge:** every Sunday, pick one prompt from the Prompts.chat library and *improve* it using Levels 2–4, then log before/after.
