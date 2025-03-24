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

This project is licensed under the GNU License. See the [LICENSE](LICENSE) file for details.

## Contributing

Contributions are welcome! Please fork the repository and create a pull request with your changes.

## Contact

For any inquiries or support, please contact [SuperCaleb](https://github.com/SuperCaleb).

---

This README provides an overview of the Oden's Network Hybrid AI system, its features, key components, usage instructions, dependencies, installation steps, and contact information.




















































































































# EyeOfOden AI Vision System

## Overview

EyeOfOden is an advanced computer vision system designed to provide real-time object detection, tracking, and scene analysis. It utilizes the YOLOv8-X model for high-accuracy object detection and the DeepSORT algorithm for object tracking. Additionally, it offers text-to-speech capabilities to announce detected objects and actions within a scene.

## Features

- **Real-time Object Detection:** Uses YOLOv8-X for detecting various objects with high accuracy.
- **Object Tracking:** Employs DeepSORT for tracking objects across frames.
- **Text-to-Speech Announcements:** Announces detected objects and their actions using a text-to-speech engine.
- **Scene Summarization:** Provides periodic summaries of the scene, including object counts and notable actions.

## Requirements

- Python 3.7+
- OpenCV
- PyTorch
- NumPy
- pyttsx3
- ultralytics (YOLO)
- deep_sort_realtime

## Installation

1. **Clone the repository:**

    ```bash
    git clone https://github.com/SuperCaleb/OdensNetwork.git
    cd OdensNetwork
    ```

2. **Create and activate a virtual environment:**

    ```bash
    python -m venv venv
    source venv/bin/activate  # On Windows use `venv\Scripts\activate`
    ```

3. **Install the required packages:**

    ```bash
    pip install -r requirements.txt
    ```

## Usage

1. **Run the EyeOfOden AI Vision System:**

    ```bash
    python "Oden's Advanced Computer Vison Program"
    ```

2. **Functionality:**
    - **Object Detection:** The program captures frames from the webcam and detects objects using the YOLOv8-X model.
    - **Object Tracking:** Detected objects are tracked across frames using DeepSORT.
    - **Text-to-Speech Announcements:** The program announces new objects entering the scene, fast-moving objects, and provides periodic summaries of the scene.
    - **Scene Analysis:** Determines object locations, distances, movements, and actions.

3. **Controls:**
    - Press `q` to exit the program.

## How It Works

1. **Initialization:**
    - The YOLOv8-X model is loaded for object detection.
    - The DeepSORT tracker is initialized for tracking objects.
    - The webcam is accessed for capturing video frames.
    - A text-to-speech engine is set up to run in a separate thread for non-blocking speech synthesis.

2. **Main Loop:**
    - Frames are captured from the webcam.
    - Objects are detected in each frame using the YOLOv8-X model.
    - Detected objects are tracked across frames using DeepSORT.
    - The program determines the location, distance, movement, and action of each tracked object.
    - Text-to-speech announcements are made for new objects and notable events.
    - A summary of the scene is generated and announced periodically.
    - The processed frames are displayed in a window.

3. **Cleanup:**
    - The webcam is released, and the OpenCV window is closed.
    - The text-to-speech thread is terminated gracefully.

## Example Output

The program provides real-time output through the OpenCV window and text-to-speech announcements. Example announcements include:

- "A new person has entered the scene on the left."
- "A fast car is moving fast right on the center."
- "Currently, there are 2 persons, 1 car, and 1 bicycle. The closest person is walking on the right."

## Troubleshooting

- **Failed to open webcam:** Ensure your webcam is connected and accessible.
- **Missing dependencies:** Make sure all required packages are installed correctly.
- **Other errors:** Check the console output for error messages and troubleshoot accordingly.

## License

This project is licensed under the MIT License.

## Contributing

Contributions are welcome! Please submit a pull request or open an issue to discuss your ideas.

---

Feel free to customize this README further based on your specific needs and preferences.
