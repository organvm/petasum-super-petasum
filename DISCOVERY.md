# Discovery: organvm/petasum-super-petasum

**Discovered:** 2026-06-24 | **Status:** PROMOTED — real value confirmed

## Value Thesis

`petasum-super-petasum` is the ORGANVM estate's only operational governance audit CLI: a working Python package (`python -m src evaluate|audit|report`) that ingests a registry JSON of repositories and emits cross-organ compliance reports tracking CI health, documentation coverage, and promotion obligations. Its latent value is concrete and twofold — (1) the `governance.py` + `tracker.py` + `report.py` stack can be pointed at the live `registry-v2.json` today and immediately surface which of the 145-repo estate's organs are failing CI or missing docs, converting the logic-first governance framework from philosophy into an operational audit instrument; and (2) `logic-rules.json` encodes the full five-level principle hierarchy as machine-readable structured data, making the governance ruleset directly consumable by agents and automation without parsing prose documents. The GitHub infrastructure layer (nine issue templates, three GitHub Actions workflows, a four-category label taxonomy) is production-ready for adoption as a template across the ORGAN organizations, providing cross-repo issue routing and incident coordination with zero additional implementation. The stub integration with `organvm_engine` is already wired for graceful fallback, meaning the CLI runs standalone now and gains richer audit depth automatically when the engine is available.

## Highest-Value First Task

Wire the audit CLI to the live ORGANVM registry: run `python -m src audit --registry <path-to-registry-v2.json>` against the current estate, identify the top governance failures, and pipe the output into a scheduled report — demonstrating that this tool produces actionable signal, not just structure.
