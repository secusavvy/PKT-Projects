The trading floor Support Centre, with 600 staff, is relocating to a new building that currently lacks a network infrastructure. As a key member of the Networks Team, you are tasked with designing a robust network solution for the new building that not only meets current business needs but also ensures future scalability and redundancy. Here’s a detailed plan based on the requirements:

1. Logical Design Overview:
   - Utilize Cisco Packet Tracer for designing and implementing the network.
   - Adopt a hierarchical model with redundancy at every layer, incorporating two routers and two multilayer switches for high availability.

2. Departmental Layout:
   - First Floor:
     - Sales and Marketing Department (120 users)
     - Human Resource and Logistics Department (120 users)
   - Second Floor:
     - Finance and Accounts Department (120 users)
     - Administrator and Public Relations Department (120 users)
   - Third Floor:
     - ICT Department (120 users)
     - Server Room (12 devices)

3. Network Requirements:
   - Redundancy:
     - Connect the network to at least two ISPs for redundancy.
     - Each router connects to both ISPs using the provided public IP addresses (195.136.17.0/30, 195.136.17.4/30, etc.).

   - Wireless Networks:
     - Each department should have a dedicated wireless network for users.

   - VLAN and Subnetting:
     - Allocate each department to a separate VLAN and subnet within the base network 172.16.1.0, using subnetting to accommodate the required number of users.

   - DHCP and Static IP Assignment:
     - Implement DHCP servers in the server room for dynamic IP allocation to all devices.
     - Assign static IP addresses to devices in the server room.

   - Routing and Switching:
     - Configure multilayer switches to handle inter-VLAN routing and assign them IP addresses.
     - OSPF will be used as the routing protocol to advertise routes between routers and switches.

   - Security and Access Control:
     - Configure SSH on all routers and layer three switches for secure remote access.
     - Implement port-security on switchports in the Finance and Accounts department to allow only authorized devices using sticky MAC addresses and shutdown as violation mode.

   - NAT and ACLs:
     - Configure PAT (Port Address Translation) on the outbound router interface to use ISP-assigned IPv4 addresses.
     - Implement necessary ACL rules to control traffic flow.

4. Configuration Tasks:
   - Set up basic device settings including hostnames, console passwords, enable passwords, banner messages, and disable IP domain lookup.