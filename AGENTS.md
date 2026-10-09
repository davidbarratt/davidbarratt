# AGENTS.md

## Project

Personal resume/portfolio site (David Barratt). Content is Markdown in the repo root — no build system, no tests. Output is correct when it reads correctly.

## Task Splitting

Multi-step pipelines (e.g. `/resume tailor`) fail when executed in one turn: the response truncates mid-task. Split by default.

1. **One step per turn.** If a task has steps, do exactly one per reply: run it, persist its output to a file, report a one-line status, stop.
2. **Files are the handoff.** Write each step's output to a working file before starting the next step. Never carry a step's result only in chat history.
3. **Keep chat output small.** Never paste a full resume, full analysis, or large report into the reply — write it to a file and state the path. Target: under ~100 lines of chat text per turn.
4. **Build large files in chunks.** Write the first section of a big artifact, then append section by section across turns. One section per turn is fine.
5. **Track progress on disk.** Keep a checklist of all pipeline steps in the working file; check each off as it completes. When resuming, read the checklist and continue at the first unchecked step.
6. **Stop cleanly if running long.** Finish the current step, update the checklist, state what remains in one line. Never end a turn with unrecorded work.

## Pipeline Conventions

- Working artifacts go in `.work/` (e.g. `.work/status.md`, `.work/gap-analysis.md`) and are deleted when the task completes.
- `RESUME.md` is the source of truth — never edit it while tailoring.
- Tailored resume output goes to `david-barratt.md` (or the path the user names).
- On resumption, the only things needed are `.work/status.md` and the step outputs already on disk — re-read them, don't re-derive.
