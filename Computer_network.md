# Networking Models: OSI and TCP/IP

## OSI Model
The **Open Systems Interconnection (OSI) model** describes how computer systems communicate over a network. Developed by the **International Organization for Standardization (ISO)**, it standardizes network communication into **seven layers**:

### Layers of an OSI Model
1. **Physical Layer**  
   - Transmits raw data between a device and a physical medium.
   - Manages electrical, optical, and mechanical aspects of data transmission.

2. **Data Link Layer**  
   - Ensures reliable data transfer between devices on the same network.
   - Handles MAC addressing and error detection.

3. **Network Layer**  
   - Manages logical addressing and routing of packets.
   - Uses IP addressing for communication across different networks.

4. **Transport Layer**  
   - Manages data delivery between systems and hosts.
   - Ensures reliable transmission, error checking, and flow control.

5. **Session Layer**  
   - Manages connection establishment, maintenance, and termination.
   - Handles authentication and reconnections after interruptions.

6. **Presentation Layer**  
   - Translates data formats between the application and network.
   - Handles encryption, compression, and data formatting.

7. **Application Layer**  
   - Provides network services directly to applications.
   - Examples include HTTP, SMTP, and FTP.

![image](https://github.com/user-attachments/assets/b270a65a-8cbf-4350-a6c8-14059085f191)
*Diagram of an OSI model*

The **OSI model** ensures different systems can communicate using standardized protocols.

---

## TCP/IP Model
The **Transmission Control Protocol/Internet Protocol (TCP/IP) model** defines how data is transmitted across networks. It consists of **four layers**, each with specific functions.

### TCP/IP Model Layers
1. **Application Layer**  
   - Interfaces with user applications like web browsers and email clients.
   - Protocols: HTTP, SMTP, FTP.

2. **Transport Layer**  
   - Manages reliable communication between devices.
   - Handles data segmentation, flow control, and error detection.
   - Protocols: TCP (Transmission Control Protocol), UDP (User Datagram Protocol).

3. **Internet Layer**  
   - Manages logical addressing and routing of data packets.
   - Uses IP (Internet Protocol) for addressing and determining the best path.

4. **Network Interface Layer**  
   - Handles physical transmission of data on the network.
   - Interacts directly with network hardware like network cards.
   - Manages data frames on the local network.

The **TCP/IP model** is the foundation of modern internet communication, streamlining network functions into fewer layers than the OSI model.

---

### Key Differences Between OSI and TCP/IP
| Feature         | OSI Model (7 Layers)        | TCP/IP Model (4 Layers)      |
|---------------|----------------------|----------------------|
| **Developed By** | ISO                   | DARPA (U.S. Department of Defense) |
| **Purpose** | Conceptual framework for standardizing network communication | Practical model for real-world networking |
| **Number of Layers** | 7 | 4 |
| **Application Support** | Application, Presentation, and Session layers | Combined into one Application layer |
| **Network Routing** | Network Layer | Internet Layer |
| **Reliability Control** | Transport Layer | Transport Layer |

---

### Summary
- **The OSI model** is a theoretical framework for standardizing network communication.
- **The TCP/IP model** is a practical model used for real-world internet communication.
- TCP/IP consolidates some OSI layers, making it more streamlined and widely adopted.
