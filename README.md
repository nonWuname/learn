# Web Development Learning Lab

A stage-based learning repository built around **understanding concepts, implementing small requirements independently, reviewing results, and preserving progress through Git**.

## Learning Roadmap

| Stage | Scope | Outcome |
| --- | --- | --- |
| **Stage 1 — Responsive Web** | HTML, CSS, responsive design | Independent responsive websites and mini-projects |
| **Stage 2 — Interactive Web** | JavaScript fundamentals, DOM, events, browser APIs | Independent interactive web applications and mini-projects |
| **Stage 3 — Deployment** | Testing, builds, hosting, release workflows | Publish and maintain the projects developed earlier |

Git, debugging, and code review are practiced throughout the stages, not postponed until Stage 3.

**The real Hanfu club website is a separate future product repository**, based on the club's actual requirements. Tools such as Codex may be integrated when appropriate.

## Repository Structure

```text
learn/
├── README.md
├── WORKFLOW.md
├── .gitattributes
├── Stage1-Responsive-Web/
│   ├── GPT-Teach/
│   │   ├── Lessons/
│   │   ├── Challenges/
│   │   └── Summaries/
│   └── My-Work/
│       ├── Exercises/
│       ├── Mini-Projects/
│       └── Summaries/
├── Stage2-Interactive-Web/
│   └── ...
└── Stage3-Deployment/
    └── ...
```

Folders are populated **as lessons are discussed and approved**. Placeholder `.gitkeep` files only preserve otherwise empty directories in Git.

- **GPT-Teach/Lessons:** Approved teaching references.
- **GPT-Teach/Challenges:** Approved practical tasks and acceptance criteria, without complete answers.
- **GPT-Teach/Summaries:** AI-drafted English study summaries, reviewed and approved by the learner.
- **My-Work/Exercises:** Learner-written solutions.
- **My-Work/Mini-Projects:** Independent stage-level projects.
- **My-Work/Summaries:** Optional learner-authored reflections; writing lengthy summaries is **not** a requirement for passing lessons.

## Study and Review Principles

**Learn → Challenge → Implement → Test & Review → Approved Summary → Commit**

- Lessons explain *why* concepts work, not just their syntax.
- Challenges specify one manageable practical task with verifiable requirements.
- The learner writes the code; AI gives progressive hints and reviews it.
- Tests assess **understanding and transfer**, using only adequately taught knowledge.
- ChatGPT drafts the study summary in **English**; the learner reviews it and may request revisions.
- **No GitHub edits or commits by ChatGPT without explicit learner approval.** Approval for one commit does not extend to later commits.

All repository documents, filenames, code comments, and commit messages should be in English. Explanations during live tutoring may be in Chinese.

## Git Commit Convention

This repository follows a practical subset of **Conventional Commits**.

**Format:** `type: short description`  
**For GPT-authored commits:** `type: short description [GPT]`

| Type | Meaning | Example |
| --- | --- | --- |
| `feat` | Add a feature or new functionality | `feat: complete first HTML page exercise` |
| `fix` | Fix incorrect behavior | `fix: correct navigation link` |
| `docs` | Add or revise documentation | `docs: add HTML introduction summary [GPT]` |
| `style` | Formatting changes that do not affect behavior | `style: format HTML indentation` |
| `refactor` | Change code structure without changing behavior | `refactor: simplify event handlers` |
| `test` | Add or update tests | `test: add form validation tests` |
| `chore` | Maintenance and repository organization | `chore: organize stage folders [GPT]` |
| `build` | Build system or dependencies | `build: update build configuration` |
| `ci` | Continuous integration workflow | `ci: add automated checks` |
| `perf` | Performance improvements | `perf: optimize image delivery` |

**Notes:**
- A **coherent commit** contains one logically related set of changes.
- `chore` means maintenance work; it is **not** short for `coherent`.
- `style` in this convention generally means formatting, not a website's visual redesign; feature-related visual changes can use `feat`.
- GitHub Desktop's **Summary** field is the commit subject line, **not** the learning summary.
- ChatGPT-authored commits must use **English** and end with **`[GPT]`**. Learner commits do not need that suffix.
- Commit messages should describe what changed; do not rewrite old Git history to rename existing commits.

Examples:

```text
docs: add HTML document structure lesson [GPT]
docs: add first HTML challenge [GPT]
feat: complete first HTML page exercise
docs: add HTML introduction summary [GPT]
```

For the full approval, ownership, and review policy, see [WORKFLOW.md](WORKFLOW.md).

## Current Material

- [Lesson 1.1 — HTML Introduction & Document Structure](Stage1-Responsive-Web/GPT-Teach/Lessons/01-html-introduction.md)
- [Challenge 1.1 — First HTML Page](Stage1-Responsive-Web/GPT-Teach/Challenges/01-first-html-page.md)
- [Lesson 1.1 — Reviewed Summary](Stage1-Responsive-Web/GPT-Teach/Summaries/01-html-introduction.md)
