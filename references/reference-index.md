# Reference Index — V1.0

This index lists specialist files included in this release. Paths are relative to `references/`.

`SKILL.md` governs shared behavior, user authority, permissions, privacy, evidence discipline, and status definitions. References provide domain-specific methods.

## Discovery
- `discovery/user-profiling.md`
- `discovery/workflow-routing.md`

## Core game design
- `game-design/core-gameplay.md`
- `game-design/mechanics-and-systems.md`
- `game-design/scope-and-feasibility.md`

## Game types
Load only when type-specific knowledge materially helps. Genre labels are routing hints, not design answers.

- `game-design/game-types/action-combat.md`
- `game-design/game-types/shooter.md`
- `game-design/game-types/survival-crafting.md`
- `game-design/game-types/card-deckbuilding.md`
- `game-design/game-types/strategy-tactics.md`
- `game-design/game-types/simulation-management.md`
- `game-design/game-types/rpg.md`
- `game-design/game-types/roguelike-roguelite.md`
- `game-design/game-types/puzzle-adventure.md`
- `game-design/game-types/narrative.md`
- `game-design/game-types/platformer.md`
- `game-design/game-types/horror.md`
- `game-design/game-types/tower-defense.md`
- `game-design/game-types/stealth.md`
- `game-design/game-types/hybrid-games.md`

## Mathematics
When numerical balance is the primary question, load the relevant mathematics reference before recommending exact tuning.

- `mathematics/balance-framework.md`
- `mathematics/economy-design.md`
- `mathematics/progression-and-curves.md`
- `mathematics/probability-and-randomness.md`
- `mathematics/simulation-and-testing.md`

## Art production
- `art-production/art-direction.md`
- `art-production/asset-planning.md`
- `art-production/asset-specification.md`
- `art-production/asset-integration.md`

## Technical
- `technical/engine-selection.md`
- `technical/architecture-planning.md`
- `technical/technical-feasibility.md`

## Production
- `production/team-roles.md`
- `production/ai-agent-workflow.md`
- `production/project-management.md`
- `production/privacy-and-isolation.md`

## Validation
- `validation/design-validation.md`
- `validation/functional-testing.md`
- `validation/balance-testing.md`
- `validation/playtesting.md`
- `validation/technical-qa.md`
- `validation/asset-qa.md`
- `validation/regression-testing.md`

## Research
- `research/research-methods.md`
- `research/source-evaluation.md`
- `research/competitor-analysis.md`
- `research/research-records.md`

## Routing precedence

1. Route from the user's immediate objective.
2. Choose one primary reference that directly governs the requested outcome.
3. Add type-specific references only when they materially improve the analysis.
4. Add mathematics references when exact numerical judgment, probability, economy, progression, or simulation is central.
5. Add supporting references only for genuine dependencies.
6. Do not profile by default.
7. Do not route by keyword alone.
8. If expertise is absent or current external facts are required, disclose the gap and use suitable current sources/tools when available.

## Common routes

- New game concept → `game-design/core-gameplay.md`; add `discovery/workflow-routing.md` only if the next action is genuinely unclear.
- Define a mechanic → `game-design/mechanics-and-systems.md`; add `game-design/core-gameplay.md` if its role in the player experience is unclear.
- Card cost/damage balance → `mathematics/balance-framework.md` → `game-design/game-types/card-deckbuilding.md`; add probability/simulation only when relevant.
- Survival resource economy → `mathematics/economy-design.md` → `game-design/game-types/survival-crafting.md`.
- Hybrid concept → `game-design/game-types/hybrid-games.md` → relevant type references → `game-design/mechanics-and-systems.md`.
- Asset pipeline → matching `art-production/` references.
- Engine/version-sensitive decision → matching `technical/` reference plus current authoritative documentation when tools permit.
- Agent handoff/project planning → `production/ai-agent-workflow.md` or `production/project-management.md`.
- Claims of completion/quality → matching `validation/` reference and actual evidence.
- Competitor/current-tool research → matching `research/` references.
- Isolated code/engine bug → do not use this Skill as the primary capability.

## Templates, examples, and evaluation

Templates in `templates/` are output formats, not specialist knowledge. Use them when the user wants the corresponding persistent artifact or structured deliverable.

Worked examples in `examples/` are independently fictional demonstrations. Never treat their details as defaults for a user's project.

Files in `evaluation/` are for testing this Skill, not for answering a user's game project.
