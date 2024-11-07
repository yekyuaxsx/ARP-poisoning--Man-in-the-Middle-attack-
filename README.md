# ARP poisoning (Man-in-the-Middle attack)

This Python script performs ARP (Address Resolution Protocol) poisoning, a type of Man-in-the-Middle (MitM) attack. ARP poisoning allows an attacker to intercept or manipulate traffic between devices in a local network. The tool works by sending false ARP responses to the target device and the gateway, redirecting the network traffic through the attacker's machine.

## Features:

- **ARP Poisoning:** Sends forged ARP packets to target devices to mislead them into sending their traffic through the attacker's machine.
- **Target and Gateway Configuration:** Allows users to specify the target IP and the gateway IP for the attack.
- **Automatic Packet Sending:** Continuously sends ARP poisoning packets until manually stopped.
- **Reset Function:** Restores the network to its normal state by resetting the ARP tables on the target and gateway devices.

## Usage:

1. **Clone the repository.**
2. **Install the required dependencies:**

   ```bash
   pip install scapy
   ```

3. **Run the script with the target IP and gateway IP as arguments:**

   ```bash
   python arp_spoofing.py --target <target_ip> --gateway <gateway_ip>
   ```

4. **To stop the attack, press `Ctrl + C`.** The script will automatically restore the ARP tables.

## Disclaimer:

This script is intended for educational purposes and ethical hacking within networks where you have explicit permission to perform penetration testing. Unauthorized use of ARP poisoning can be illegal and unethical.
