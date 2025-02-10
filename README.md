# SimulationAndMetrology
Final project for Simulation and Metrology course at IP Paris

# Heterogeneous Queue Simulation

## Overview
This project simulates a heterogeneous traffic queue using **SimPy**. It models different types of network traffic (data, voice, and video) competing for a shared **100 Mbps** server with an infinite capacity queue.

## Features
- **Traffic Models:**
  - **Data Traffic:** Poisson-distributed packet arrivals with variable sizes.
  - **Voice Traffic:** Constant bit rate (CBR) traffic.
  - **Video Traffic:** Bursty ON/OFF model.
- **Performance Metrics:**
  - **Response Time:** Time from packet arrival to completion.
  - **Loss Rate:** Proportion of packets dropped when the queue is full.
- **Event-Driven Simulation:** Efficiently handles packet arrivals, service, and queue dynamics.
- **Visualization:** Generates plots for response times and loss rates.

## Installation
This project uses Python 3 and requires a **virtual environment** for dependency management.

### 1. Create a Virtual Environment
```bash
python3 -m venv venv
source venv/bin/activate  # Linux/Mac
venv\Scripts\activate  # Windows
```

### 2. Install Dependencies
```bash
pip install -r requirements.txt
```

## Usage
To run the simulation:
The script will generate performance metrics and plots of the simulation results.

## Output
- The script plots:
  - **Loss rate over time** for each traffic type.
  - **Response time over time** for each traffic type.
- The simulation results can also be redirected to a file:

## File Structure
```
/SimulationAndMetrology
│── simProject.ipynb         # Main simulation script
│── burstiness_results.csv # Simulation Results
│── requirements.txt      # Dependencies
│── README.md             # Project documentation
│── venv/                 # Virtual environment (excluded from GitHub)
```

## Dependencies
- `numpy`
- `pandas`
- `matplotlib`
- `simpy`

## Contributing
Feel free to fork this repository, submit issues, or suggest improvements.

## License
This project is licensed under the MIT License.

