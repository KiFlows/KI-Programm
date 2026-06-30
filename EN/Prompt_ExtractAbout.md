You know me from our previous chats and your memory.
The templates are public on GitHub. Fetch them yourself — I'm not attaching or downloading anything.

Templates (fetch via raw URL, repo KiFlows/KI-Programm, branch main):
- https://raw.githubusercontent.com/KiFlows/KI-Programm/main/EN/Skill_about-me.md
- https://raw.githubusercontent.com/KiFlows/KI-Programm/main/EN/Skill_firma-about.md
- https://raw.githubusercontent.com/KiFlows/KI-Programm/main/EN/Skill_firma-brand-voice.md
- https://raw.githubusercontent.com/KiFlows/KI-Programm/main/EN/Skill_firma-produkte.md
- https://raw.githubusercontent.com/KiFlows/KI-Programm/main/EN/Workspace.md

Steps:
1. Fetch each of the five raw URLs and read the template as the base structure.
2. Fill in each template individually — use EVERYTHING you already know about me, my company, and my writing style.

Output:
- If you can create files: return each filled template as its own .md file (same filename as the template).
- If not: return each filled template as ONE copyable Markdown code block, with the filename as a text line above it — one after another.

Rules:
- Keep the header of each template (the three lines **Internal name** / **Visible name** / **Description**) and fill in the values. Don't turn it into a YAML block.
- In the header lines, ONLY replace the placeholders [Name] / [Company] with the real values — change nothing else. Don't translate proper or company names (Cristina stays Cristina, "My Dream" stays "My Dream").
- The content (everything below the line) is written entirely in ONE language: English. Exception: proper names, company names and fixed terms stay original.
- Replace EVERY [ ] placeholder with real values and remove the brackets. No [ ] may remain — except [PLEASE ADD].
- Where info is missing: do NOT guess. Write [PLEASE ADD] and give me ONE bundled list of questions across all templates at the end.
- Don't change the structure (headings, the three header fields).
- For firma-brand-voice: derive my tone from how I have written to you in our chats — not from generic assumptions.
- For firma-produkte: facts only, no marketing. What you're unsure about → [PLEASE ADD].

Specifics:
- Skill_about-me.md: put EVERYTHING you know about me here — in detail.
- Workspace.md has three parts, keep all short (always active):
  - **Company description** — short description of the company (1 sentence).
  - **About me (short)** — the most important points about me (overlap with about-me is fine).
  - **Model instructions** — how I work with the agents (tone toward me, disagreement welcome, ask before big actions, language, format). This is NOT brand voice (= external presentation) — derive it from how I write to you in our chats and what I ask for.

If a URL can't be fetched: tell me exactly which one, instead of guessing.
