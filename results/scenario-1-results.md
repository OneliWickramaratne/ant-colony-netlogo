# Scenario 1 — Low Number of Ants

## 1. Objective

The objective of Scenario 1 was to observe the food-search behaviour of the ant colony when a low number of ants was used. The scenario examined how the ants initially explored the environment, how quickly food collection began, and how pheromone trails developed while the ants travelled between the food source and the nest.

---

## 2. Simulation Settings

| Parameter | Value |
|---|---:|
| Number of ants | 30 |
| Evaporation rate | 0.05 |
| Show pheromone | On |
| Nest location | Centre of the NetLogo world |
| Food location | Upper-right area of the world |
| Initial tick | 0 |
| Final tick | 1005 |

The simulation used 30 ants because Scenario 1 required a low number of agents. The evaporation rate was kept at 0.05, and the pheromone display was enabled so that the development of trails could be observed.

---

## 3. Procedure

1. The NetLogo model was opened from the project repository.
2. The `number-of-ants` slider was set to `30`.
3. The `evaporation-rate` slider was set to `0.05`.
4. The `show-pheromone?` switch was turned on.
5. The `setup` button was clicked to create the world, nest, food area and ants.
6. A screenshot was taken at tick 0.
7. The `Go` button was clicked to start the simulation.
8. The ants were observed as they moved away from the nest and searched for food.
9. A screenshot was taken at tick 47 when ants were carrying food and pheromone trails had started to appear.
10. The simulation was continued until approximately tick 1000.
11. The final monitor values and behaviour were recorded at tick 1005.

---

## 4. Initial Conditions

At tick 0, all 30 ants were positioned at the centre of the nest. The open ground was displayed in green, the nest was displayed in brown, and the food source was displayed in yellow.

The initial monitor values were:

| Monitor | Initial value |
|---|---:|
| Food Collected | 0 |
| Average Trip Time | 0 |
| Ants Carrying Food | 0 |
| Ticks | 0 |

The ants had not yet started moving, and no pheromone trail was present.

---

## 5. Early Simulation Observation

By tick 47, the ants had spread away from the nest and explored different parts of the environment.

The recorded values at tick 47 were:

| Monitor | Value at tick 47 |
|---|---:|
| Food Collected | 2 |
| Average Trip Time | 27.5 ticks |
| Ants Carrying Food | 2 |
| Ticks | 47 |

At this stage, two ants were carrying food and two units of food had already been returned to the nest. Blue pheromone paths were visible between parts of the environment, the nest and the food area.

The exact tick when the first ant reached the food source was not recorded separately. However, the results confirm that food discovery and collection occurred before tick 47.

---

## 6. Final Results

The simulation was stopped at tick 1005.

| Result | Recorded value |
|---|---:|
| Number of ants | 30 |
| Evaporation rate | 0.05 |
| Final tick | 1005 |
| Food Collected | 42 |
| Average Trip Time | 115 ticks |
| Ants Carrying Food at final tick | 0 |

By the end of the simulation, the colony had collected 42 units of food. The food source had been mostly depleted, leaving only a small number of food patches.

The `Ants Carrying Food` monitor showed 0 at the final tick because no ant was carrying food at that exact moment. The graph shows that ants carried food at several earlier points during the simulation.

---

## 7. Observations

| Observation item | Result |
|---|---|
| Initial movement behaviour | The ants initially moved randomly away from the central nest and spread in different directions. |
| Food discovery | Food was discovered early in the simulation, before tick 47. |
| Early food collection | Two food units had been collected by tick 47. |
| Pheromone behaviour | Blue pheromone trails appeared as ants carrying food travelled through the environment. |
| Trail formation | Several temporary paths formed rather than one completely stable path. |
| Food collection progress | Food collection increased from 2 units at tick 47 to 42 units at tick 1005. |
| Final carrying state | No ants were carrying food at tick 1005. |
| Overall result | The colony successfully found the food source and transported most of the food back to the nest. |

---

## 8. Analysis

The low-ant scenario demonstrated that a colony of 30 ants was capable of locating the food source and transporting food back to the nest without central control.

At the beginning of the simulation, the ants moved randomly because they did not yet have a strong pheromone trail to follow. This random movement allowed the ants to explore different sections of the environment.

Once some ants reached the food source, they began returning toward the nest while depositing pheromone. The blue paths visible at tick 47 show that environmental information was already being created through the ants' movements.

Other ants could then respond to the pheromone in nearby patches. This produced a collective searching pattern even though each ant followed only simple local rules.

The colony collected 42 units of food by tick 1005. This shows that the low number of ants was still sufficient to perform the food-search task successfully. However, the trails were not permanently stable because pheromone evaporated over time and the ants retained some random movement.

The average trip time increased to 115 ticks by the end of the run. This may have occurred because some ants travelled through longer or less direct routes before returning to the nest.

The final value of zero ants carrying food does not mean that the model failed. It only means that no ant was holding food at tick 1005. Earlier activity is confirmed by the graph, the 42 collected food units and the visible reduction in the food source.

---

## 9. Emergent Behaviour

The main emergent behaviour observed in Scenario 1 was the development of pheromone-based paths between the nest and the food area. No single ant controlled the colony or planned the complete route. Instead, each ant moved and reacted using local information.

As multiple ants travelled through similar areas, their individual actions produced visible colony-level patterns. This was a positive emergent behaviour because it helped the colony discover the food source and collect 42 food units using only 30 ants.

---

## 10. Evaluation of the Scenario

One strength of the model is that it clearly demonstrates how simple ant behaviours can produce coordinated food-search activity. The model also provides visual evidence through the pheromone display, monitors and graph.

One limitation is that the food patches are removed permanently when collected. Therefore, once most food has been collected, the number of ants carrying food decreases and eventually reaches zero.

Another limitation is that the exact first-food tick was not recorded automatically. The early screenshot only confirms that food collection had already begun by tick 47.

The scenario assumed that all ants had identical movement behaviour, speed and sensing ability. It also assumed that the world did not contain obstacles or environmental hazards.

---

## 11. Conclusion

Scenario 1 demonstrated that 30 autonomous ants could explore the NetLogo environment, discover the food source, develop pheromone paths and collect 42 food units by tick 1005. The scenario showed how simple individual actions can create organized colony-level behaviour without centralized control.

