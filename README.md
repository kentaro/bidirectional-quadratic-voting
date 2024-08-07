# Bidirectional Quadratic Voting Experiment

This experiment simulates and compares different voting methods, including normal voting, quadratic voting, and bidirectional quadratic voting, across various voter distributions.

## Overview

The experiment explores how different voting methods perform under various voter ideology distributions. It simulates candidate preferences, voter preferences, and calculates matching scores for each voting method.

## Key Components

1. **Candidates**: 5 candidates with varying ideological positions.
2. **Issues**: 6 issues including Environmental Protection, Economic Growth, Education Reform, Social Security, Foreign Policy, and Technology.
3. **Voters**: 10,000 simulated voters.
4. **Voter Distributions**: Normal, Bimodal, Skewed Left, and Skewed Right.

## Voting Methods

1. **Normal Voting**: Based on a specified distribution (Tokyo Governor Election 2024 Results).
2. **Quadratic Voting**: Voters allocate credits quadratically to express preference intensity.
3. **Bidirectional Quadratic Voting**: Both voters and candidates use quadratic voting to express preferences.

## Simulation Process

1. Generate candidate preferences.
2. Generate voter preferences for each distribution type.
3. Calculate matching scores for each voting method.
4. Visualize results using matplotlib.

## Results

The experiment produces:
- Candidate preference distribution graph.
- Voter ideology distribution graphs for each distribution type.
- Comparison graphs of voting results for each distribution and voting method.
- Numerical output of matching scores for each candidate under different voting methods and voter distributions.

## Code Structure

The main components of the code are:

```python:experiments.ipynb
startLine: 25
endLine: 83
```

This section includes functions for generating preferences, calculating voting scores, and implementing different voting methods.

## Running the Experiment

The experiment is executed in a Jupyter notebook environment. The main simulation and visualization code is located at:

```python:experiments.ipynb
startLine: 200
endLine: 310
```

## Conclusion

This experiment provides insights into how different voting methods perform under various voter ideology distributions, potentially informing discussions on electoral system design and reform.
