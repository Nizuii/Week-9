# What is OSI Model

- The goal in defining OSI model was to create a reference model that enables the communication of different technical systems via various devices and technologies and provides compatibility.
- The OSI model uses seven different layers, which are hierarchically based on each other to achieve this goal.
- These layers represent phases in the establishment of each connection through which the sent packets pass.
- In this way, the standard was created to trace how a connection is structured and established visually.

## OSI Model Layer

1. **Application Layer (Layer 7)**: Among other things, this layer controls the input and output of data and provides the application functions.
2. **Presentation Layer (Layer 6)**: The presentation layer's task is to transfer the system-dependent presentation of data into a form independent of the application.
3. **Session Layer (Layer 5)**: The session layer controls the logical connection between two systems and prevents, for example, connection breakdowns or other problems.
4. **Transport Layer (Layer 4)**: Layer 4 is used for end-to-end control of the transferred data. The Transport Layer can detect and avoid congestion situations and segment data streams.
5. **Network Layer (Layer 3)**: On the networking layer, connections are established in circuit-switched networks, and data packets are forwarded in packet-switched networks. Data is transmitted over the entire network from the sender to the receiver.
6. **Data Link Layer (Layer 2)**: The central task of layer 2 is to enable reliable and error-free transmissions on the respective medium. For this purpose, the bitstreams from layer 1 are divided into blocks or frames.
7. **Physical Layer (Layer 1)**: The transmission techniques used are, for example, electrical signals, optical signals, or electromagnetic waves. Through layer 1, the transmission takes place on wired or wiPhynctions of each OSI layer

## Functions of OSI Layer.

### 1. Application layer (Layer 1)

- Acts as the interface between user apps (ex: web browsers) & the network.
- Provides services like web browsing, file transfer, email. DNS, etc... So applications can send & recieve data.

### 2. Presentation layer (Layer 2)

- Converts data into a format that the recieving application can understand. (For example text, images, video formats).
- Handles encryption / decryption & compression / decompression of data for security & efficency.

### 3. Session layer (Layer 3)

- Start, Manages, Terminates **'Conversation'** (Session) between 2 devices or applications.
- Keeps tracks of who is talking to whom & can add checkpoints so communication can resume if interrupted.

### 4. Transport layer (Layer 4)

- Breaks down data into smaller pieces (Segments) & reassembles them at the other end.
- Ensures complete & correct delivery using error checking, retransmission & flow control. (eg: TCP/UDP)

### 5. Networking layer (Layer 5)

- Decides the best path for data to travel across different networks using logical address like IP.
- Handles routing, logical addressing & splitting / reassembling packets if they are too large.

### 6. Data link layer (Layer 6)

- Package data into frames & adds physical (MAC) address so devices on the same network can identify each other.
- Detects basic errors in frames & controls which device can use the shared medium at a given time.

### 7. Physical layer (Layer 7)

- Deals with the actual transmission of bits (0's and 1's) over cables, radio waves, fiber etc...
- Defines things like voltage levels, connectors, transmission speed & how bits are represented on the medium.

## Data Encapsulation & Decapsulation.

- Data encapsulation is the process of adding headers to data as it moves down the OSI layer at the sender & decapsulation is removing them as it moves up the layers at the reciever. Below is a step by step flow in simple terms.

**Encapsulation (Sender side)**: Each layer wraps the data from the layer above with its own control information before sending it.
**Decapsulation (Reciever side)**: Each higher layer removes its own control information recovering the original user data at the end.

### Encapsulation (From user to wire.)

- Message is sent in a chat app.  

#### 1. Application, Presentation, Session (layer 7-5)

- You type a message; the app generates "data".
- These top layers may format, encrypt or manage the session, but in OSI terms the unit is still just called "data".

#### 2. Transport Layer (layer 4)

- Splits the data into chunks & adds a transport header. (Source port, destination port, sequence numbers, etc...)
- Now the unit is called a segment (TCP) or datagrams (UDP).

#### 3. Network Layer (layer 3)

- Takes each segment & adds an IP header (source IP, destination IP, TTL, etc...)
- Now the unit is called a packet.

#### 4. Data Link Layer (layer 2)

- Takes each packet & adds a layer 2 header (source MAC & destination MAC, FCS / error-checked, etc...)
- Now the unit is called a frame.

#### 5. Physical Layer (layer 1)

- Converts the bits of the frames into electrical / optical / radio signals & sends them over the medium.
- On the air or wire, it is just a stream of bits.
