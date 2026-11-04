# Learning and Git Workflow

## Lesson loop

1. **Discuss:** ChatGPT teaches one coherent concept and discusses questions with the learner.
2. **Challenge:** ChatGPT proposes a small practical requirement and objective acceptance criteria. No full solution by default.
3. **Implement:** The learner writes and tests the code independently.
4. **Review:** ChatGPT inspects the learner's changes and gives progressively stronger hints when needed.
5. **Summarize:** The learner writes their own summary. ChatGPT may review it, but must not silently rewrite it.
6. **Record:** Meaningful changes are committed and pushed by the appropriate contributor.

## Approval policy for ChatGPT

- ChatGPT **must discuss draft lesson materials and practice requirements before writing them to GitHub**.
- ChatGPT **must receive explicit approval before every GitHub commit or file mutation it performs**.
- Approval of one change does not automatically authorize later changes.
- ChatGPT must not alter the learner's exercise solutions or personal summaries without explicit approval.
- Lessons and challenges are published one coherent unit at a time, not bulk-generated ahead of instruction.

## Commit messages

- All ChatGPT-created commit messages must be in English and end with **`[GPT]`**.
- Example: `docs: add HTML document structure lesson [GPT]`
- Learner-authored commits use clear English messages without the suffix unless desired.
- Do not rewrite earlier Git history merely to rename old commits.

## Directory ownership

- `GPT-Teach/Lessons/`: lesson content approved by the learner.
- `GPT-Teach/Challenges/`: approved practice specifications, constraints, and acceptance criteria; no answer key by default.
- `My-Work/Exercises/`: independent exercise submissions.
- `My-Work/Mini-Projects/`: independent stage projects.
- `My-Work/Summaries/`: learner-written notes and reflections.

Empty directories contain `.gitkeep` placeholders only to make the skeleton visible in Git.
