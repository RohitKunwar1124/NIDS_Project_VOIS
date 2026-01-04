# Network Intrusion Detection System

A machine learning-based web application for real-time network traffic classification and intrusion detection.

## Features

- Real-time network traffic analysis
- Automated attack classification (Normal, DoS, Probe, R2L, U2R)
- User-friendly web interface
- RESTful API for integration
- Pre-trained ML model for accurate predictions

## Project Structure

```
├── NSL_Dataset/          # Training and test datasets
├── results/              # Screenshots and results
├── static/              # CSS styling files
├── templates/           # HTML templates
├── app.py               # Flask web application
├── model.pkl            # Pre-trained ML model
├── requirements.txt     # Python dependencies
└── README.md            # Project documentation
```

## Problem Statement

Network security is critical in today's digital world. This system addresses the need for automated detection of network intrusions and attacks by classifying network traffic into:

1. **Normal** - Legitimate network traffic
2. **DoS** - Denial of Service attacks
3. **Probe** - Surveillance and scanning attacks
4. **R2L** - Remote to Local unauthorized access
5. **U2R** - User to Root privilege escalation

## Dataset

This project uses the NSL-KDD dataset, a widely recognized benchmark for network intrusion detection systems.

For more information: http://www.unb.ca/cic/datasets/nsl.html

## Attack Types

### DoS (Denial of Service)
Attacks that deplete victim resources, making systems unable to handle legitimate requests (e.g., syn flooding).

### Probe
Surveillance attacks aimed at gaining information about remote victims (e.g., port scanning).

### R2L (Remote to Local)
Unauthorized access from a remote machine to gain local access (e.g., password guessing).

### U2R (User to Root)
Unauthorized access to root/administrator privileges by exploiting vulnerabilities (e.g., buffer overflow attacks).

## Installation

1. Clone the repository
2. Install dependencies:
   ```bash
   pip install -r requirements.txt
   ```

## Usage

1. Run the Flask application:
   ```bash
   python app.py
   ```

2. Open your web browser and navigate to `http://localhost:5000`

3. Fill in the network connection features in the web form

4. Click "Predict" to get the attack classification result

## Requirements

- Python 3.x
- Flask
- scikit-learn
- joblib
- NumPy

See `requirements.txt` for complete list of dependencies.

## License

MIT License
