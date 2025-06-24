# finmark-platform-tech

The **three-tier architecture** is a hierarchical network design that divides the network into three layers: core, distribution, and access. The core layer serves as the high-speed backbone, the distribution layer manages routing, security policies, and VLANs, and the access layer connects end-user devices. This structure offers benefits such as scalability, easier management, high performance, and support for redundancy and security policies. However, it also introduces higher costs, added complexity, and potential latency. While ideal for medium to large networks requiring robust performance and reliability, it may be excessive for smaller environments.

The Three-Tier Network Architecture enhances security by introducing multiple control points across different layers. Each tier can enforce specific security policies, creating a layered defense strategy known as **defense-in-depth**.

1. Access Layer
    - Port Security: Limits access to specific MAC addresses.
    - 802.1X Authentication: Controls user/device access via identity-based policies.
    - VLAN Segmentation: Isolates users/devices to contain threats.
    - DHCP Snooping & Dynamic ARP Inspection (DAI): Prevents IP spoofing and man-in-the-middle attacks.
    - PoE Security: Restricts power to trusted devices only.
2. Distribution Layer
    - Access Control Lists (ACLs): Filters traffic between VLANs and enforces security rules.
    - Routing Boundaries: Controls communication paths and isolates broadcast domains.
    - Network Policy Enforcement: Applies QoS, firewall rules, and route filtering.
    - Redundancy with Security: Uses secure routing protocols (e.g., EIGRP with authentication).
3. Core Layer
    - Fast, Secure Transport: Ensures high-speed encrypted data flow across the enterprise.
    - Policy-Based Routing: Directs sensitive traffic through firewalls or IDS/IPS.
    - Minimal Services: Reduces attack surface (no unnecessary services or protocols).