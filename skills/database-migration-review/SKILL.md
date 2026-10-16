---
name: database-migration-review
description: Plan and review database schema or data migrations for safety, compatibility, and rollback. Use when changing columns, indexes, constraints, data shape, or persistence behavior in an active application.
---

# Database Migration Review

## Understand the deployment model
Identify the database engine, migration framework, table sizes, traffic patterns, replication setup, and whether application versions overlap during deployment. Verify these facts rather than assuming the environment.

## Migration workflow
1. Inspect schema definitions, existing migrations, query patterns, and relevant data models.
2. Describe the desired schema and data invariant.
3. Classify the change as additive, backfill, constraint tightening, rename/removal, or potentially blocking operation.
4. Consider old and new application versions running at the same time.
5. Estimate lock duration, table rewrite, index build, storage, and backfill costs using database-specific behavior.
6. Define validation queries and monitoring signals before rollout.

## Safer rollout patterns
- Prefer expand-and-contract for changes that need application compatibility across deployments.
- Add new fields or tables before switching readers and writers.
- Backfill in bounded, restartable batches with progress tracking and rate limits.
- Validate the backfill before making the new representation authoritative.
- Remove obsolete schema only after all deployed consumers have stopped using it.
- Use database-native online or concurrent operations where supported and appropriate.

## Rollback and data integrity
A schema rollback does not necessarily restore changed or deleted data. Distinguish code rollback from data recovery. Define backup, restore, and forward-fix plans for destructive changes. Check constraints, uniqueness, nullability, foreign keys, and transaction boundaries.

## Verification checklist
- [ ] Migration applies to a representative schema.
- [ ] Existing and new application versions remain compatible during rollout.
- [ ] Data invariants and row counts are validated.
- [ ] Failure midway can be detected and safely resumed or recovered.
- [ ] Query plans and indexes are reviewed for important paths.
- [ ] Deployment and rollback instructions are documented.

Never execute a destructive migration against a live database without explicit authorization and an understood recovery plan.
