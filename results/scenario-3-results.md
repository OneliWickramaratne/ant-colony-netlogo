# Scenario 3 — Pheromone Evaporation Test

**Ant count:** [same as Scenario 2 — fill in, e.g. 100]

## Low evaporation rate (0.05)
- Tick 5: pheromone trail barely visible yet, ants mostly still searching randomly
- Tick 35: a clear blue trail has formed from the nest outward, showing where ants have been travelling repeatedly
- Tick 143: trail is well-established and visibly connects toward the food source, several ants successfully carrying food (yellow) back to the nest

## High evaporation rate (0.82)
- Tick 5: no visible trail, same starting state as low rate
- Tick 35: trail barely visible — pheromone decays almost as fast as it's laid down
- Tick 143: still no meaningful trail has formed; ants continue to rely mostly on random search rather than a reinforced path

## Comparison
At a low evaporation rate (0.05), pheromone accumulates faster than it decays, allowing a stable, visible trail to form and strengthen over time — this closely matches the expected "shortest path" emergent behaviour described in the brief. At a high evaporation rate (0.82), pheromone disappears almost as quickly as it's deposited, preventing a reinforced trail from ever forming. This shows evaporation rate is a critical parameter: too high, and the colony loses the ability to communicate discovered paths through pheromone, relying instead on random search alone.