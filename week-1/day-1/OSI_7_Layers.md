# Day 1 - OSI 7 Layers

## OSI 7 Layers
1. Physical Layer
2. Data Link Layer
3. Network Layer
4. Transport Layer
5. Session Layer
6. Presentation Layer
7. Application Layer

### Layer 1 - Physical Layer
- Carry a bit stream (0 and 1) over a physical medium.
- Physical medium (Electrical, Optical, Radio Frequency)
- Simplex, Half Duplex, Full Duplex

### Layer 2 - Data Link Layer
- Data in this layer is called Frames.
- Error Detection and Correction. (Error-free data transmission)
- Physical Addressing (MAC Address - 48 bits)
- Access Control (Who can send data and when)

### Layer 3 - Network Layer
- Data in this layer is called Packets.
- Logical Addressing (IPv4 - 32 bits, IPv6 - 128 bits)
- Routing (Selecting best path for data transmission)
- Fragmentation (Breaking large packets into smaller packets)
- Inter-Networking (Connecting multiple networks)

### Layer 4 - Transport Layer
- Data in this layer is called Segments.
- Process-to-Process Communication (Application to Application)
- Connection Control (Connection-oriented, Connectionless)

### Layer 5 - Session Layer
- Dialog Control (Half Duplex, Full Duplex)
- Synchronization (Data flow synchronization)
  - Checkpointing (Data recovery)

### Layer 6 - Presentation Layer
- Data Translation (Data format translation)
- Data Encryption (Data security)
- Data Compression (Data size reduction)

### Layer 7 - Application Layer
- Access to Network Resources (File, Database, Email, Web)
- User Interface (User interaction with the network)
- Application Services (Network services)
- Network Virtual Terminal (Remote login)

## How OSI 7 Layers Work?
- Data is encapsulated at each layer.
- Data is decapsulated at each layer.
- Each layer adds and removes its own header and footer.
- Each layer communicates with its peer layer.

![OSI 7 Layers]('images/osi-7-layers.png' 'OSI 7 Layers')
