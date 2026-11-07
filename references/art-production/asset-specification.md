# Asset Specification

## Purpose
Make an asset request concrete enough to produce, review, and integrate.

## Specification fields
Use only applicable fields:
- Asset ID and name.
- Gameplay purpose.
- Asset category.
- Visual reference and exactly what is referenced.
- Dimensions/aspect ratio.
- Camera/view and orientation.
- File format and alpha/background requirements.
- Scale and anchor/pivot.
- Layers and occlusion relationship.
- Animation states/frames.
- Collision or interaction requirements.
- Variants.
- Naming/location conventions.
- Prohibited elements.
- Visual acceptance criteria.
- Technical acceptance criteria.
- Integration acceptance criteria.

## Functional geometry
If an asset participates in insertion, occlusion, hit detection, modular construction, UI slicing, animation, or collision, specify the functional structure before final art production.

A beautiful flattened image may be unusable if the game needs separable foreground/background regions, pivots, masks, or state variants.

## AI-generated assets
For AI generation:
- Separate style constraints from object constraints.
- State single-object/background rules when relevant.
- Validate alpha rather than trusting prompt wording.
- Generate and approve a representative sample before batch production.
- Do not assume generated dimensions, transparency, or layer structure are technically correct until inspected.
