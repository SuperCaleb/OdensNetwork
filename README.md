![Screenshot 2025-03-30 211533](https://github.com/user-attachments/assets/d58c40e4-fd80-4077-91d6-7291b2bb23c9)
![Screenshot 2025-03-30 211626](https://github.com/user-attachments/assets/229cd89d-6f54-49d1-b1d5-dfdf4316d899)
![Screenshot 2025-03-30 211644](https://github.com/user-attachments/assets/594950d6-abd2-48f7-a8cf-17dbc557c992)
![Screenshot 2025-03-30 211703](https://github.com/user-attachments/assets/125fd493-78df-4d49-ad22-f19fe22950c7)
![Screenshot 2025-03-30 211721](https://github.com/user-attachments/assets/c88229c6-5d38-434d-8b7c-bbbcb57f8d06)
# Oden's Network - README

## Table of Contents
- [Introduction](#introduction)
- [Overview](#overview)
- [Key Features](#key-features)
- [Installation](#installation)
- [Configuration](#configuration)
- [Usage](#usage)
  - [Running Oden](#running-oden)
  - [Commands](#commands)
- [Components](#components)
  - [System State Management](#system-state-management)
  - [Configuration Management](#configuration-management)
  - [Advanced Prometheus Monitoring](#advanced-prometheus-monitoring)
  - [Logging System](#logging-system)
  - [Anomaly Detection](#anomaly-detection)
  - [Action Execution](#action-execution)
  - [Notification System](#notification-system)
  - [Threat Intelligence](#threat-intelligence)
  - [Oden Brain](#oden-brain)
  - [Oden Policy](#oden-policy)
  - [Oden Dynamics](#oden-dynamics)
  - [Consciousness Module](#consciousness-module)
  - [Chain of Thought (CoT)](#chain-of-thought-cot)
  - [Health Check](#health-check)
- [Development](#development)
- [Contributing](#contributing)
- [License](#license)

## Introduction
**Oden's Network** is an advanced cybersecurity and monitoring system designed to detect, analyze, and respond to various threats in real-time. Oden leverages state-of-the-art machine learning, anomaly detection, and AI-driven decision-making to ensure the security and stability of your systems.

## Overview
Oden is built with a modular architecture that includes components for monitoring system metrics, detecting anomalies, executing actions, and maintaining overall system health. It integrates with popular tools and services like Prometheus for monitoring, TensorFlow for machine learning, and various APIs for threat intelligence.

## Key Features
- **Real-time Monitoring**: Continuous system metrics collection and analysis.
- **Anomaly Detection**: Advanced machine learning models to detect unusual behavior.
- **Automated Response**: AI-driven decision-making to execute predefined actions based on detected anomalies.
- **Prometheus Integration**: Export key metrics to Prometheus for visualization and alerting.
- **Threat Intelligence**: Integration with multiple threat intelligence sources.
- **Enhanced Logging**: Structured logging with alerting capabilities.
- **Health Checks**: Regular validation and fine-tuning of machine learning models.

## Installation
To install Oden, you need to have Python 3.7+ installed on your system. Follow these steps to set up Oden:

1. Clone the repository:
   ```sh
   git clone https://github.com/SuperCaleb/OdensNetwork.git
   cd OdensNetwork
   ```

2. Create a virtual environment and activate it:
   ```sh
   python3 -m venv venv
   source venv/bin/activate
   ```

3. Install the required dependencies:
   ```sh
   pip install -r requirements.txt
   ```

## Configuration
Oden's configuration is managed through the `OdenConfig` class. Key configuration parameters include log file paths, alert thresholds, metrics intervals, and API keys for threat intelligence sources.

You can customize the configuration by editing the `OdenConfig` class in the source code or by setting environment variables for sensitive information like API keys and email passwords.

## Usage
### Running Oden
To start Oden, simply run the main script:
```sh
python Oden
```

Oden will initialize its components, start monitoring, and begin processing system metrics. The Prometheus server will start on port 8000 by default.

### Commands
Oden supports a few interactive commands that can be issued via standard input (stdin):

- `status`: Provides a detailed status update of the system.
- `explain_last_action`: Explains the reasoning behind the last action taken by Oden.

## Components
### System State Management
The `SystemState` class manages the overall state of the system, including active status, bad IPs, metrics history, anomaly history, and more.

### Configuration Management
The `OdenConfig` class defines the configuration parameters for Oden. These include logging settings, metrics intervals, thresholds, and API keys for various integrations.

### Advanced Prometheus Monitoring
Oden uses Prometheus to monitor key system metrics like CPU usage, memory usage, anomaly scores, and GPU utilization. The `start_prometheus_server` function starts a Prometheus metrics server on a separate thread.

### Logging System
The `OdenLogger` class provides an enhanced logging system with structured logging, alert thresholds, and metrics reporting. Logs are written to a rotating file and can trigger alerts based on the volume and severity of log messages.

### Anomaly Detection
Oden uses machine learning models to detect anomalies in system metrics. The `OdenBrain` class manages the training, prediction, and validation of these models. Anomalies are detected based on a combination of reconstruction errors, classification scores, and cluster distances.

### Action Execution
Oden can execute predefined actions based on detected anomalies. Actions include terminating processes, encrypting files, transmitting alerts, deleting suspicious files, and more. The `execute_action` function handles the execution of these actions and updates the effectiveness of each action.

### Notification System
Oden can send notifications via email and Slack. The `send_notification` function formats and sends alerts based on context provided by the system. Email notifications are sent using the SMTP protocol.

### Threat Intelligence
Oden integrates with multiple threat intelligence sources to update its list of bad IPs. The `refresh_threat_intel` function periodically fetches threat intelligence data and updates the system's bad IP list.

### Oden Brain
The `OdenBrain` class is the core of Oden's anomaly detection system. It includes methods for building and training machine learning models, predicting anomalies, and validating model performance.

### Oden Policy
The `OdenPolicy` class implements a Dueling Deep Q-Network (DQN) with Prioritized Experience Replay to decide on actions based on the current state of the system. It uses reinforcement learning to improve its decision-making over time.

### Oden Dynamics
The `OdenDynamics` class models the dynamics of the system by predicting future states based on current metrics and actions. It helps in estimating the impact of actions and planning proactive steps.

### Consciousness Module
The `ConsciousnessModule` class simulates a rudimentary form of consciousness by maintaining a self-state, assessing emotional impact, and reflecting on actions. It enhances Oden's decision-making by considering the system's overall well-being.

### Chain of Thought (CoT)
The `OdenCoT` class manages the chain of thought for Oden, assessing anomalies, selecting actions, evaluating responses, and planning proactive steps. It integrates with the Consciousness Module for enhanced decision-making.

### Health Check
The `health_check` function periodically validates the performance of Oden's machine learning models and fine-tunes them if necessary. It ensures that the models remain accurate and effective over time.

## Development
To contribute to Oden's development, follow these steps:

1. Fork the repository and clone your fork.
2. Create a new branch for your feature or bugfix.
3. Implement your changes and write tests if applicable.
4. Commit your changes and push your branch to your fork.
5. Create a pull request to the main repository.

## Contributing
We welcome contributions from the community! Please read our [CONTRIBUTING.md](CONTRIBUTING.md) file for guidelines on how to contribute to Oden.

## License
Oden is licensed under the MIT License. See the [LICENSE](LICENSE) file for more details.

---

Thank you for using Oden's Network! For any questions or support, please contact us at support@example.com.










































































































































































































































































































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


