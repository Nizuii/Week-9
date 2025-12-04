# What is TCP

<img src="images/tcp.jpg">

- **TCP** stands for Transmission Control Protocol.
- **TCP** works in layer 3 in **TCP/IP** & layer 4 in **OSI** model.
- **TCP** ensures:  

  - No data loss.
  - Packet arrive in correct order.
  - Retransmission happens if something is missing.
  - Connection-based communication.

## How TCP atually starts.

- **TCP** uses the **3 way handshake**:

  1. **Client** ➡️ **Server**: SYN (I want to connect)
  1. **Server** ➡️ **Client**: SYN-ACK (I'm Ready)
  1. **Client** ➡️ **Server**: SYN (Lets go)  

> Connection is created and data transmission begins

## What is TCP good for:

Anything where acuracy matters like:

- Web browsing (HTTP/HTTPS)
- File Transfer (FTP, SFTP)
- Email (SMTP/IMAP)
- SSH
- Database Communication

## What are TCP Flags

<img src="images/tcp-flags.png">

- **TCP Flags** are single bit indicators inside the TCP header.
- Each flag is either 0's (off) & 1's (on).
- When "on", they signal a specific type of operation in the connection cycle.
- There are 8 main TCP Flags.

### 1. SYN (Synchronize)

Used to start a connection.
- This is basically the **"Hey I want to connect signal"**
