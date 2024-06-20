# PowerAdaptationInterference Simulation Project

## Overview

The **PowerAdaptationInterference** project utilizes NS-3 (Network Simulator 3) to simulate and analyze scenarios in WiFi networks where power adaptation strategies interact with interference. This simulation framework aims to provide insights into the performance metrics of WiFi nodes under varying conditions of transmission power levels, interference levels, and network congestion.

## Key Features

### NodeStatistics Class

The core component of the project is the `NodeStatistics` class, which monitors and collects extensive data on each WiFi node during the simulation. This includes:

- **Power Levels**: Tracks changes in transmission power levels based on adaptation algorithms.
- **Data Rates**: Monitors variations in data rates influenced by interference and adaptive modulation techniques.
- **State Durations**: Records the durations spent in different states such as idle, busy (processing or waiting for channel access), transmit, and receive.

### Gnuplot Visualization

Visualization is crucial for understanding simulation results. The project utilizes Gnuplot to generate graphical outputs that illustrate:

- **Throughput**: Graphs depicting the throughput achieved by each node over time.
- **Power Consumption**: Trends in power consumption across nodes throughout the simulation period.
- **State Distribution**: Pie charts or histograms showing the distribution of time spent in various operational states by the nodes.

### Flow Monitoring

Utilizes NS-3's FlowMonitor module to capture and analyze flow-level statistics including:

- **Throughput**: Calculated as the amount of data successfully delivered per unit time.
- **Packet Loss**: Percentage of packets that fail to reach their destination.
- **Delay**: Average time taken for packets to traverse the network.

### Configurability

The simulation framework offers flexibility in configuring various parameters:

- **Transmission Power Levels**: Adjustable to simulate different power adaptation strategies.
- **RTS Thresholds**: Influences the decision-making process for channel access and collision avoidance.
- **Simulation Time**: Duration of simulation runs, allowing for long-term performance evaluation.
- **Node Positions**: Configurable to simulate different network topologies and node distributions.

## Installation

### Dependencies

- **NS-3**: Ensure NS-3 is properly installed and configured on your system.
- **Gnuplot**: Required for generating visualizations from simulation output data.

### Setup

1. Clone the repository:
   ```bash
   git clone <repository_url>
