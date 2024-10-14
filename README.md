# Automation System Re-Design (Framing Machine & Tables)

Client: OZ BUILD CONSTRUCTIONS

# Introduction:

The current setup at OZ BUILD CONSTRUCTIONS' framing machine and panel tables station is fully automated and controlled by a centralized Beckhoff PLC system. This system is responsible for coordinating operations across multiple stations, including:

Framing Station: Two nailing stations for automated framing processes.
Panel Tables: Six tables for processing wall and floor panels.
The system consists of two main electrical cabinets, connected via EtherCAT for communication. The entire process is controlled by a central Beckhoff PLC, which receives signals from a Human-Machine Interface (HMI). Each panel has its own I/O modules, safety modules, and power supplies to ensure smooth operations.

Currently, the system operates on outdated TwinCAT 2 software for PLC programming and HMI development, making maintenance and future scalability difficult. Communication between the PLC, I/O modules, and the HMI is facilitated by EtherCAT, a high-performance fieldbus protocol.

Project Objectives:
Decentralize Control: Separate the control systems of different stations, simplifying the management of the production line:

Wall framing stations
Wall station tables
Floor station tables
Upgrade to TwinCAT 3: Re-develop the existing PLC program using the latest TwinCAT 3 software to enhance system performance, scalability, and maintainability.

HMI Software Re-Development: Develop a new HMI software interface that is modern, user-friendly, and integrated with the upgraded TwinCAT 3-based PLC system.

Version Control & Collaboration: Implement the entire project on GitHub to ensure proper version control, documentation, and collaboration.

System Architecture:
Main PLC: Beckhoff PLC controlling system operations.
Communication Protocol: EtherCAT protocol between I/O modules, PLC, and HMI.
I/O Modules: Distributed I/O for various sensors, actuators, and safety systems.
HMI: Centralized HMI controlling and monitoring the entire system.
Steps Involved:
PLC Separation: Divide the control of different production stations (wall framing, wall station tables, and floor station tables) into separate PLCs for easier control and troubleshooting.

Program Migration to TwinCAT 3:

Analyze and migrate the existing PLC program from TwinCAT 2 to TwinCAT 3.
Optimize code structure to support decentralized control.
Integrate communication between separate PLCs using EtherCAT.
HMI Software Development:

Develop a new HMI interface with modern UI/UX using TwinCAT 3.
Ensure real-time data monitoring and control through intuitive graphics and navigation.
Testing & Commissioning:

Thorough testing of the decentralized PLC systems and the new HMI interface.
Ensure communication and data flow among all components is seamless.
Version Control with GitHub:

Use GitHub to store the PLC programs and HMI software for version control and collaborative development.
Keep the repository up-to-date with detailed documentation and changelogs.
