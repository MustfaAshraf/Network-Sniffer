# Network Sniffer Tool

Welcome to the Network Sniffer Tool project! This repository contains a Python-based network sniffer tool that captures and analyzes network traffic using the `scapy` library.

## Overview

This project provides a network sniffer tool implemented in Python, utilizing `scapy` for packet capture and analysis. The tool captures packets from a specified network interface, analyzes packet headers, identifies protocols (TCP, UDP, or others), and displays relevant information such as source and destination IP addresses, ports, and payload data.

## Features

- **Packet Capture**: Captures network packets in real-time.
- **Protocol Detection**: Identifies and categorizes packets based on TCP, UDP, or other protocols.
- **Payload Inspection**: Displays packet payload for deeper analysis.

## Functionality

### Packet Capture and Analysis

The `network_sniffer.py` script:
- Uses `scapy` to sniff packets on the network interface.
- Analyzes packets to extract:
  - Source and destination IP addresses.
  - Protocol type (TCP, UDP, or Other).
  - Source and destination ports.
  - Payload data if available.

## Usage

To use this tool:
1. Ensure you have Python installed along with the `scapy` library (`pip install scapy`).
2. Run the `network_sniffer.py` script with appropriate permissions (e.g., sudo on Unix-like systems).
3. The tool will start capturing and displaying network packets in real-time.

## Example

```plaintext
Example output from the network sniffer tool:

Packet:
Source IP:  192.168.1.100
Destination IP:  8.8.8.8
Protocol: UDP
Source port:  12345
Destination port:  53
Payload:
"Hello, world!"

Packet:
Source IP:  8.8.8.8
Destination IP:  192.168.1.100
Protocol: UDP
Source port:  53
Destination port:  12345
Payload:
"Response from server"
```
## Contributing
Contributions to enhance packet analysis capabilities, add support for additional protocols, improve performance, or enhance documentation are welcome. Fork this repository, implement your changes, and submit a pull request. For significant changes, please open an issue to discuss the proposed modifications.

Explore network traffic and deepen your understanding of networking with the Network Sniffer Tool! 🌐🔍
