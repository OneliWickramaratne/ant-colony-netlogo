# Ant Colony Food Search Simulation

SE404.3 Agent-Based Systems — Group Assignment

A NetLogo simulation of ants searching for food using pheromone trails, 
demonstrating emergent swarm behaviour through simple reactive agent rules.

## Team

| Member | Branch | Focus |
|--------|--------|-------|
| Member 1 | `member-1-setup` | Setup & agent creation |
| Member 2 | `member-2-movement` | Movement rules |
| Member 3 | `member-3-pheromone` | Pheromone logic |
| Member 4 | `member-4-decision-interface` | Decision rule & interface |
| Member 5 | `member-5-parameters-results` | Parameters, scenarios & results |

## Project Structure

```
ant-colony-netlogo/
├── ant-colony.nlogo       # main model file
├── results/                # scenario test results
└── screenshots/             # interface screenshots per member
```
## How to Run

1. Open `ant-colony.nlogo` in NetLogo
2. Click **setup**, then **go**
3. Adjust sliders (number-of-ants, evaporation-rate) to test different scenarios

## Workflow

- Each member works on their own branch, listed above
- Push commits to your branch, then open a Pull Request into `main` when your part works
- Merge order: Member 1 → 2 → 3 → 4 → 5 (later parts depend on earlier ones)
