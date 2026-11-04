# Web Development Learning Lab

This repository documents my hands-on journey learning web development, Git, and an AI-assisted software engineering workflow.

**CampusConnect is a practice project**, not the final Hanfu club website. A production website for a friend's Hanfu club will be planned around the club's real requirements, likely in a separate repository.

## How I learn

Each milestone follows the same loop:

1. **Learn:** Understand one new concept, its purpose, syntax, and common mistakes.
2. **Challenge:** Receive a small, concrete requirement with clear acceptance criteria.
3. **Implement:** Write and test the code myself. Ask for progressive hints when stuck.
4. **Review:** Use ChatGPT and GitHub to inspect the implementation and explain issues.
5. **Summarize:** Write my **own** notes about what I learned and what went wrong; AI can review them, but does not write them for me.
6. **Commit:** Save a meaningful, tested milestone in Git history before moving on.

A commit represents a coherent change, **not** every line edited. Git history preserves earlier versions, while tags can mark larger milestones.

## Learning roadmap

- **Foundations:** HTML, CSS, browser basics, JavaScript fundamentals, and Git/GitHub.
- **Responsive website:** Build a working, mobile-friendly practice site.
- **Interactive website:** Use JavaScript and the DOM to implement actual user interactions.
- **Independent exercises and mini-projects:** Test understanding without copying a complete solution.
- **AI-assisted workflow:** Review diffs, track issues, test, and improve code with AI as a reviewer.

**Future product:** Plan, build, test, and launch the Hanfu club's minimum viable product (MVP) once the requirements are understood. A small preview can be deployed before the official launch.

## Repository layout

```text
learn/
├── README.md
├── .gitattributes
└── projects/
    └── campusconnect/
        ├── index.html
        └── style.css
```

Folders such as `notes/` and `exercises/` will be added **when I create actual content**. Learning notes are written by me. Projects should evolve incrementally instead of copying the entire site into a new `Stage 2` or `Stage 3` folder.

## Working with this repository

- Write code locally in VS Code.
- Inspect changes and create commits with GitHub Desktop.
- Push commits to GitHub; use the history to review progress.
- Use specific commit messages such as `feat: add hero section`, `fix: correct event link`, or `docs: add CSS box-model notes`.
- Let AI teach, challenge, explain, and review—but keep implementation decisions and learning notes in my own hands.

## Current practice project

[CampusConnect](projects/campusconnect/) — a simple HTML/CSS site used for incremental frontend exercises.
