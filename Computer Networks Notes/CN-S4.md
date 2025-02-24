Routing
- Wireless router generating network


Static
- Manually create and manage routing table entries
- Use command line utilities to display, modify, and create routes
- Routes remain unchanged until manuallu updated

- Suitable for Small networks & environment where network is static

- Scalability issue

Dynamic
- Used when static route is impractical due to frequent change on routing table

Ruting information protocol (RIP)
- Send routing table to everything every 30 seconds
- Use Hop count as metric for distance
- Each router = 1 hop

Open shortest path first (OSPF)
- Uses link state advertisement (LSAs)
- No hop count
- Use djikstra algorithm for route efficiency
- Efficient and faster convergence than RIP
- Require to use medium level of power and storage on routers

Enhance interior gateway routing protocol (EIGRP) (Interior of Network)
- Hybrid: Distance vector and link state mashup
- Use neighbor discovery message to gather route information to find out which computer is connected to the router
- Using bandwidth, traffic congestion, transmission delay, reliability, and MTU size
- More scabale than RIP and support autonomous system for larger networks

Border Gateway protocol (BGP) (Exterior of Network)
- Used IPv4 and IPv6
- Scalable than RIP and OSPF
- Manage hundreds of routes
- Require ssubstantial process power, memory and storage
- Use for banking or multinational countries

Administrative Distance
- Set of values to determine te trustworthiness of a route based on its source

Bandwidth Management
- Network layer is responisble for end-to-end communication
- Make sure there is no bottleneck and computers can manage
Different types:
- File transfer: tolerate relays and transmission
- Web Traffic: Tolerate delays and lost bits
- Streaming audio/video: can buffer data and handle packet loss
Real time apps:
- Sensitive to delays and lost data
- Dropped calls or data corruption

Purpose:
- prioritize traffic to ensure cirtical application receive the necessary bandwidth

