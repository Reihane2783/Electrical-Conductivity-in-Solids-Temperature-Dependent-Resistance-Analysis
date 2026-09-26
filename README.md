# Resistance vs Temperature Analysis

A Python-based analysis of the temperature dependence of electrical resistance for a conductor and a semiconductor.

## Overview

This project calculates resistance values from experimental measurements and analyzes their temperature dependence using:

- Linear regression for the conductor
- Exponential regression for the semiconductor
- Mean squared error (MSE) evaluation
- Experimental data visualization
- Export of calculated data to Excel

## Method

The analysis calculates the complementary length values:

- `L2-R = 100 - L1-R`
- `L2-N = 100 - L1-N`

The corresponding resistance values are then calculated as:

- `Rx-R = 100 × L1-R / L2-R`
- `Rx-N = 1000 × L1-N / L2-N`

The temperature dependence is modeled using:

- **Conductor:** Linear regression
- **Semiconductor:** Exponential regression

## Visualization

The generated plot shows:

- Experimental resistance data
- Linear fit for the conductor
- Exponential fit for the semiconductor
- Fitting error for both datasets
