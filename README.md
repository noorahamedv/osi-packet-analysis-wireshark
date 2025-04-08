# OSI Packet Analysis using Wireshark

This project explores deep packet inspection of network protocols using Wireshark, mapped to the OSI model. The analysis covers InfiniBand, CIPSO, and SIP signaling with visual insights from I/O and flow graphs.

## 📁 Files Included
- [`Assignment_1_OSI_Analysis.pdf`](report/Assignment_1_OSI_Analysis.pdf): Full report with detailed protocol breakdown
- Wireshark visualizations: Protocol Hierarchy Stats, I/O Graphs, and Flowgraphs
- Sample data captures in `data/` folder

## 🛠️ Tools & Technologies
- Wireshark
- PCAP sample files from Wireshark Wiki
- OSI Layered Networking Model
- lab.dynamite.ai (for visualization)

## 📊 Packet Capture Analyses

### 1. `infiniband.cap`
- High-performance InfiniBand and UDP communication
- Subnet management messages: `SubnGet`, `SubnGetResp`
- ICMPv6 and ARP communication breakdown
- Wireshark I/O Graph: Burst at beginning, suggesting packet spike

### 2. `ipv4_cipso_option.pcap`
- CIPSO enforcement in secure IPv4 networks
- Loopback ping behavior (`127.0.0.1`) with TTL = 64
- Internal echo requests/replies visualized using ICMP protocol
- Stable packet trends in the I/O graph

### 3. `DTMFsipinfo.pcap`
- SIP INVITE, CANCEL, INFO messages for VoIP session
- UDP transport, media negotiation via SDP
- Flowgraph visualization of SIP dialogs
- Byte transmission graph shows burst communication trends

## ✅ Key Learnings
- Mapped real-world packet flows to OSI model
- Understood protocol-specific roles and usage contexts
- Practiced analyzing packet headers and behaviors for diagnosis

## 📎 References
- [Wireshark Sample Captures](https://wiki.wireshark.org/SampleCaptures)
- [OSI Model Overview](https://en.wikipedia.org/wiki/OSI_model)
- [lab.dynamite.ai](https://lab.dynamite.ai/) - Visualization tool

