# AI Agent Workflow

## Purpose
Turn approved work into bounded, auditable tasks for coding or other execution agents.

## Choose the simplest model
- Single agent for bounded work.
- Coordinator + specialists when expertise or file isolation justifies it.
- Multi-agent parallel work only when coordination benefit exceeds conflict cost.

More agents do not automatically mean faster delivery.

## Task contract
Include as relevant:
- Task ID.
- Objective.
- Context.
- Confirmed decisions.
- Input files.
- Dependencies.
- Allowed file scope.
- Prohibited changes.
- Expected deliverables.
- Tests/evidence.
- Acceptance criteria.
- Stop/approval conditions.

## Parallel work
Before parallelizing:
- Check shared files.
- Check shared data/schema.
- Check dependency order.
- Assign integration ownership.
- Define how conflicts are resolved.

## Completion
An execution agent's "done" means submitted for review, not accepted. Require actual change summary, tests/evidence, known issues, and unresolved risks.
