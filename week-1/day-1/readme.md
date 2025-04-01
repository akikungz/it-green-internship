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
  - Electrical: Copper, Coaxial, Twisted Pair
  - Optical: Fiber
  - Radio Frequency: Wireless, Satellite

#### Thai Language
- ส่งข้อมูลในรูปแบบของบิต (0 และ 1) ผ่านสื่อที่เป็นกลไกทางกายภาพ เช่น สายทองแดง, สายไฟเบอร์, Wi-Fi

<!--
- Simplex, Half Duplex, Full Duplex
  - Simplex: One-way communication (TV, Radio)
  - Half Duplex: Two-way communication but not simultaneously (Walkie-Talkie)
  - Full Duplex: Two-way communication simultaneously (Mobile Phone)
-->

### Layer 2 - Data Link Layer
- Data in this layer is called Frames.
- Error Detection and Correction. (Error-free data transmission)
- Physical Addressing (MAC Address - 48 bits)
- Access Control (Who can send data and when)
- Framing (Frame delimiting, Addressing, Error detection)
- Flow Control
  - Stuffed Bits (Prevent data loss)
  - Sliding Window (Data transmission speed)

#### Thai Language
- ส่งข้อมูลในรูปแบบของเฟรม โดยมีการตรวจจับและแก้ไขข้อผิดพลาดในข้อมูล มีการกำหนดที่อยู่ของอุปกรณ์ในเครือข่าย และควบคุมการเข้าถึง รวมถึงการควบคุมการไหลของข้อมูล

### Layer 3 - Network Layer
- Data in this layer is called Packets.
- Logical Addressing (IPv4 - 32 bits, IPv6 - 128 bits)
- Routing (Selecting best path for data transmission)
- Fragmentation (Breaking large packets into smaller packets)
  - MTU (Maximum Transmission Unit)
- Inter-Networking (Connecting multiple networks)

#### Thai Language
- ส่งข้อมูลในรูปแบบของแพ็กเก็ต มีการกำหนดที่อยู่ของอุปกรณ์ในเครือข่าย และเลือกเส้นทางที่ดีที่สุดสำหรับการส่งข้อมูล และแบ่งแพ็กเก็ตใหญ่เป็นแพ็กเก็ตเล็กๆ ตามขนาด

### Layer 4 - Transport Layer
- Data in this layer is called Segments.
- Process-to-Process Communication (Application to Application)
- Connection Control (Connection-oriented, Connectionless)

| Details | TCP | UDP |
|---|---|---|
| Connection | Connection-oriented | Connectionless |
| Reliability | Reliable | Unreliable |
| Error Detection | Yes | No |
| Error Correction | Yes | No |
| Flow Control | Yes | No |
| Ports | 0 to 65535 | 0 to 65535 |
| Examples | HTTP, FTP, SMTP | DNS, DHCP, TFTP |

![TCP vs UDP](images/tcp_udp.jpg 'TCP vs UDP')

#### Thai Language
- ส่งข้อมูลในรูปแบบของเซกเมนต์ มีการควบคุมการเชื่อมต่อระหว่างโปรแกรม และมีการควบคุมการส่งข้อมูล
- การส่งข้อมูลแบบ TCP เป็นการส่งข้อมูลที่มีการตรวจสอบการเชื่อมต่อ และการยืนยันข้อมูลระหว่างการส่ง
- การส่งข้อมูลแบบ UDP เป็นการส่งข้อมูลที่ไม่มีการตรวจสอบใดๆ เน้นความไวและไม่สนใจข้อมูลที่สูญหาย

### Layer 5 - Session Layer
- Dialog Control (Half Duplex, Full Duplex)
- Synchronization (Data flow synchronization)
  - Checkpointing (Data recovery)

Examples:
- NetBIOS (Network Basic Input/Output System)
- RPC (Remote Procedure Call)

#### Thai Language
- ควบคุมการสนทนาระหว่างโปรแกรม และควบคุมการสร้างการเชื่อมต่อระหว่างโปรแกรม

### Layer 6 - Presentation Layer
- Data Translation (Data format translation)
- Data Encryption (Data security)
- Data Compression (Data size reduction)

Examples:
- ASCII (American Standard Code for Information Interchange)
- EBCDIC (Extended Binary Coded Decimal Interchange Code)
- Media Formats (JPEG, MP3, MPEG)
- Encryption (SSL, TLS)
- Compression (ZIP, RAR)
- Translation (EBCDIC to ASCII)

#### Thai Language
- แปลงรูปแบบข้อมูล และเข้ารหัสข้อมูล และบีบอัดข้อมูล ก่อนส่งข้อมูล

### Layer 7 - Application Layer
- Access to Network Resources (File, Database, Email, Web)
- User Interface (User interaction with the network)

| Application | Protocol | Port |
|---|---|---|
| Web | HTTP | 80/tcp |
| File | FTP | 21/tcp |
| Email | SMTP | 25/tcp |
| Remote Login | Telnet | 23/tcp |
| Remote Login | SSH | 22/tcp |
| Name Resolution | DNS | 53/tcp, 53/udp |
| Dynamic Host Configuration Protocol | DHCP | 67/udp, 68/udp |

#### Thai Language
- เป็นการสื่อสารระหว่าง User กับ Network และเข้าถึงทรัพยากรต่างๆในระบบเครือข่าย เช่น ไฟล์, ฐานข้อมูล, อีเมล, เว็บ

![OSI 7 Layers](images/osi_7_layers.png 'OSI 7 Layers')

<!--
![Hop to Hop](images/hop_to_hop.png 'Hop to Hop')

![Source to Destination](images/source_to_destination.png 'Source to Destination')
-->
