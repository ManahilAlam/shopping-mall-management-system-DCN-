# shopping-mall-management-system-DCN-
The objective of this project is to design and implement a robust, secure, and efficient network for a shopping mall system. The network will facilitate communication between all devices and departments within the mall, ensuring seamless operations and enhancing the overall shopping experience for customers.

Design and Implementation of shopping mall management system
1. INTRODUCTION
This project outlines the design and implementation of the network for shopping mall office a three-floor establishment with various departments. The goal is to create a robust, secure, and efficient network that facilitates communication between all devices and departments.
2. NETWORK DESIGN OVERVIEW
•	Floors and Departments:
o	1st Floor: Reception, Store, Logistics
o	2nd Floor: Finance, HR, Sales/Marketing
o	3rd Floor: IT, Admin
•	Network Infrastructure:
o	Three routers connecting each floor.
o	One switch per floor.
o	WIFI networks for laptops and phones.
o	Printers in each department.
o	VLANs for department segmentation.

3. NETWORK CONFIGURATION DETAILS
3.1 Routers and Serial Connections
•	Routers: Three routers located in the server room (IT department).
Serial DCE Cable Connections:
o	Router connections with networks:
	10.10.10.0/30 (Router 1 to Router 2)
	10.10.10.4/30 (Router 2 to Router 3)
	10.10.10.8/30 (Router 3 to Router 1)
3.2 VLAN Configuration
1st Floor VLANs:
o	Reception: VLAN 80, Network 192.168.8.0/24
o	Store: VLAN 70, Network 192.168.7.0/24
o	Logistics: VLAN 60, Network 192.168.6.0/24
2nd Floor VLANs:
o	Finance: VLAN 50, Network 192.168.5.0/24
o	HR: VLAN 40, Network 192.168.4.0/24
o	Sales: VLAN 30, Network 192.168.3.0/24
3rd Floor VLANs:
o	Admin: VLAN 20, Network 192.168.2.0/24
o	IT: VLAN 10, Network 192.168.1.0/24
3.3 DHCP Configuration
•	Each router acts as a DHCP server for its respective VLANs, dynamically assigning IP addresses.
3.4 OSPF Routing Protocol
OSPF Configuration:
o	Enable OSPF on all routers to advertise routes.
o	Ensure all VLAN networks and serial connections are included in OSPF configuration.

4. IMPLEMENTATION STEPS
1.	Setup Hardware:
o	Install routers and switches.
o	Connect routers using serial DCE cables.
o	Connect switches to routers.
2.	Configure VLANs:
o	Assign VLANs to respective departments.
o	Configure trunk ports between switches and routers.
3.	Enable OSPF Routing:
o	Configure OSPF on all routers.
o	Advertise all necessary networks.
4.	Setup DHCP:
o	Configure DHCP pools on routers for each VLAN.
o	Set up user credentials.
5.	Testing and Verification:
o	Ensure all devices obtain IP addresses via DHCP.
o	Confirm inter-department communication.

6. CONCLUSION
The network design and implementation for shopping mall system ensures secure, efficient, and seamless communication between all departments and devices. By segmenting the network using VLANs and implementing robust security measures, the hotel's network infrastructure supports its operational needs effectively.





