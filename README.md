# devcard.md — Open Standard Specification
> Version 0.1 — Proposed by the community, for the community

---

## What is devcard.md?

`devcard.md` is an open standard for a developer's personal identity file.

It lives in your GitHub (Gist or repo), travels with you across every AI tool you use, and tells any AI assistant exactly **who you are, how you work, and how to talk to you** — so you never have to explain yourself again.

Think of it as your **developer passport**. One file. Every tool. Every time.

---

## The Problem

Every AI tool you use starts from zero.

- You re-explain your stack. Again.
- You re-explain your code style. Again.
- You re-explain your preferences. Again.
- The AI calls you "user" when your name is Z.

There are already standards for *project* context (`CLAUDE.md`, `AGENTS.md`, `copilot-instructions.md`) — but nothing for **the human behind the keyboard**.

`devcard.md` fixes that.

---

## How It Works

1. You create your `devcard.md` file once
2. You push it to a public GitHub Gist or repo
3. Any AI tool reads it via the raw GitHub URL
4. The AI now knows you — your vibe, your name, your style
5. You never onboard yourself again

---

## The Standard Schema

```markdown
# devcard.md

## Identity
- Name: [Your full name]
- Call me: [What you want the AI to call you]
- Role: [e.g. Full Stack Developer, ML Engineer, Indie Hacker]
- Based in: [City / Country — optional]
- GitHub: [your handle]

## My Stack
- Primary languages: [e.g. TypeScript, Python]
- Frameworks: [e.g. Next.js, FastAPI]
- Databases: [e.g. PostgreSQL, Redis]
- Cloud: [e.g. AWS, Vercel]
- Tools I live in: [e.g. VS Code, Cursor, Neovim]

## My Vibe
- Working style: [e.g. Move fast, figure it out later]
- Strength: [e.g. Seeing the big picture, system design]
- Weakness: [e.g. I skip documentation, perfectionism on UI]
- I like: [e.g. Direct answers, no fluff, bullet points]
- Don't: [e.g. Over-explain basics, add boilerplate I didn't ask for]

## Code Style
- Indentation: [tabs / 2 spaces / 4 spaces]
- Naming conventions: [e.g. camelCase JS, snake_case Python]
- Comments: [e.g. Only when non-obvious]
- Commit style: [e.g. Conventional Commits]
- PR style: [e.g. Small PRs, draft early]

## AI Preferences
- Tone: [e.g. Technical peer, not a tutor]
- Response length: [e.g. Concise — lead with the answer]
- Code output: [e.g. Always include types, no placeholder comments]
- When I'm stuck: [e.g. Ask me one question, not five]
- Celebrate wins: [yes / no / sometimes]

## Currently Working On
- [Brief description of your current project or focus]

## Fun Facts (optional)
- [Something that makes you human — the AI remembers this]
```

---

## Rules of the Standard

1. **The file is called `devcard.md`** — lowercase, exact name
2. **It lives at the root** of your Gist or a dedicated repo
3. **All sections are optional** — use what's useful to you
4. **It's human-readable AND AI-readable** — that's the point
5. **You own it** — it's your file, your data, your identity
6. **Keep it honest** — the AI works better when it knows the real you
7. **Version it** — update it as you grow

---

## For AI Tool Builders

To support `devcard.md` in your tool:

1. Let users input their raw GitHub Gist or repo URL
2. Fetch the raw `devcard.md` content at session start
3. Inject it as system context before the first message
4. Reference the user's preferred name throughout
5. Adapt tone, depth, and style to their stated preferences

That's it. No SDK. No API. Just markdown.

---

## Why Markdown?

- Every developer already writes it
- GitHub renders it as a beautiful profile card
- AI tools consume it natively
- No syntax errors from a missing bracket
- It's readable by humans AND machines
- It can evolve without breaking parsers

---

## Contribution

This is an open standard. It belongs to the community.

- Propose changes via GitHub Issues
- Fork and experiment
- Implement it in your tool and add it to the adopters list
- Share your `devcard.md` publicly to grow the movement

---

## The Vision

Every developer has a vibe.
Every developer has a name.
Every developer has strengths, weaknesses, a style, and a story.

AI tools should know that from day one — not day never.

`devcard.md` is the layer that makes AI tools feel like teammates, not strangers.

---

*"Write it once. Work with every tool. Be known everywhere."*

---

**Repository:** github.com/bukscom/devcard-spec  
**Status:** Proposal — v0.1  
**License:** MIT  
**Author:** bukscom
