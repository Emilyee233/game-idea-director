# Workflow Routing

## Purpose

Choose the next useful action without forcing a rigid production sequence.

## Keep three dimensions separate

### 1. User capability

Relevant domain proficiency and evidence. See `user-profiling.md`.

### 2. Project work areas

- Concept and audience.
- Gameplay and mechanics.
- Systems and content.
- Mathematics and balance.
- Art and assets.
- Technical design.
- Production and coordination.
- Prototype and validation.

These are parallel areas of work, not sequential stages.

### 3. Work-area status

Use one primary maturity status where appropriate:

- **Not Started:** no meaningful work yet.
- **Exploring:** alternatives or requirements are being investigated.
- **Drafted:** a proposal or specification exists but is not approved.
- **Confirmed:** the user has approved the relevant design.
- **Implemented:** the planned work has been implemented.
- **Tested:** a relevant test has been executed and recorded.
- **Accepted:** the agreed acceptance criteria have been met and the authorized reviewer has accepted the result.

Track blockers separately as a flag or note. A work area can be Implemented and Blocked from testing, for example. Do not force blocker status into the maturity sequence.

Decision, task, and test statuses remain separate and are defined in the main `SKILL.md`.

## Routing procedure

1. Identify the user's immediate objective.
2. Identify the primary work area.
3. Identify supporting areas only if the task depends on them.
4. Check relevant confirmed decisions and constraints.
5. Identify missing prerequisites that could materially change the answer.
6. Decide whether to answer, ask a key question, propose, research, prepare a task, or evaluate evidence.
7. Select the smallest useful set of existing references.
8. State assumptions and the next deliverable when useful.

## Primary-reference selection

Choose the reference that directly governs the requested outcome:

- Player actions, decisions, and engagement → `core-gameplay.md`.
- Rules, mechanics, state, system roles, and dependencies → `mechanics-and-systems.md`.
- Scope, feasibility, and prototype boundaries → `scope-and-feasibility.md`.
- User experience affects explanation depth → `user-profiling.md`.

Add supporting references only when needed. For a request spanning several areas, state the primary question first and then address dependencies in order.

## When to ask or proceed

Ask when different answers would materially change the design, permission, or risk.

Proceed with a stated assumption when it is low-risk and reversible.

Pause for clarification or approval when missing information creates material technical, financial, privacy, scope, or irreversible-change risk.

## Direct entry and iteration

Users may enter any work area directly. Do not require earlier documents to be completed first.

Return to an earlier design question when evidence reveals a material flaw. Explain why.

## Routing output

Do not expose a long internal checklist on every turn. When helpful, briefly state:
- The immediate objective.
- The primary work area.
- A material prerequisite or uncertainty.
- The proposed next action.
- The expected output or evidence.
