

---

# Lightweight Oden

## Overview
Lightweight Oden is a Python script designed for anomaly detection and automated response in system metrics. It utilizes a lightweight neural network to detect anomalies and perform actions such as terminating processes, blocking IPs, or investigating anomalies.

## Features
- **Anomaly Detection:** Uses a neural network to identify unusual system behavior based on metrics like CPU usage, memory usage, disk usage, and network connections.
- **Automated Actions:** Executes predefined actions (Terminate, Block, Investigate) based on the detected anomalies.
- **Logging:** Maintains a log of activities and detected anomalies for further analysis.
- **Configuration:** Easily configurable parameters for anomaly thresholds, metrics history size, and action cooldowns.

## Setup and Usage

### Prerequisites
- Python 3.x
- Required Python libraries: `numpy`, `tensorflow`, `psutil`, `sklearn`

### Installation
1. Clone the repository:
   ```sh
   git clone https://github.com/SuperCaleb/OdensNetwork.git
   ```
2. Navigate to the directory:
   ```sh
   cd OdensNetwork
   ```
3. Install the necessary Python libraries:
   ```sh
   pip install numpy tensorflow psutil scikit-learn
   ```

### Configuration
The configuration can be adjusted in the `OdenConfig` class within the script:
```python
@dataclass
class OdenConfig:
    log_file: str = "oden_security.log"
    anomaly_threshold: float = 0.85
    metrics_window: int = 5
    metrics_history_size: int = 100
    memory_size: int = 1000
    learning_rate: float = 0.0003
    check_interval: float = 1.0
    action_cooldown: float = 3.0
```
Adjust these parameters based on your requirements.

### Running the Script
Execute the script using Python:
```sh
python3 Lightweight Oden
```
The script will start monitoring system metrics and execute actions based on the detected anomalies.

### Stopping the Script
The script can be stopped gracefully using SIGINT (Ctrl+C) or SIGTERM signals.

## Logging
The script logs its actions and detected anomalies to the file specified in the configuration (`oden_security.log`).

## License
This project is licensed under the GNU General Public License v3.0. See the [LICENSE](https://github.com/SuperCaleb/OdensNetwork/blob/Oden's-Weapon/LICENSE) file for details.

## Repository
- [GitHub Repository](https://github.com/SuperCaleb/OdensNetwork)

### Author
- GitHub: [SuperCaleb](https://github.com/SuperCaleb)

---

