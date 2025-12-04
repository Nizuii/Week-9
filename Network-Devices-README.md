# 1. HUB - The dumbest device (Layer 1)

<img src="images/hub.webp">

- Operates at OSI Layer 1
- Takes an electrical signal on one port and broadcast it to every other ports.
- No MAC table, No intelligence, No filtering. Its literally a multi port repeater.

**Functionality**

- Every device connected shares the same collision domain.
- If one device sends, everyone hears it.

**Security impact**

- Very Insecure
- Because it broadcasts all traffic to every port, an attacker can easily sniff packets with tools like Wireshark.
