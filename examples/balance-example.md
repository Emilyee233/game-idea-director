# Worked Example: Card Balance Without False Precision

> Fictional example.

## Question
Card A costs 2 energy and deals 12 damage. Card B costs 3 and deals 20. Is B overpowered?

## Bad answer
“12/2 = 6 and 20/3 = 6.67, so B is 11% too strong. Set it to 18 or 19.”

Why this is weak: it treats one efficiency ratio as proof and invents an exact tuning value.

## Better analysis
Known:
- A = 6 damage per energy.
- B ≈ 6.67 damage per energy.

Unknown but material:
- Energy per turn.
- Draw/hand constraints.
- Whether high cost consumes an entire turn.
- Enemy health breakpoints.
- Overkill.
- Card roles and rarity.
- Synergies and repeated triggers.

If a turn has exactly 3 energy, B's higher efficiency may compensate for inflexibility. If a turn has 10 energy and cards chain freely, the same premium may be excessive.

## Next step
Ask for the highest-value missing context, then establish a test range rather than pretending 19 is intrinsically correct.

## Validation
Formula comparison → representative encounter/deck simulation → human playtest.
