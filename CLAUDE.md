# Project instructions

## Required context

- Read `docs/00-index.md`, `docs/01-context-projecte.md`, `docs/02-decisions-i-pendents.md`, and `docs/03-inici-desenvolupament.md` before architecture or functional work.
- All explanatory development context belongs in versioned `docs/`. A fresh clone is sufficient to start technical design; access to the project Page or local business documents is not required.
- `info/` is ignored and contains only real documents such as invoices, debit notes, payment notices, original emails and attachments. Do not store requirements, decisions, plans or instructions there.
- If real samples are unavailable, work on design or synthetic examples. Request specific documents only when a task depends on them.
- Distinguish original client requirements, confirmed agreements, proposals and assumptions. Do not promote a proposal to an agreement without confirmation.

## Scope and development

- Marino is the final operational system. The first proposed delivery covers phases 1 to 4, without an AI dependency.
- Initial ingestion is headless. Preserve original emails and attachments outside SQL; register metadata, processing state and file references in SQL from the start.
- Marino's update mechanism for auxiliary SQL records remains unvalidated.
- Documentary reconciliation does not establish bank settlement, business approval or accounting generation. Phases 5 to 7 are later evolution.
- Do not assume a SQL engine, mail platform, hosting provider, implementation stack or AI provider is confirmed.
- Before implementation, state the requirement covered, dependencies and acceptance criteria.
- Use synthetic data and simulated adapters for unavailable systems; do not claim they validate real integration.
- Preserve traceability and retry behavior. Add relevant behavioral tests for repeated ingestion, partial failures, relationships and corrections when implementing those features.
- Document actual setup, build, run and verification commands once implementation exists.

## Documentation and Git

- Maintain functional context and business decisions in Catalan. Write new technical design and code identifiers in English.
- `docs/01-context-projecte.md` is the consolidated functional baseline. Other documents index, guide or detail it; avoid contradictory copies.
- Record new decisions with date, status and rationale. Keep unresolved choices explicit.
- Keep `info/`, real files and secrets out of commits; never force-add them.
- Record newly agreed context in `docs/` and reconcile it with the review Page. Synchronization is manual.
- Do not require `CLAUDE.local.md` or untracked context files to understand the project.
