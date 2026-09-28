# Reframe Readiness

A static GitHub Pages checklist adapted from the supplied Reframe readiness brief. Public source contains the generic checklist and supplied rule snapshot, not private repository drafts, research files, credentials or user edits. No backend or build dependencies.

## Run

`npm start` then open http://127.0.0.1:4173. Run logic checks with `npm test` (Node 26 tested).

## Features

66 populated tasks across pitch, pilot, invited proposal, pre-award and later work; owner/status/stage filters; task steps, evidence references, review, reopen and audit history; deterministic next actions; four autosaved pitch editors with Unicode counts and version checkpoints; source registry; engineering snapshot import; claim and engagement records; print; light/dark layouts; complete JSON export and explicit per-record conflict merge.

Progress is transactional IndexedDB state in each browser. Seed changes do not erase saved progress. Export backups regularly. Import preserves a pre-restore recovery copy in IndexedDB. Profiles are authorship labels, not authentication. Different devices and browser profiles do not synchronize. Other applications on the same web origin can potentially access browser storage; do not store secrets or sensitive participant data.

## Scope adaptations and remaining checks

GitHub Pages cannot host the brief's Node/SQLite service. This implementation uses browser storage, not SQLite, and has no server restart requirement. Existing private pitch text can be imported manually as Markdown with four numbered `##` headings; it is never committed to the public repository. No engineering snapshot existed at implementation time. Historical readout figures are explicitly unverified for the current app.

Rules from the supplied September 28, 2026 snapshot remain owner-review items. The official pitch headings and limits were checked during implementation. The tool does not calculate legal eligibility, invitation deadline windows, regulatory determinations or research authorization. It does not submit applications or contact people. It provides the requested hosted checklist, not every feature of the document's local planning-server specification. Manual VoiceOver validation remains outstanding.

## Deployment

Dedicated GitHub repository, main branch root deployed with GitHub Pages. `.nojekyll` disables Jekyll processing. All assets use relative paths.
