# PortScanner

# pscan.py – Port Scanner

## Overview

This Python-based command-line tool performs TCP port scanning and basic banner grabbing for a given target host. It allows users to detect open ports, attempt TCP connections, and retrieve available service banners. Intended for educational use and legal internal testing environments.

## Functionality

- Resolves hostnames to IP addresses
- Iterates over a list of user-defined TCP ports
- Attempts to establish a socket connection with each port
- If connected, sends a basic probe and prints the banner (if available)
- Handles common socket errors and timeouts gracefully

## Prerequisites

- Python 3.6 or higher
- Command-line access to run the script
- Internet or intranet connectivity to the target host
- Legal authorization to scan the target host

## How to Run

1. Open a terminal or command prompt.
2. Navigate to the folder containing `port_scanner.py`.
3. Run the following command:

```CL
python pscan.py -t <target-host> -p <comma,separated,ports>
```

## Notes
-Not all ports return banners. Some services do not respond until specific protocol messages are sent.
-Target servers may block repeated or unauthorized scans.
-If the script exits without results, double-check your input and ensure the ports are accessible.
-The script uses a 5-second timeout per connection by default.
-This tool is for educational and ethical use only—you are responsible for ensuring you have permission to scan any target.
