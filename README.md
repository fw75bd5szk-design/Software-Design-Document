# Software-Design-Document

# CS 230 Portfolio: Draw It or Lose It

## About the Project

The Gaming Room was the client for this project. The company already had an Android game called *Draw It or Lose It* and wanted to expand it into a web-based application that could be used on multiple operating systems and devices. The new system needed to support multiple teams and players, keep game, team, and player names unique, and maintain consistent game data for every connected user. It also needed to be reliable, secure, and able to support more users as the game grew.

## What I Did Well

I think I did particularly well in the evaluation and recommendations portions of the software design document. I compared macOS, Linux, Windows, and mobile devices from the server, client, and development perspectives instead of assuming that one platform would work equally well for every purpose. Based on reliability, scalability, compatibility, and cost, I recommended Linux for the server while allowing users to access the game through web browsers on Windows, macOS, Android, and iOS. I also explained how the singleton and iterator design patterns would support one `GameService` instance and prevent duplicate names.

## How the Design Document Helped

Working through the design document helped me organize the client’s requirements before focusing on implementation. Breaking the project into requirements, constraints, the domain model, platform evaluations, and recommendations made the relationships between the different parts of the system easier to understand. This would make developing the code more efficient because the major classes, responsibilities, design patterns, and technical decisions are identified before the system is built. It would also give the development team a shared reference during implementation and testing.

## What I Would Revise

If I could revise one section, I would add more detail to the system architecture view. I would include a diagram showing how the browser clients, Linux web server, Java application, and MySQL database communicate with one another. I would also identify where authentication, HTTPS connections, backups, and monitoring fit into the architecture. This would make the recommended distributed client-server design easier for another developer to understand and implement.

## Interpreting the User’s Needs

I interpreted the users’ needs by separating the client’s business goals from the system’s technical requirements. The Gaming Room wanted to reach more players, but the software also had to enforce unique names, support multiple teams and players, synchronize game data, and perform consistently across different devices. I used these needs to recommend a web-based client-server system with responsive design and centralized data management.

Considering users’ needs is important because a technically functional application can still fail if it does not solve the client’s actual problem or provide a good experience for the people using it.

## My Software Design Approach

My approach to software design is to begin by identifying the users, business goals, functional requirements, nonfunctional requirements, and design constraints. I then use models and diagrams to define the system’s classes, relationships, and flow of information before comparing possible technologies.

In future projects, I would continue using this process while adding prototypes, user stories, security reviews, and feedback checkpoints earlier in the design phase. These techniques would help reveal missing requirements sooner and reduce the amount of rework needed during development.
