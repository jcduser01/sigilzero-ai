# Documentation index

A routing map from each document to the part of the project it is the source of
truth for. Before completing a change, find the row(s) whose subject your change
touched and update those documents **in the same change** — stale docs are defects.
When you add or remove a document, or add a subsystem, update this index too.

## Top level

| Document | Source of truth for |
|---|---|
| [README.md](README.md) | Project overview, architecture summary, CLI/smoke commands, development setup, adding pipelines, release checklist |
| [IMPLEMENTATION_SUMMARY_STAGE_10.md](IMPLEMENTATION_SUMMARY_STAGE_10.md) | Historical implementation record for Stage 10 (schema migration framework); see `docs/10_schema_versioning_migrations.md` for current architecture |
| [IMPLEMENTATION_SUMMARY_STAGE_11.md](IMPLEMENTATION_SUMMARY_STAGE_11.md) | Historical implementation record for Stage 11 (Langfuse observability); see `docs/11_observability_langfuse.md` for current architecture |
| [IMPLEMENTATION_SUMMARY_PHASE_1.0.md](IMPLEMENTATION_SUMMARY_PHASE_1.0.md) | Historical implementation record and honest status assessment for Phase 1.0 determinism guardrails |
| [STAGE_9_ACTUAL_STATUS.md](STAGE_9_ACTUAL_STATUS.md) | Historical record of Phase 1.0 verification scope corrections and outstanding testing gaps identified at Stage 9 |
| [VERIFICATION_CHECKLIST.md](VERIFICATION_CHECKLIST.md) | Step-by-step verification procedure for all Phase 1.0 determinism invariants (pre-launch checklist) |

## docs/

| Document | Source of truth for |
|---|---|
| [docs/05_generation_modes.md](docs/05_generation_modes.md) | Generation modes subsystem: single/variants/format mode contract, seed derivation, output layout per mode, determinism validation |
| [docs/07_brand_compliance_scoring.md](docs/07_brand_compliance_scoring.md) | Brand compliance scoring pipeline: `phase0_brand_compliance_score.py` interface, snapshot layout, response schema, DoD |
| [docs/08_chainable_pipelines.md](docs/08_chainable_pipelines.md) | Chainable pipeline contract: `prior_artifact.resolved.json` snapshot, chain metadata, determinism guarantees for composed stages |
| [docs/10_schema_versioning_migrations.md](docs/10_schema_versioning_migrations.md) | Schema migration architecture: `migrations.py` framework, `migrate_schemas.py` CLI, version lineage (1.0.0 → 1.2.0), operational procedures |
| [docs/11_observability_langfuse.md](docs/11_observability_langfuse.md) | Langfuse observability integration: `langfuse_client.py` + `observability.py` API, tracing boundary, graceful-degradation contract |
| [docs/12_release_candidate_hardening.md](docs/12_release_candidate_hardening.md) | Stage 12 hardening changes: registry completeness, `smoke_release_candidate_hardening.py` checks, canonical manifest write guarantees |
| [docs/ARCHITECTURE_PHASE_1.0_DETERMINISM.md](docs/ARCHITECTURE_PHASE_1.0_DETERMINISM.md) | Authoritative specification of all 7 determinism invariants: snapshot format, hash algorithm, `run_id` derivation, verification procedures |
| [docs/ARCHITECT_REPORT_PHASE_1.0.md](docs/ARCHITECT_REPORT_PHASE_1.0.md) | Historical architect report for Phase 1.0: structural changes, backward compatibility analysis, verification scope clarification |
| [docs/ARCHITECT_REPORT_STAGE_10.md](docs/ARCHITECT_REPORT_STAGE_10.md) | Historical architect report for Stage 10: migration framework structural changes, determinism preservation proof |
| [docs/ARCHITECT_REPORT_STAGE_11.md](docs/ARCHITECT_REPORT_STAGE_11.md) | Historical architect report for Stage 11: observability enhancements, determinism boundary confirmation |
| [docs/ARCHITECT_STAGE_8.md](docs/ARCHITECT_STAGE_8.md) | Historical architect report for Stage 8: chainable pipeline implementation validation, byte-identical determinism proof |
| [docs/USER_GUIDE.md](docs/USER_GUIDE.md) | Operator guide: job creation patterns, use-case recipes, pipeline composition strategies, how to add new job types |
| [docs/VISUAL_ARCHITECTURE_PHASE_1.0.md](docs/VISUAL_ARCHITECTURE_PHASE_1.0.md) | ASCII diagram reference for the determinism chain (input → snapshot → hash → `inputs_hash` → `run_id`), chaining model, no-silent-drift invariant |
