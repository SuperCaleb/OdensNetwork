# Oden

Oden is a real-time anomaly detection and response system designed to monitor and protect network systems. It uses advanced machine learning techniques, including a Transformer-based predictor and a Deep Q-Network (DQN) for decision-making, to identify and respond to potential security threats.

## How Oden Works

### Key Components

1. **Configuration (`OdenConfig`)**: Configures various parameters such as log file, anomaly threshold, input window size, metrics history size, training samples, learning rate, check interval, action cooldown, and retrain interval.

2. **System State (`SystemState`)**: Maintains the global state of the system, including active status, bad IPs, metrics history, anomaly history, new metrics buffer, action timing, emotional state, and active threads.

3. **Logging**: Uses Python's `logging` module to log important events and anomalies to the specified log file.

4. **Transformer-Based Predictor**: A Transformer model that predicts system metrics based on historical data to detect anomalies.

5. **Enhanced DQN-Based Action Policy**: A reinforcement learning model that selects actions based on the detected anomalies and the current system state.

6. **System Metrics Collection**: Gathers real-time system metrics such as CPU usage, memory usage, disk usage, number of processes, number of connections, and number of bad connections.

7. **Action Execution**: Executes predefined actions such as terminating processes, blocking connections, investigating anomalies, isolating the network, and alerting the administrator based on the detected anomalies.

8. **Training Data Processing**: Collects and processes training data for the Transformer model to learn and improve its predictions.

9. **Core Detection and Learning Logic**: The main loop that continuously monitors the system, detects anomalies, selects actions, and learns from the environment.

### How to Use Oden

#### Prerequisites

- Python 3.6+
- Required Python packages: `numpy`, `tensorflow`, `psutil`, `scikit-learn`, `dataclasses`

#### Setup

1. **Install the required Python packages**:
    ```sh
    pip install numpy tensorflow psutil scikit-learn dataclasses
    ```

2. **Clone the repository**:
    ```sh
    git clone https://github.com/SuperCaleb/OdensNetwork.git
    cd OdensNetwork
    ```

#### Running Oden

1. **Run the main script**:
    ```sh
    python Lightweight\ Oden
    ```

2. **Collect initial training data**:
    The system will collect initial training data to train the Transformer model.

3. **Train the Transformer model**:
    The system will train the Transformer model using the collected training data.

4. **Start monitoring**:
    The system will start monitoring the real-time system metrics, detecting anomalies, and executing actions based on the detected anomalies.

#### Stopping Oden

To safely stop Oden, send a SIGINT (Ctrl+C) or SIGTERM signal. The system will shutdown gracefully, ensuring that all threads are terminated properly.

### Customizing Oden

You can customize various parameters by modifying the `OdenConfig` class. For example, you can change the log file name, anomaly threshold, input window size, metrics history size, training samples, learning rate, check interval, action cooldown, and retrain interval.

### Example Log Output

Logs are saved to the specified log file (`oden_security.log` by default). Example log output:
```
2025-03-24 19:47:57 - Terminated process: suspicious_process (PID: 12345)
2025-03-24 19:48:57 - Blocked process: malicious_process (PID: 67890)
2025-03-24 19:49:57 - Investigating anomaly
2025-03-24 19:50:57 - Network isolated: SSH only
2025-03-24 19:51:57 - Critical anomaly detected!
```

### Important Notes

- **Critical Processes**: The system has a list of critical processes (`CRITICAL_PROCESSES`) that it will not terminate or block.
- **Emotional State**: The system uses an emotional state model to adjust its behavior based on the severity of detected anomalies.
- **Self-Replication**: The system can spawn new threads to handle high anomaly scores, ensuring continued monitoring and response.

## Conclusion

Oden is a powerful tool for real-time anomaly detection and response, leveraging advanced machine learning techniques to protect your network systems. Customize and extend Oden to fit your specific requirements, and ensure the security and stability of your network infrastructure.






































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
