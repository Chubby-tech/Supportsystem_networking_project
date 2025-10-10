# Supportsystem_networking_project
This is a trading floor support system networking project


A trading floor Support centre employs 600 staff. They have recently expanded and as a result,
need to move to a new building. A building has been identified but has no network.
This means that before they can make to move out, new network service needs to be designed and implemented in the new building.
Existing Network comprises of the following elements:
The new building is expected to have three floors with two departments in each for example;
 
1. First floor (Sales and Marketing Department-25users expected. Human Resource and Logistics Department-25 users expected)
2. Second floor (Finance and Accounts Department-25 users expected. Administrator and Public Relations Department-25 users expected)
3. Third floor (IT-25 users expected, Server Room-25 devices expected)
 
Therefore, as a key member of the Networks Team, you have been tasked to design a network for the new building.
At this stage, logical design is required, which shows the measures that you would put in place to ensure
that the new network meets the current business need and is future-proofed.
 
Requirements
1. Use Cisco Packet Tracer to design and implement the network solution.
2. Use hieratical model providing redundancy at every layer ie. two routers and two multilayer switches are expected to be used to provide redundancy.
3. The network is also expected to connect to at least two ISPs to provide redundancy and each router to be connected to the two ISPs.
4. Each department is required to have a wireless network for the users
5. Each department should be in a different VLAN and in different subnetwork.
6. Provided a base network of 172.16.1.0, carry out subnetting to allocate the correct number of IP addresses to each department.
Organize Pag
7. The company network is connected to the static, public IP addresses (Internet Protocol) 195.136.17.0/30, 195.136.17.4/30, 195.136.17.8/30 and 195.136.17.12/30 connected to the two Internet providers.
8. Configure basic device settings such as hostnames, console password, enable password. banner messages, disable IP domain lookup.
9. Devices in all the departments are required to communicate with each other with the respective multilayer switch configured for inter-VLAN routing.
10. The Multilayer switches are expected to carry out both routing and switching functionalities thus will be assigned IP addresses.
11. All devices in the network are expected to obtain an IP address dynamically from
the dedicated DHCP servers located at the server room.
12. Devices in the server room are to be allocated IP address statically.
13. Use OSPF as the routing protocol to advertise routes both on the routers and multilayer switches.
14. Configure SSH in all the routers and layer three switches for remote login.
15. Configure port-security for the Finance and Accounts department to allow only one device to connect to a switchport, use sticky method to obtain mac-address and violation mode shutdown.
16. Configure NAT to use the respective outbound router interface IPv4 address, implement the necessary ACL rule.
17. Test Communication, ensure everything configured is working as expected.
 
 
 
 
