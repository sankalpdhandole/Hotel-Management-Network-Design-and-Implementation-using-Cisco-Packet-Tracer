 Hotel-Management-Network-Design-and-Implementation-using-Cisco-Packet-Tracer
Detailed Project Description for Interviews

Project Title: Design and Implementation of Vic Modern Hotel Network

Project Objective:
The objective of this project was to design and implement a robust, secure, and efficient network for Vic Modern Hotel, covering three floors with multiple departments. The network needed to support both wired and wireless devices, ensure secure access, and provide seamless communication across all departments.

Project Scope:
- Three Floors: Each floor has specific departments with unique network requirements.
- Devices: Included routers, switches, access points, PCs, printers, laptops, and phones.
- Connectivity: Both wired and wireless.
- Security: Implementing secure protocols and configurations.

1. Network Topology Creation
- Devices Placement:
  - Placed three routers in the server room on the third floor.
  - Placed one switch per floor to manage the network devices on that floor.
  - Deployed access points on each floor to provide Wi-Fi connectivity.

- Device Connections:
  - Connected the routers using serial DCE cables to establish a backbone network with IP subnets 10.10.10.0/30, 10.10.10.4/30, and 10.10.10.8/30.
  - Connected each switch to its respective router using Ethernet cables.
  - Connected end devices such as PCs, printers, and phones to switches and access points for wired and wireless connectivity.

2. IP Addressing and VLAN Configuration
- Router Interconnections:
  - Assigned IP addresses to the router interfaces using the specified subnets for inter-router communication.

- VLANs:
  - Created VLANs for each department to logically segment the network:
    - Reception (VLAN 80)
    - Store (VLAN 70)
    - Logistics (VLAN 60)
    - Finance (VLAN 50)
    - HR (VLAN 40)
    - Sales/Marketing (VLAN 30)
    - Admin (VLAN 20)
    - IT (VLAN 10)
  - Assigned appropriate IP address ranges to each VLAN to manage traffic efficiently.

3. Routing and DHCP Configuration
- Routing Protocol:
  - Configured OSPF (Open Shortest Path First) on all routers to enable dynamic routing and ensure efficient data packet forwarding between VLANs and floors.

- DHCP Configuration:
  - Set up DHCP on each router to dynamically assign IP addresses to devices within their respective VLANs, ensuring efficient IP management and reducing manual configuration.

- SSH Configuration:
  - Enabled SSH (Secure Shell) on all routers for secure remote access, allowing administrators to manage the routers securely from remote locations.

4. Switch Configuration
- VLAN Assignment:
  - Created VLANs on each switch and assigned the correct ports to each VLAN to ensure devices within the same department can communicate and are isolated from other departments.

- Trunk Ports:
  - Configured trunk ports on switches to carry traffic from multiple VLANs, allowing inter-VLAN communication through a single physical link between switches and routers.

5. Port Security Configuration
- Port Security:
  - Implemented port security on the IT department switch to restrict access to a specific port (fa0/1) using the sticky method, allowing only the Test-PC to connect. This enhanced security by preventing unauthorized devices from accessing critical network segments.

6. Access Point Configuration
- Wi-Fi Networks:
  - Configured wireless networks on each access point to provide seamless connectivity for wireless devices. Ensured that each floor’s wireless network was connected to its respective VLAN, enabling wireless devices to obtain IP addresses dynamically and communicate within their VLAN.

7. Testing and Verification
- Inter-VLAN Routing:
  - Tested communication between devices in different VLANs to ensure proper inter-VLAN routing was functioning, verifying that data packets were correctly forwarded between departments.

- DHCP Assignment:
  - Verified that devices on each VLAN received IP addresses from the correct DHCP pools, ensuring dynamic IP assignment was functioning as expected.

- SSH Access:
  - Tested SSH access from the Test-PC to routers to confirm secure remote management capabilities.

- Port Security:
  - Ensured that only the Test-PC could access the restricted port on the IT department switch, verifying the effectiveness of the port security configuration.

- Overall Network Communication:
  - Conducted comprehensive testing to ensure all devices could communicate with each other as required, both within and across VLANs, and that the network met all operational requirements.

 Summary
This project involved designing and implementing a hierarchical network for Vic Modern Hotel, incorporating advanced features such as VLANs, dynamic routing with OSPF, DHCP for dynamic IP addressing, secure remote access with SSH, and port security. The successful implementation and thorough testing ensured a robust, secure, and efficient network capable of meeting the hotel's connectivity and operational needs. Through this project, I demonstrated my ability to plan, design, implement, and test a complex network, addressing both wired and wireless connectivity while ensuring robust security measures.
