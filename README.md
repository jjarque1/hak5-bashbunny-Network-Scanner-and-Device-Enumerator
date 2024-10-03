# Network Scanner and Device Enumerator

---

## Description

The **Network Scanner and Device Enumerator** is a payload designed to scan the local network and identify all connected devices. Using the popular tool `nmap`, this payload enumerates devices within a specified network range, providing an overview of network activity. This is particularly useful for network auditing and monitoring in controlled environments.

## How it Works

1. The payload opens a terminal session on a Linux machine.
2. It runs `nmap` to scan the local network (default range is 192.168.1.0/24, which can be adjusted).
3. The results of the scan, including IP addresses and MAC addresses of devices, are saved to a log file.
4. The log file is copied to the Bash Bunny's storage for later analysis.

## Requirements

- Target: Linux machine with `nmap` installed
- Bash Bunny in HID and storage mode

## Ethical Use Disclaimer

This payload is intended for ethical hacking and educational purposes only. Unauthorized scanning of networks without explicit permission is illegal and unethical. Ensure you have the proper authorization before running this script.

## Liability Disclaimer

The author of this payload assumes no responsibility for any illegal or unethical use of the code. This payload is provided as-is, and it is the user's responsibility to ensure its use complies with all applicable laws and regulations.

## Usage

1. Insert the Bash Bunny into the target machine.
2. The payload will automatically start a network scan using `nmap`.
3. Once the scan is complete, the results will be saved to `/network_scan.txt` on the Bash Bunny's storage.
4. Eject the Bash Bunny and review the scan results.
