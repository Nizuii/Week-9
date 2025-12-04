# What is UDP

<img src="images/UDP-gif.gif">

- **UDP** stands for User Datagram Protocol.
- UDP Ensures:

  - No handshake.
  - No reliability.
  - No retransmission.
  - Just sends packets blindly.

Because of this:
- Its much faster than TCP
- But not reliable as TCP

## What is UDP used for

Anywhere where speed is important than accuracy.

- Video streaming
- Online gaming
- VoIP calls
- DNS Lookups
- DHCP

If 1 frame or 1 voice packet is lost user won't notice.

## cybersecurity relevance

### 1. UDP Flood Attack

UDP Flood attack is a type of DDOS Attack where attacker sends massive amounts of UDP packets to the random pets of target system.

The goal is to overwhelm the target system by making it soncume its:

- Bandwidth
- CPU
- Memory
- Application stack

#### Working Mechanism

**1.** Attacker sends a huge number of UDP packets to the victim.
**2.** Packets are sent to random ports.
**3.** The victim machine receives a packet on a port with no application listening, so it must:

- Check the port
- Realize nothing is running
- Respond with an ICMP “Port Unreachable” message  
**4.** This reply consumes:

- CPU
- Outbound bandwidth
- kernal resources

> When millions of such packets hit per second → system becomes overloaded.
