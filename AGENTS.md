# AGENTS.md — jokes

How to work in this repo. See `README.md` for what this project is.

Read `THE_LIST.md` (the master joke list — the project's deliverable and state file) before answering questions or making edits.

---

## State File

`/THE_LIST.md` — the numbered master list of jokes in Markdown format. This is the source of truth.

## Hard Rules

- Nothing gets added to the list without explicit user approval.
- Nothing gets removed from the list without explicit user approval.
- When new jokes are proposed — whether by the user or by the model — number them as candidates and wait for approval before adding.
- When jokes are approved, append them to the list immediately and update the running count at the bottom.
- Remove duplicates silently during batch imports; flag only if uncertain.
- Jokes can be any category: clean, dark, adult, dad jokes, etc. Follow the user's lead on tone.
- When the user asks for jokes from the list (e.g. "top 5", "family friendly only"), filter and present from the existing list — do not invent new ones unless asked.

## Candidate Workflow

1. Propose a labeled batch of ~10–12 candidate jokes (A–L or similar).
2. User selects by letter.
3. Append approved jokes to THE_LIST, update the running count, confirm additions.

Lars typically approves 3–7 per batch. Quality over quantity.

## Humor Profile

Lars's aesthetic: clever misdirection, dark one-liners, edgy-but-not-cruel. His own framing: "dark and bordering on evil but not cruel." Clean and dad jokes are included but as distinct tiers, not the primary flavor.

Audience tiers to keep in mind when filtering on request:
- **Family/younger child** — clean and dad joke tiers only
- **Dark-humor-loving child** — dark one-liners acceptable
- **Teenager** — broader range

## Edit Conventions

- Read before editing; batch edits per file; preserve blank lines between headings and list elements.
- Branch + PR; never commit to main. Main is branch-protected.
- No manual version numbers in file content — git is the history.

## Execution

Model-tiered: plan with a strong model, execute with a fast one. The content here is prose and list management, not code. Simple edits can happen inline.
