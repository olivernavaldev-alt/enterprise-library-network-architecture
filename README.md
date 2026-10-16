LibEase: Enterprise Library Network Architecture

A full enterprise-style network for a library, designed and simulated in Cisco Packet Tracer 8.x. LibEase is built to be redundant, secure, and always on, so that staff and patrons keep reliable access to library services even when a link or device fails.

The project file is Library_Network.pkt.

Overview

LibEase models the network of a modern library that serves several types of users: library staff, patrons on public workstations, and guests on wireless. The design separates these groups into their own VLANs, protects internal resources from guest traffic, and removes single points of failure at both the gateway and internet-connection levels.

The network includes:

Segmented VLANs that separate staff, patron, server, and guest traffic
Dual ISP connections for internet redundancy
HSRP gateway failover so hosts keep a working default gateway if a router fails
Rapid PVST+ for fast, loop-free Layer 2 convergence
ACLs that restrict guest access to internal resources
FTP and DNS servers providing file sharing and name resolution
Wireless access for patrons and guests
Objectives
Segment the network. Use VLANs to isolate different user groups and improve both performance and security.
Ensure high availability. Provide redundancy at the gateway (HSRP), the Layer 2 switching layer (Rapid PVST+), and the WAN edge (dual ISPs) so a single failure does not cause an outage.
Secure guest access. Apply access control lists so guest users can reach the internet but not internal library systems.
Provide core network services. Deploy FTP and DNS servers to support file transfer and name resolution across the network.
Support wireless connectivity. Offer wireless access for staff and visitors while keeping it properly segmented.
Demonstrate enterprise design practices. Apply real-world networking concepts in a simulated environment using Cisco Packet Tracer.
