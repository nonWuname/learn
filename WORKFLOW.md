# Learning and Git Workflow

## Purpose

The repository is a **learning archive**, not the final Hanfu club product. Stage 1 focuses on HTML/CSS and responsive web design; Stage 2 adds JavaScript and interactive websites; Stage 3 develops testing and deployment skills.

Each stage includes **independent mini-projects**. The production Hanfu club website will be developed separately when its requirements are known; Codex integration is optional.

## Teaching and Assessment Loop

1. **Learn:** ChatGPT teaches one natural, coherent concept in depth, explaining purpose, mechanism, syntax, examples, and common mistakes.
2. **Challenge:** ChatGPT proposes a practical task with explicit acceptance criteria, without supplying a complete solution by default.
3. **Implement:** The learner independently writes and tests the code. ChatGPT supplies progressively stronger hints when requested.
4. **Test and Review:** ChatGPT reviews the implementation and tests understanding with targeted reasoning, code-analysis, or transfer questions. **Do not assess details that have not been adequately taught.** Teach gaps before retesting.
5. **Summarize:** ChatGPT prepares a clear **English** summary grounded in the lesson, the exercise, and any misunderstandings. The learner **reviews, requests changes, and approves** the summary. The learner is no longer required to rewrite long summaries.
6. **Commit:** Make coherent version-control commits with permission, keeping the learner's work under their control.

A lesson is considered mastered only after successfully applying its concepts and passing an appropriate understanding check. A commit records progress but does not itself demonstrate mastery.

## Approval and Editing Rules

- **Discuss before publishing:** Lesson, challenge, and summary drafts should be shown in chat before GitHub publication.
- **Explicit approval is required before every GitHub write or commit by ChatGPT.** Approval is specific to the proposed changes; do not assume permission for later updates.
- ChatGPT can suggest changes to the learner's implementations, but must not directly modify `My-Work/` without clear permission.
- ChatGPT must **not** publish unreviewed or bulk-generated future lessons.
- The learner may request revisions to any GPT-prepared material.
- The learner owns their exercises and independent mini-projects; AI assistance should build understanding rather than replace it.

## Folder Responsibility

| Path | Owner and purpose |
| --- | --- |
| `GPT-Teach/Lessons/` | ChatGPT-prepared teaching notes, published after learner approval |
| `GPT-Teach/Challenges/` | Approved requirements, constraints, and acceptance criteria; no full solutions |
| `GPT-Teach/Summaries/` | ChatGPT-prepared summaries, reviewed and approved by the learner |
| `My-Work/Exercises/` | Learner-written solutions |
| `My-Work/Mini-Projects/` | Independently developed practice projects |
| `My-Work/Summaries/` | Optional learner reflections, not required for lesson completion |

Use English for all text committed to the repository, including lessons, challenges, summaries, READMEs, workflow documents, file names, comments, and commit messages. Chat-based tutoring may use Chinese.

## Commit Message Convention

**Conventional Commit format:** `type: description`.

- `feat` — new functionality
- `fix` — bug fix
- `docs` — documentation or teaching content
- `style` — code formatting only, without behavioral changes
- `refactor` — internal restructuring, same behavior
- `test` — tests
- `chore` — maintenance, organization, or configuration housekeeping
- `build` — build system or dependencies
- `ci` — continuous integration
- `perf` — performance improvement

**GPT rule:** Commit messages written by ChatGPT must be in English and end in `[GPT]`.

Examples:

```text
docs: add HTML introduction lesson [GPT]
docs: publish first HTML challenge [GPT]
feat: complete first HTML page exercise
fix: correct malformed HTML closing tag
chore: organize learning folders [GPT]
```

The **Summary** field in GitHub Desktop contains the short commit subject line. The optional **Description** field can explain details. Neither field is the learning summary.

Prefer **one coherent change per commit**. Do not modify previously recorded history simply to rename old commits.

## GitHub Desktop Workflow

1. Write and run code locally.
2. Inspect modified files and their diffs.
3. Stage or select the intended changes.
4. Enter an English commit Summary.
5. Commit to the current branch.
6. Push to GitHub when ready.
7. If ChatGPT pushed a commit remotely, fetch/pull before working from an outdated local branch. Preserve and reconcile any local uncommitted changes first.

## Publication Safeguard

For each GPT-authored document: **draft → discuss → revise → learner approval → commit**. No approval, no GitHub write.
