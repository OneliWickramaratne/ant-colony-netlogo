# Scenario 1 — Low Number of Ants

# Objective

The objective of Scenario 1 was to observe the food-search behaviour of the ant colony when a low number of ants was used. The scenario examined how the ants initially explored the environment, how quickly food collection began, and how pheromone trails developed while the ants travelled between the food source and the nest.


# Simulation Settings

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


#  Initial Conditions

At tick 0, all 30 ants were positioned at the centre of the nest. The open ground was displayed in green, the nest was displayed in brown, and the food source was displayed in yellow.

The initial monitor values were:

| Monitor | Initial value |
|---|---:|
| Food Collected | 0 |
| Average Trip Time | 0 |
| Ants Carrying Food | 0 |
| Ticks | 0 |

The ants had not yet started moving, and no pheromone trail was present.



# Early Simulation Observation

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

# Final Results

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


# Observations

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


# Analysis

The results show that 30 ants were able to find the food source and return food to the nest. At the beginning, the ants moved randomly because no strong pheromone trail existed.
By tick 47, two food units had been collected and visible pheromone paths had started to form. The colony collected 42 food units by tick 1005, with an average trip time of 115 ticks.
The value of zero ants carrying food at the final tick does not mean the simulation failed. It only means that no ant was carrying food at that exact moment. Overall, the scenario demonstrates how simple individual ant behaviours can produce coordinated colony-level food-search behaviour.



