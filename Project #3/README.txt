Radeon Company Ltd., a US-owned firm specializing in Banking and Insurance, is expanding its operations into Africa, starting with a new branch in Nairobi, Kenya. They have acquired a four-story building within the city and are seeking final-year students from a local university to design and implement their network infrastructure. As a student taking on this role, it's crucial to carefully analyze and fulfill the following requirements to meet the company's needs:

1.Network Topology Visualization:
   - Utilize a software modeling tool like MS Visio, Visual Paradigm, or Draw.io to design a hierarchical network topology that encompasses all floors and departments.

2.Network Simulation Software:
   - Implement the designed topology using Cisco Packet Tracer or GNS3 for realistic network simulation and configuration.

3.Routing Protocol:
   - Use OSPF (Open Shortest Path First) as the routing protocol to advertise routes across the network.

4.Wireless Networks:
   - Each department should have a dedicated wireless network to cater to approximately 60 users, both wired and wireless.

5.Automatic IP Address Assignment:
   - Implement DHCP (Dynamic Host Configuration Protocol) servers to assign IPv4 addresses dynamically to all host devices.

6.Inter-Department Communication:
   - Ensure seamless communication between devices in all departments.

7.Server Requirements:
   - Create HTTP and E-mail servers within the network infrastructure.

8.IP Address Planning:
   - Base network: 192.168.10.0
   - Perform subnetting based on the number of hosts required per department. Determine subnet masks, usable IP address ranges, and broadcast addresses for each subnet.

9.Device Configurations:
   - Configure all end devices with appropriate IP addresses based on subnet calculations.
   - Implement port-security on switches using sticky MAC address learning and shutdown violation mode.

10.Security Configurations:
    - Configure SSH (Secure Shell) on all routers for secure remote login.
    - Implement basic device settings including hostnames, passwords (console and enable), banner messages, disable domain IP lookup, and encrypt configured passwords.

11.VLAN Implementation:
    - Assign each department to a different VLAN and configure VLANs on switches accordingly.