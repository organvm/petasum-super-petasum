# Discovery: organvm/petasum-super-petasum

**Discovered:** 2026-06-24  
**Status:** PROMOTED — real value confirmed

## Value Thesis

`petasum-super-petasum` is the governance backbone of the ORGANVM estate — not merely a policy document but a working Python CLI (`evaluate`/`audit`/`report`) that ingests a repository registry JSON and produces structured CI health and documentation coverage reports per organ, backed by a machine-readable 16-principle hierarchy (`logic-rules.json`), an `ObligationTracker` dataclass for cross-organ promotion duties with due-date and overdue detection, and a full set of GitHub issue templates plus Actions workflows for real-time cross-repo incident coordination. Its highest latent value is as an **active governance enforcement layer**: the `GovernanceReport` + `ObligationTracker` engine already exists and passes all 37 tests; what is missing is the wire between the CLI and the live ORGANVM registry. Once connected, this becomes the estate-wide compliance monitor that can fail CI, post audit summaries on PRs, and surface overdue cross-organ obligations across all 89 active repositories — a capability no other organ currently provides.

## Highest Latent Value

The combination of machine-readable governance rules (`logic-rules.json`), a pluggable `organvm_engine` integration hook, and a report-to-markdown pipeline is the foundation for an estate-wide governance dashboard. Every promotion decision, CI failure, and documentation gap in the 145-repo system can flow through this single audit surface.

## Best First Task

Add a GitHub Actions workflow (`governance-audit.yml`) that runs `python -m src audit --registry <path-to-registry>` on a nightly schedule and on PRs to `main`, posting failures as issue comments — converting the passive policy spec into a live enforcement gate for the entire ORGANVM estate.
