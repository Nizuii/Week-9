# What is OSI Model?

- The Open System Interconnection model is a theoratical framework that provides how data moves across a network into 7 layers.
- Its simply a blueprint. A way to understand how communication happens between 2 devices.
- The OSI layer exists to make networking understandable, structured and standard.
- Its purpose is to:
  
  1. Breakdown complex network communication into smaller pieces.
  2. Provide common language for engineers, developers, cyber security analysts.
  3. Organize protocols & technologies into the right layers.
  4. Help troubleshoot issues layer by layer.

## Why it was created?

- Because different companies used to make systems that couldn't talk to each other. The OSI model was created to unify networking approaches.

## How OSI layer is helpful in cyber security.

- To understand attack layer wise.
- To spot vulnerabilities based on layers.
- To troubleshoot professionally.
- To read packets & logs with purpose.
- To understand how data flows in a network.

## Working example:

### Layer 7 - Application Layer
- Your browser sends an HTTP/HTTPS request:
  
  > google.com

- **Protocols**: HTTP, HTTPS, DNS

### Layer 6 - Presentation Layer
- Your data gets:

  - Encrypted (TLS/SSL)
  - Compressed (If needed)
  - Formatted for transmission.

- This is where HTTPS -> TLS kicks in.
- **Protocols**: TLS, SSL
- **Attacks Example**: SSL Stripping

### Layer 5 - Session Layer

-
