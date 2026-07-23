# Scenario 2 — Ant Count Comparison (Movement Rule Test)

**Comparing:** 30 ants (Scenario 1, Member 1's baseline) vs. 100 ants (this scenario)

## 30 ants
- Tick 100: ants dispersed across the map in a loose, uneven scattered pattern, a couple of ants have already reached the food patch (visible as yellow triangles) and turned back toward the nest
- Tick 200: only 2–3 ants carrying food (yellow) at any given time; most are still searching, food patch has barely shrunk
- Tick 723: food patch is noticeably eaten into at one corner, but a large portion is still untouched, with only 30 ants independently random-searching, coverage of the map is slow

## 100 ants
- Tick 9: ants have spread into a near-perfect ring around the nest, this is an artifact of all ants starting at the same point with random headings and moving forward at the same speed each tick, not an emergent trail yet
- Tick 100: search coverage is visibly denser than the 30-ant run at the same tick count; several ants already carrying food (yellow) scattered across the map, and the food patch has started shrinking from one edge
- Tick 197: food patch is reduced further, more yellow (food-carrying) ants visible simultaneously than at any point in the 30-ant run

## Change made to Random Search

The initial version of random-search turned each ant by an independent random amount every tick, which produced jittery, unrealistic zig-zagging rather than believable "wandering". This was changed to a correlated random walk, partly with the help of an LLM: each turn is now a small net rotation rather than a large independent one, so ants keep moving roughly in the same direction between ticks. Boundary steering was also added, so ants turn back toward the centre before reaching the edge of the world instead of getting stuck along it.

Reference: T. Fronville, "Correlated random walk" (Version 1.1.0), CoMSES Computational Model Library, 2023. Available: https://www.comses.net/codebases/a33c5f0a-a903-45e0-ae72-cb7abbce2f9f/releases/1.1.0/

## Comparison
With 100 ants, the map is searched far more thoroughly and quickly than with 30. Food is located and depleted noticeably faster simply because more independent searchers cover more ground per tick. However, movement in both runs is still purely random: ants that find food turn back individually, but there's no shared trail guiding others toward the same source. This is expected at this stage, since pheromone deposit and trail-following haven't been implemented yet. The ring pattern visible at tick 9 in the 100-ant run is also worth noting, it's a byproduct of synchronized starting conditions, not a rule I coded intentionally, and it disappears within the next ~20 ticks as random turning desynchronizes the ants.