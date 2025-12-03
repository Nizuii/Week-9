# What is OSI Model

- The goal in defining OSI model was to create a reference model that enables the communication of different technical systems via various devices and technologies and provides compatibility.
- The OSI model uses seven different layers, which are hierarchically based on each other to achieve this goal.
- These layers represent phases in the establishment of each connection through which the sent packets pass.
- In this way, the standard was created to trace how a connection is structured and established visually.

1. **Application Layer (Layer 7)**: Among other things, this layer controls the input and output of data and provides the application functions.
2. **Presentation Layer (Layer 6)**: The presentation layer's task is to transfer the system-dependent presentation of data into a form independent of the application.
3. **Session Layer (Layer 5)**: The session layer controls the logical connection between two systems and prevents, for example, connection breakdowns or other problems.
4. **Transport Layer (Layer 4)**: Layer 4 is used for end-to-end control of the transferred data. The Transport Layer can detect and avoid congestion situations and segment data streams.
5. **Network Layer (Layer 3)**: On the networking layer, connections are established in circuit-switched networks, and data packets are forwarded in packet-switched networks. Data is transmitted over the entire network from the sender to the receiver.
6. **Data Link Layer (Layer 2)**: The central task of layer 2 is to enable reliable and error-free transmissions on the respective medium. For this purpose, the bitstreams from layer 1 are divided into blocks or frames.
7. **Physical Layer (Layer 1)**: The transmission techniques used are, for example, electrical signals, optical signals, or electromagnetic waves. Through layer 1, the transmission takes place on wired or wireless transmission lines.
