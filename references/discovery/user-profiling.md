# User Profiling

## Purpose

Adapt explanation depth to the user's relevant demonstrated experience. This is a lightweight conversational aid, not a certification or permanent label.

## Independent capability areas

Assess only areas relevant to the current task:

1. Game design.
2. Systems and mathematics.
3. Art and asset production.
4. Technical and programming.
5. Project management.
6. AI collaboration.

## Proficiency levels

- **Unknown:** insufficient evidence; do not infer beginner status.
- **Foundational:** benefits from basic explanations, examples, and guided choices.
- **Working:** can apply concepts with some support.
- **Advanced:** can independently reason about complex trade-offs and edge cases.

## Evidence and confidence

Record the evidence type separately from confidence.

Evidence types:
- **Self-reported:** the user explicitly describes their experience.
- **Observed:** reasoning or decisions demonstrated in conversation.
- **Demonstrated:** work product or task result was provided and inspected.
- **Unverified:** an assumption that has not been checked.

Confidence:
- **Low:** one weak signal, ambiguous wording, or self-report without relevant example.
- **Medium:** multiple consistent signals or one relevant demonstrated task.
- **High:** repeated, relevant demonstrated work across more than one task.

Confidence describes confidence in the assessment, not the user's skill itself. Do not assign High confidence from vocabulary or tool familiarity alone.

## Interaction rules

- Reuse known information.
- Ask only a question that could change the current guidance.
- Do not issue a long questionnaire by default.
- Let the user correct the assessment.
- Update only the relevant capability when new evidence appears.
- A user may be Advanced in art and Foundational in systems design.
- Respect requests for direct professional discussion.

## Minimal profile format

If the user has authorized project-record creation and a persistent profile is useful:

| Domain | Level | Evidence type | Confidence | Notes |
|---|---|---|---|---|
| Game design | Unknown | Unverified | Low | — |
| Systems/math | Unknown | Unverified | Low | — |
| Art/assets | Unknown | Unverified | Low | — |
| Technical/programming | Unknown | Unverified | Low | — |
| Project management | Unknown | Unverified | Low | — |
| AI collaboration | Unknown | Unverified | Low | — |

Do not create or update a file merely because the user asked a question.
