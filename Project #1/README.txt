Ridoine company, a rapidly expanding organization based in Eastern Australia with a global customer base exceeding 2 million, specializes in the buying and selling of food items. They are planning to establish a new branch near the local village Bonalbo and are seeking young IT graduates to design the network infrastructure for this branch. This network will operate independently from the headquarters and has specific requirements for implementation:

1.Network Devices: Utilize one Cisco router and one Cisco switch.
2.Departments: Organize into three departments: Admin/IT, Finance/HR, and Customer Service/Reception.
3.VLAN Segmentation: Each department should reside in its own VLAN.
4.Wireless Access: Provide a wireless network for each department.
5.Automatic IP Addressing: Implement DHCP to assign IPv4 addresses to host devices.
6.Inter-Department Communication: Ensure devices across all departments can communicate with each other.

Given an ISP-assigned base network of 192.168.1.0, you, as the network engineer, are responsible for designing and implementing a solution that meets these requirements.

Technologies Implemented:

- Network Architecture: Establish a basic network using a single Cisco router for inter-VLAN routing and a Cisco switch for access.
- Cabling: Ensure correct cabling to connect all networking devices.
- VLAN Configuration: Create VLANs and assign ports to respective VLANs on the switch.
- Subnetting and IP Addressing: Plan subnetting within the 192.168.1.0 network to accommodate each department.
- Inter-VLAN Routing: Configure the router to enable communication between VLANs using the router-on-a-stick method.
- DHCP Server: Configure the router to act as a DHCP server, distributing IP addresses dynamically to devices.
- Wireless Network: Implement Cisco Access Points to provide wireless connectivity for users in each department.
- Host Device Configuration: Ensure all host devices automatically obtain IPv4 addresses via DHCP.