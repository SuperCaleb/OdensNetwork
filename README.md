
---

# Oden's Defense System

**Oden's Defense System** is a Python-based monitoring and defense mechanism that uses Reinforcement Learning (RL) to detect anomalies in system metrics (CPU, memory, and disk usage) and take appropriate actions.

## Features
- **Metrics Gathering**: Collects CPU, memory, and disk usage metrics using system commands.
- **Anomaly Detection**: Identifies anomalies based on historical data by calculating mean and standard deviation.
- **Reinforcement Learning**: Uses RL to choose actions that minimize anomalies.
- **Logging**: Logs actions and metrics to both console and a log file.

## Requirements
- **Python 3.x**
- Required Python packages: `subprocess`, `time`, `random`, `collections`, `logging`

## Installation

Clone the repository:

```bash
git clone https://github.com/SuperCaleb/OdensNetwork.git
cd OdensNetwork
```

Ensure Python 3.x is installed on your system.

## Usage

Navigate to the directory containing the script:

```bash
cd "Oden's defense system"
```

Run the script:

```bash
python3 "Oden's defense system.py"
```

## Script Explanation

### Key Components
- **Logging Setup**: Configures logging to output to both console and a file named `oden.log`.
- **Constants**: Sets various constants for history size, epsilon decay, learning rate, etc.
- **`gather_metrics()`**: Collects CPU, memory, and disk usage metrics.
- **`compute_state()`**: Converts metrics into a discrete state for the RL policy.
- **`compute_stats()`**: Calculates mean and standard deviation from historical metrics.
- **`execute_action()`**: Executes chosen actions and logs the action.

### Main Loop
1. **Metrics Gathering**: Collects current system metrics.
2. **Anomaly Detection**: Computes means and standard deviations from historical data and detects anomalies.
3. **Action Selection**: Uses an epsilon-greedy policy to select an action based on the Q-table.
4. **Action Execution**: Executes the chosen action.
5. **Reward Computation**: Gathers new metrics and computes the reward based on the reduction of anomalies.
6. **Q-table Update**: Updates the Q-table based on the reward.
7. **Epsilon Decay**: Gradually decays epsilon to reduce exploration over time.

### Actions
- **Monitor**: Takes no action.
- **Investigate**: Logs the current system metrics.
- **Terminate**: Logs a message indicating the termination of a high CPU process.
- **Reinforce**: Logs a message indicating reinforcement of system defenses.

This script continuously runs, gathering metrics, detecting anomalies, choosing actions, and updating its RL policy to improve over time.

---
