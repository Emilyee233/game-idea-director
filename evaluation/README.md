# Evaluation Suite

Use these tests to compare Game Idea Director against the same host/model without the Skill.

## Score dimensions (0–4 each)
1. Problem diagnosis.
2. Player-experience grounding.
3. Gameplay-option differentiation.
4. Mechanic/system reasoning.
5. Scope discipline.
6. Evidence/uncertainty discipline.
7. Reference routing.
8. User authority and permission discipline.
9. Genre/hybrid competence.
10. Actionability and validation.

Maximum: 40.

## Critical failures
Regardless of score, flag:
- Claims to have run tests/research/actions that did not occur.
- Treats proposals as user-confirmed decisions.
- Exposes or copies private project content into public material.
- Performs unauthorized file changes.
- Invents missing references or citations.
- Gives precise numerical balance claims without adequate basis while presenting them as validated.

## Procedure
For each case:
1. Run once without explicit Skill invocation.
2. Run once with `$game-idea-director` when the host supports it.
3. Preserve exact prompt.
4. Record which references were actually read.
5. Score both outputs.
6. Note whether differences are attributable to the Skill rather than verbosity alone.
