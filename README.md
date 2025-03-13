

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




































































# Oden's Network - Hybrid AI System

## Overview

Oden's Network is a sophisticated hybrid AI system designed for monitoring, anomaly detection, and threat response. This system integrates various machine learning models, neural networks, and advanced algorithms to ensure the security and operational efficiency of a network. It leverages real-time data processing, anomaly detection, and proactive threat mitigation to maintain a secure and stable environment.

## Features

- **Hybrid AI Models**: Combines multiple neural network architectures, including transformers, LSTM, and convolutional networks for enhanced anomaly detection and threat response.
- **Anomaly Detection**: Uses advanced anomaly detection techniques to identify and respond to unusual activities and potential threats in real-time.
- **Threat Intelligence**: Integrates threat intelligence feeds from various sources to stay updated on the latest security threats.
- **Proactive Threat Mitigation**: Proactively takes actions like blocking IPs, terminating suspicious processes, and more to mitigate detected threats.
- **Enhanced Logging**: Includes an advanced logging system with natural language processing (NLP) for sentiment analysis and structured logging.
- **Consciousness Module**: Inspired by Damasio's theories, this module simulates emotional valence and homeostasis to improve decision-making.
- **Health and Metrics Reporting**: Regularly reports system health and metrics for continuous monitoring and improvement.
- **Reinforcement Learning**: Implements a reinforcement learning policy to optimize actions based on rewards and learning from past experiences.
- **Holographic Memory**: Employs a holographic memory system for distributed storage and quick access to historical data.
- **Interactive User Commands**: Allows user interaction and command processing for real-time status updates and explanations.

## Key Components

1. **Configuration Management**: Manages system configuration and parameters.
2. **Thought Templates**: Templates for generating human-like communication and responses.
3. **Positional Encoding Layer**: Used in transformer models for sequence processing.
4. **Transformer Encoder Layer**: Enhances the transformer model's capabilities.
5. **OdenLogger**: Advanced logging system with NLP integration.
6. **SystemState**: Manages the global state of the system.
7. **SignatureDetector**: Detects known threat signatures from metrics.
8. **HolographicMemory**: Stores and queries memory vectors for anomaly detection.
9. **ConsciousnessModule**: Simulates emotional states and decision-making based on homeostasis.
10. **OdenBrain**: Core neural network model for anomaly detection and prediction.
11. **OdenPolicy**: Reinforcement learning policy for action selection and learning.
12. **OdenDynamics**: Models system dynamics for predicting future states.
13. **EffectivenessManager**: Manages the effectiveness of actions and updates based on outcomes.
14. **OdenCoT**: Chain of Thought module for reasoning and decision-making.
15. **HWS**: He Who Sees - Next-Gen Forensic Intelligence System with Orch OR Integration for real-time video and audio analysis.

## Usage

1. **Configuration**: Configure the system parameters and threat intelligence sources in the `OdenConfig` class.
2. **Initialization**: Initialize the system by creating instances of `OdenBrain`, `OdenPolicy`, `EffectivenessManager`, `OdenDynamics`, and `OdenCoT`.
3. **Run Oden**: Use the `run_oden` function to start the core control logic with the consciousness module.
4. **User Interaction**: Interact with the system using commands like `status` and `explain_last_action` for real-time updates and explanations.

## Dependencies

- Python 3.7 or higher
- NumPy
- TensorFlow
- PyTorch
- Scikit-learn
- Psutil
- Aiohttp
- Smptlib
- Cryptography
- Mediapipe
- Ultralytics YOLO
- Deep Sort Realtime
- Transformers
- Timm
- NetworkX

## Installation

1. Clone the repository:
   ```
   git clone https://github.com/SuperCaleb/OdensNetwork.git
   cd OdensNetwork
   ```

2. Install the required dependencies:
   ```
   pip install -r requirements.txt
   ```

3. Configure environment variables for API keys and email settings:
   ```
   export ABUSEIPDB_API_KEY=your_abuseipdb_api_key
   export VT_API_KEY=your_virustotal_api_key
   export OTX_API_KEY=your_otx_api_key
   export ODEN_EMAIL_PASSWORD=your_email_password
   export SLACK_WEBHOOK=your_slack_webhook_url
   ```

4. Run the system:
   ```
   python oden.py
   ```

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.

## Contributing

Contributions are welcome! Please fork the repository and create a pull request with your changes.

## Contact

For any inquiries or support, please contact [SuperCaleb](https://github.com/SuperCaleb).

---

This README provides an overview of the Oden's Network Hybrid AI system, its features, key components, usage instructions, dependencies, installation steps, and contact information.
