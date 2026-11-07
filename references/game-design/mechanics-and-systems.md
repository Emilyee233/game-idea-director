# Mechanics and Systems Framework

## Purpose

Derive mechanics and systems from intended player experience and gameplay. Avoid feature lists based only on genre conventions.

## Distinguish the concepts

- **Player action:** what the player does.
- **Mechanic:** a rule governing an action, state change, condition, or outcome.
- **Core gameplay:** the main repeated player activity and its intended engagement.
- **Gameplay loop:** a recurring sequence of actions and feedback, where applicable.
- **System:** a coordinated set of rules, mechanics, and state that manages a meaningful part of the game.
- **Content:** concrete instances such as cards, enemies, items, levels, or events.
- **Presentation:** visual, audio, animation, and UI communication.
- **Implementation:** code, data structures, engine components, and technical architecture.

A mechanic does not always require a separate system. Do not split systems merely to make documentation look comprehensive.

## Derivation

Use this flexible chain:

Player experience → player actions → mechanics → core gameplay and applicable loops → systems → content and presentation → implementation considerations → validation.

This is iterative. Technical constraints, content cost, and test results may require revisiting earlier decisions.

## Mechanic analysis

For a significant mechanic, define as needed:
- Purpose.
- Player action or trigger.
- Preconditions.
- Rules and resolution.
- Inputs and outputs.
- State changes.
- Constraints and edge cases.
- Feedback to the player.
- Related mechanics and systems.
- Content or asset needs.
- Technical considerations.
- Testable acceptance criteria.

## System role — classify what the system does

These are role categories, not scope decisions:

- **Core:** directly enables or governs core gameplay.
- **Supporting:** provides necessary support to core gameplay.
- **Expansion:** adds depth or additional content.
- **Meta:** manages progression or state across sessions, levels, or runs.

A system can have one or more relevant roles if the design genuinely warrants it. Explain the role rather than forcing a label.

## Current scope decision — classify whether to build it now

This is a separate dimension:

- **Essential:** required for the current agreed milestone.
- **Optional:** useful but not required.
- **Conditional:** required only if a stated design condition applies.
- **Deferred:** intentionally postponed.

Examples:
- A Meta system may be Essential to a prototype whose main premise is persistent cross-run progression.
- A Core system may be Deferred if the first experiment isolates another central mechanic.

Never combine system role and scope decision into one mutually exclusive list.

## System specification

For a significant system, capture:
- Purpose and player-experience goal.
- Related gameplay and mechanics.
- Inputs, outputs, rules, and state.
- Dependencies and affected systems.
- Content and assets.
- Important numerical parameters.
- Constraints and edge cases.
- Technical considerations.
- Acceptance criteria.
- Validation method.

Use proportionate detail. A simple system does not need an enterprise-scale specification.

## Dependency relationships

Use these relationships when they clarify design:

- **Depends on:** one system requires another.
- **Feeds into:** one system's output becomes another's input.
- **Influences:** changes in one system affect another.
- **Shares data with:** systems use common state or data.

When a major rule changes, inspect affected systems, content, assets, implementation, tasks, and tests.

## System necessity test

Before adding a system, ask:

1. What player-experience or gameplay need does it serve?
2. Which mechanic or activity does it support?
3. What changes if it is removed?
4. Can an existing system already provide the behavior?
5. What content, technical work, and maintenance does it add?
6. Is it needed for the current milestone?

Do not add inventory, quests, crafting, equipment, progression, economy, achievements, or other familiar systems automatically.

## Hybrid and unfamiliar games

Analyze the mechanics and player activities that make up the combination. Identify:
- The primary experience.
- Supporting activities.
- Shared resources or state.
- Interactions between mechanics.
- Conflicting incentives or pacing.
- The riskiest combination to prototype.

If the combination does not fit an established genre, describe the mechanics directly rather than forcing a label.

## Validation

For each critical mechanic or system, define a testable question. Distinguish theoretical coherence from observed player behavior and implemented results.

Do not claim a system is fun, balanced, or validated without relevant evidence.
