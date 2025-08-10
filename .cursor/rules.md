# Cursor Rules

- Maintain `@memories.md`, `@lessons-learned.md`, and `@scratchpad.md` continuously.
- Follow the Mode System and Scratchpad Management protocols defined in `cursorrules 2.txt`.
- Keep artifacts under version control.

## Files
- `@memories.md`: chronological, one-line entries per interaction; create overflow files when >1000 lines.
- `@lessons-learned.md`: one-line comprehensive entries with timestamp, category, issue → solution → why, plus tags.
- `@scratchpad.md`: active task tracker using required structure and status markers.
- `docs/project-requirements.md`: source of truth for requirements; warn if missing/incomplete.
- `docs/phases/PHASE-X/`: archive per phase with feature docs.

## Mode System
- Plan Mode: create a new chat session section in `@scratchpad.md` with Current Task, Understanding, Questions, Confidence, Next Steps.
- Processing Steps: parse requirements, cross-reference, generate ≥3 questions, compute confidence, task breakdown, iterate until ≥95%.
- Agent Mode: activate only when confidence ≥95%, questions answered, tasks defined, no blockers, requirements verified. Enables code edits, file ops, commands, system changes, scratchpad updates.

## Scratchpad Management
- Required structure with Tasks list and status markers: [X], [-], [ ], [!], [?].
- Unique task IDs, real-time updates, dependencies, timestamps, cross-references.
- Phase transitions: archive to `docs/phases/PHASE-X/`, init new phase, transfer relevant tasks, update confidence.

## Enforcement
- Always validate work against `docs/project-requirements.md` before changes. Emit warnings if incomplete.

## Accessibility, Quality, and Style
- Write clean, maintainable, TypeScript-friendly code with explicit types, early returns, and clear names. Include ARIA/keyboard/focus management where applicable. Mobile-first responsive design, robust error handling, performance and SEO mindful.

## Problem-Solving
- Use structured reasoning to identify root causes during bugs/issues. Cross-reference memory, lessons, and requirements.