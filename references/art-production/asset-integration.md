# Asset Integration

## Purpose
Verify that an approved-looking asset actually works in the target game environment.

## Integration checks
As relevant:
- Import settings and compression.
- Actual pixel density and scale.
- Pivot/anchor.
- Layer order and occlusion.
- Masks, collision, hit areas, or navigation.
- Animation setup.
- Nine-slice or atlas behavior.
- Material/shader behavior.
- Resolution/aspect-ratio behavior.
- Memory/performance impact.
- References and missing-file behavior.

## Three independent approvals
Keep separate:
1. **Visual QA** — looks correct.
2. **Technical Asset QA** — file/structure/specification is correct.
3. **Integration QA** — behaves correctly in the game.

Passing one does not imply the others.

## Change impact
Replacing an asset may affect pivots, masks, collision, animation, layout, references, or gameplay readability. Inspect dependent systems before treating replacement as cosmetic.
