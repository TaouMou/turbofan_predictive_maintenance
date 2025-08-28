# Turbofan Engine Predictive Maintenance

## Introduction

Prognostics and health management is a crucial field in industry, aiming to predict the state of assets to avoid unexpected downtime and failures. This project focuses on the prediction of Remaining Useful Life (RUL) for turbofan jet engines using the NASA C-MAPSS dataset. The dataset consists of simulated run-to-failure data for a fleet of engines, where each engine starts in a healthy state and develops faults over time. The objective is to use multivariate time series sensor data and operational settings to estimate how many operational cycles remain before an engine fails, enabling proactive maintenance strategies.

The NASA C-MAPSS dataset is widely used for benchmarking predictive maintenance algorithms and is available on Kaggle:  
[https://www.kaggle.com/datasets/behrad3d/nasa-cmaps/data](https://www.kaggle.com/datasets/behrad3d/nasa-cmaps/data)


## Dataset

The data is provided as text files with **26 columns**:
1. Unit number (engine ID)
2. Time, in cycles
3. Operational setting 1
4. Operational setting 2
5. Operational setting 3
6-26. Sensor measurements 1-21

Each row is a snapshot of an engine at a single operational cycle.

### Data Set Organization

- **FD001**: 100 train/test trajectories, 1 condition, 1 fault mode
- **FD002**: 260/259 train/test, 6 conditions, 1 fault mode
- **FD003**: 100 train/test, 1 condition, 2 fault modes
- **FD004**: 248/249 train/test, 6 conditions, 2 fault modes

### Reference
Reference: A. Saxena, K. Goebel, D. Simon, and N. Eklund, Damage Propagation Modeling for Aircraft Engine Run-to-Failure Simulation, in the Proceedings of the 1st International Conference on Prognostics and Health Management (PHM08), Denver CO, Oct 2008.