# AGENTS.md

## Project

Personal resume/portfolio site (David Barratt). Content is Markdown in the repo root — no build system, no tests. Output is correct when it reads correctly.

## Task Splitting

Multi-step pipelines (e.g. `/resume tailor`) fail when a **single response** tries to think through and emit the whole task at once — that response truncates mid-task. Truncation is a response-level failure, not a task-level one. The fix is to chunk work per response while continuing autonomously per request.

1. **Work to completion.** A multi-step task is one request, not many. Keep executing across successive responses without waiting for user input: do the next step, persist output, update the checklist, continue. Only stop when the task is done, genuinely blocked, or the user's input is required.
2. **Chunk per response, not per request.** Each assistant response does at most one pipeline step (or one section of a large artifact): bounded reasoning, one tool action, brief status. Never do an entire pipeline's thinking plus output in one message — that is what truncates.
3. **Files are the handoff.** Write each step's output to a working file before starting the next step. Never carry a step's result only in chat history.
4. **Keep chat output small.** Never paste a full resume, full analysis, or large report into the reply — write it to a file and state the path. Target: under ~100 lines of chat text per response.
5. **Build large files in chunks.** Write the first section of a big artifact, then append section by section across successive responses.
6. **Track progress on disk.** Keep a checklist of all pipeline steps in the working file; check each off as it completes. If a native todo tool is available in the session, mirror the checklist there for live visibility — but the disk file remains authoritative, because it survives truncation and restarts while in-session state does not. The disk checklist is the recovery mechanism: if a response truncates or a session restarts, read it and continue at the first unchecked step — don't re-derive.
7. **Stop cleanly only when interrupted.** If a step runs long, finish it, update the checklist, state what remains in one line, then resume immediately — never end a request with unrecorded work.

## Pipeline Conventions

- Working artifacts go in `.work/` (e.g. `.work/status.md`, `.work/gap-analysis.md`) and are deleted when the task completes.
- `RESUME.md` is the source of truth — never edit it while tailoring.
- Tailored resume output goes to `david-barratt.md` (or the path the user names).
- On resumption, the only things needed are `.work/status.md` and the step outputs already on disk — re-read them, don't re-derive.
