To design and implement the network for Vic Modern Hotel, we'll follow the provided requirements and utilize Cisco Packet Tracer for simulation. Here’s a detailed plan based on the specifications:

### Network Design Overview:

1. Floor Layout:
   - First Floor:
     - Reception (VLAN 80, 192.168.8.0/24)
     - Store (VLAN 70, 192.168.7.0/24)
     - Logistics (VLAN 60, 192.168.6.0/24)
   - Second Floor:
     - Finance (VLAN 50, 192.168.5.0/24)
     - HR (VLAN 40, 192.168.4.0/24)
     - Sales/Marketing (VLAN 30, 192.168.3.0/24)
   - Third Floor:
     - Admin (VLAN 20, 192.168.2.0/24)
     - IT (VLAN 10, 192.168.1.0/24)

2. Device Placement:
   - Each floor will have a Layer 2 switch.
   - All three floors will be interconnected via routers placed in the IT department's server room.

3. Wireless Networks:
   - Each floor will have a Wi-Fi network for laptops and phones.

4. Printers:
   - Each department will have a printer.

5. Routing and VLAN Configuration:
   - Routing Protocol: OSPF will be used to advertise routes between routers.
   - VLANs: Each department will be assigned to a VLAN as specified.

6. IP Addressing:
   - Subnetting will be based on the provided network ranges for each department.

7. DHCP:
   - Each router will act as a DHCP server for its respective floor.

8. SSH Configuration:
   - SSH will be configured on all routers for secure remote access.

9. Port Security:
   - Port security will be configured on the switch in the IT department to restrict access to port fa0/1 using the sticky method for MAC address learning.

### Configuration Steps:

1. Network Topology:
   - Use Cisco Packet Tracer to visually design the network topology with three floors interconnected via routers, each connecting to a Layer 2 switch on the respective floor.

2. VLAN and IP Address Assignment:
   - Configure VLANs and assign IP addresses as per the specified subnet ranges on each switch.

3. Inter-VLAN Routing:
   - Implement inter-VLAN routing using the router-on-a-stick method on the routers.

4. DHCP Configuration:
   - Configure DHCP pools on each router to provide dynamic IP addresses to devices in each department.

5. OSPF Configuration:
   - Enable OSPF on all routers to advertise subnets and establish routing between floors.

6. SSH Configuration:
   - Configure SSH on all routers for secure remote management.

7. Port Security Configuration:
   - On the switch in the IT department, configure port security on port fa0/1 to allow only the Test-PC using the sticky MAC address method with shutdown violation mode.

8. Wireless Network Configuration:
   - Deploy Cisco Access Points on each floor to provide wireless connectivity.