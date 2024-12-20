# ML_project


This repository contains code for analyzing sensor data from the Unitree Go1 Dogrobot to classify the surface it walks on. The project uses machine learning techniques to process and analyze data obtained from various sensors available on the robot.

## Dataset Overview

The data used in this project comes from the Unitree Go1 Dogrobot and includes:
- **Joint Angular Position Sensors**: 12 sensors capturing the angles of the robot's joints.
- **Joint Torque Sensors**: 12 sensors measuring torque applied to each joint.
- **Gyroscopes**: 3 sensors providing rotational velocity data in three axes.
- **Accelerometers**: 3 sensors capturing linear acceleration data in three axes.

The dataset combines these inputs to identify patterns associated with different surface types.

## Code Description

1. **Data Preprocessing**:
   - Sensor data is read and normalized.
   - Features are extracted from angular positions, torque, gyroscope, and accelerometer data.

2. **Model Training**:
   - Supervised learning models are trained using labeled data of known surface types.
   - Features are mapped to surface categories.
   - we have used both LSTM and GRU (RNN models) 
 
3. **Evaluation**:
   - Models are evaluated using metrics like accuracy, precision, recall, and F1 score.
   - Confusion matrices are used to analyze misclassifications.

4. **Deployment**:
   - The trained model is exported for deployment on the Unitree Go1 Dogrobot for real-time surface classification.

## Requirements

- Python 3.8 or higher
- Libraries: `numpy`, `pandas`, `scikit-learn`
