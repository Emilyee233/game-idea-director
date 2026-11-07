# Architecture Planning

## Purpose
Translate confirmed game requirements into maintainable technical boundaries without overengineering early prototypes.

## Start from requirements
Identify:
- Core runtime states.
- Persistent data.
- High-change design data.
- Major systems and ownership.
- Communication between systems.
- Save/load boundaries.
- Content configuration needs.
- Testing seams.

## Prefer data-driven design when
Designers or content creators need to add content without changing code, values change frequently, or many instances share common rules.

Do not make everything data-driven by default; additional abstraction has cost.

## Boundaries
For each major module clarify:
- Responsibility.
- Inputs/outputs.
- Owned state.
- Public interface/events.
- Dependencies.
- Failure behavior.

Avoid circular dependencies and "god" managers that own unrelated responsibilities.

## Prototype architecture
For an early prototype, optimize for clarity, changeability, and testability rather than hypothetical scale. Record shortcuts that must be revisited before production.
