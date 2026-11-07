# Worked Example: Hybrid Game Integration

> Fictional example.

## Concept
A submarine logistics game where the player manages oxygen and cargo while occasionally piloting a small drone into wrecks.

## Risk
This could become two disconnected games: spreadsheet logistics and action exploration.

## Integration analysis
### Logistics
Experience: planning under scarcity.
Actions: allocate cargo, fuel, oxygen, repair capacity.

### Drone exploration
Experience: uncertain discovery.
Actions: navigate, scan, retrieve, retreat.

### Connection
- Logistics determines drone range and recovery capacity.
- Drone discoveries change future route and cargo decisions.
- Damage/resources recovered feed directly into submarine planning.

## Prototype question
“Does drone exploration create meaningful information and resource consequences for the logistics layer?”

## Minimal test
One submarine planning screen, one small wreck, three resource types, and one return decision.

Do not build a world map, crew relationships, crafting tree, or multiple biomes until the connection between the two activities is proven.
