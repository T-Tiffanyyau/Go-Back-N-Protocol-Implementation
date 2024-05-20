# Go-Back-N Protocol Implementation
The Go-Back-N Protocol Implementation is a practical venture into the development of a reliable data-transfer protocol. This project focuses on implementing the Go-Back-N protocol in Python, providing a deeper understanding of transport-layer protocols in computer networks.

## Installation
1. Clone or download the repository.
2. Ensure Python 3 is installed on your system. You can check this by running `python3 --version` in your command line.
3. Navigate to the downloaded project directory.

## Running the Simulator
To run the simulator with the specified configuration, use the following command:

```
python rdtsim.py -n 20 -l 0.05 -c 0.05 -v 2
```
Simulation Configuration
- (-n) Number of layer 5 messages to be provided: 20
- (-l) Loss probability: 0.05
- (-c) Corruption probability: 0.05
- (-v) Trace level: 2

Note: These variables can be changed to suit different testing and simulation requirements.

This configuration ensures that at least 20 messages are successfully transferred from the sender to the receiver, with a loss probability of 0.05, a corruption probability of 0.05, and a trace level of 2. The output will demonstrate how the protocol correctly recovers from packet loss and corruption.

## Features
- Reliable Data Transfer: Implements the Go-Back-N protocol for reliable data transfer between sender and receiver.
- Window Management: Manages a sliding window for packet transmission and acknowledgments.
- Checksum Calculation: Ensures data integrity using checksums for packets.
- Timer Management: Handles retransmissions using a single timer for multiple outstanding packets.
- ACK Handling: Uses acknowledgments (ACKs) for confirming received packets.
## Advanced Features
- Error Handling: Detects and handles packet loss and corruption.
- Efficiency: Optimizes packet transmissions to minimize retransmissions.
- Scalability: Supports different window sizes based on the simulation’s sequence number limit.
## Programming Concepts Covered
- Networking: Utilizes custom transport-layer protocol logic.
- Data Structures: Efficient use of lists for managing packets and window state.
- Error Handling: Robust exception handling for packet corruption and loss.
- Code Modularization: Organized into multiple classes and methods for readability and maintenance.


Last Updated: May 1, 2024

