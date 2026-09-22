# Home-Network-Simulation-Lab-Cisco-Packet-Tracer-Wireless-Router-Access-Point-
Small Cisco Packet Tracer lab where I built a home style network from scratch, a wireless router as the hub, wired server and PCs, a couple of wireless laptops, and a standalone access point extending coverage to a remote client. Focused on getting the physical and wireless layout right before moving on to addressing and configuration.

Home Network Simulation Lab (Cisco Packet Tracer, Wireless Router, Access Point, Mixed Wired and Wireless Clients)

Tools used: Cisco Packet Tracer, HomeRouter PT AC (wireless router), AccessPoint PT, Server PT, PC PT, Laptop PT

Overview
This lab was built in Cisco Packet Tracer to practice designing a small home or small office style network from scratch rather than just working inside a network someone else already configured. The topology mixes wired and wireless connections off a single wireless router, plus a separate access point out at the edge of the network to extend wireless coverage to a client sitting further away. The goal was to get comfortable placing devices, wiring them up correctly, and thinking through which devices should be wired versus wireless in a mixed environment.

Objective
Build a small network with a central wireless router acting as the core device, attach a mix of wired PCs, a server, and both wired and wireless laptops, then extend the network out to a remote client using a standalone access point. This is meant to mirror a realistic small network layout where not everything can reasonably run a cable back to the router.

Environment
Central device: HomeRouter PT AC, labeled Wireless Router0
Server: Server PT, labeled Server0, wired directly into the router
Wired PC: PC PT, labeled Admin, wired directly into the router
Wired PC: PC PT, labeled Staff, wired directly into the router
Wireless laptop: Laptop PT, labeled Laptop2, connecting to the router over a wireless link
Wireless laptop: Laptop PT, labeled Laptop1, placed near the router
Edge device: AccessPoint PT, labeled Access Point0, wired back to the router over a long run
Remote wireless client: Laptop PT, labeled Laptop3, connecting wirelessly through Access Point0 rather than the main router
Platform: Cisco Packet Tracer, Logical workspace view

What I Did

Laying Out the Core
I started with the HomeRouter PT AC in the center of the workspace since everything else in this topology hangs off of it, either by a direct wired connection or over its built in wireless radio. This felt closer to how a real home or small office network is usually drawn, one router in the middle acting as the hub for everything else.

Wiring the Server and Admin Devices
I connected Server0 directly into the router with a straight cable, along with the Admin and Staff PCs. Keeping these wired rather than wireless made sense here since they represent devices that are expected to stay in one place and benefit from a stable, faster connection rather than sharing wireless bandwidth.

Adding Wireless Clients
Laptop2 connects to the router over wireless rather than a physical cable, shown by the dashed line instead of a solid one in Packet Tracer. This represents a device that needs to move around or simply does not have a wired drop nearby, which is a normal part of most real networks now.

Extending Range With an Access Point
The most interesting part of this build was placing Access Point0 out at a distance from the router and running a long wired backhaul connection to it. Laptop3 then connects wirelessly to that access point instead of talking directly to the router. This is meant to simulate a real world situation where a single wireless router does not have enough range to cover an entire building or property, so a second access point gets wired back to the main router to extend coverage further out.

Working Through Packet Tracer Itself
A good chunk of this exercise was just getting comfortable inside the Packet Tracer interface, dragging devices from the device shelf at the bottom, drawing connections between them, and switching between the Logical and Physical views to understand how the software represents a network versus how it would actually sit in a physical space.

What I Would Add Next
Assign static IP addressing to each device and document the addressing scheme
Configure the wireless router's SSID and security settings instead of leaving defaults
Test end to end connectivity between devices using ping and simple ping troubleshooting
Add a second router or switch to practice a slightly larger, segmented topology
Look into why Laptop1 was placed but not yet connected in this version, and either wire it up or connect it wirelessly with a clear reason for the choice

Where I Am Coming From
I am moving into cybersecurity from a background in healthcare, so a lot of my early hands on practice, including labs like this one, is about building the fundamentals from the ground up. Networking basics like this one matter because you cannot secure or analyze a network you do not understand the shape of first. Before worrying about attacking or defending anything, I wanted to get comfortable just building a small, realistic network layout by hand.

Limitations
This lab only covers physical and wireless layout, no IP addressing, routing, or security configuration was done yet
No connectivity testing was performed between devices in this version
Laptop1 appears placed in the topology without a confirmed connection, which would need to be resolved in a follow up version

References
Cisco Packet Tracer documentation, available through the Cisco Networking Academy
