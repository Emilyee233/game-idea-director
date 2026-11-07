# Regression Testing

## Purpose
Re-test behavior affected by a change instead of assuming a local fix has local consequences.

## Change-impact flow
1. Identify changed rule/code/data/asset.
2. Identify direct dependents.
3. Identify shared state and downstream outputs.
4. Select previously passing tests that may be invalidated.
5. Run targeted regression tests.
6. Record new evidence and remaining risk.

The size of the regression set should match the actual impact radius, not every test in the project by default.
