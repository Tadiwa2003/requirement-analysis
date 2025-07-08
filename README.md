# requirements_analysis in Software Development 

What is Requirement Analysis ?
Requirement Analysis: Brief Overview
Requirement Analysis is the crucial phase in the Software Development Lifecycle (SDLC) where the needs and expectations for a software system are clearly identified, understood, and documented.

What it is:
It's the process of defining what the software must do and what characteristics it must have, bridging the gap between business needs and technical implementation.

Key Activities:
Elicitation: Gathering needs from stakeholders.

Analysis: Examining needs for clarity, consistency, and feasibility.

Specification: Documenting the agreed-upon requirements (e.g., in an SRS).

Validation: Confirming requirements meet stakeholder needs.

Management: Handling changes to requirements throughout the project.

Importance in SDLC:
Foundation: Provides the blueprint for all subsequent phases (design, development, testing).

Risk Mitigation: Reduces costly rework, prevents scope creep, and lowers the risk of project failure by catching issues early.

Alignment: Ensures everyone involved has a shared understanding of the project's goals.

Why is Requirement Analysis important ?

Key Reasons Why Requirement Analysis is Critical in SDLC
Provides a Solid Foundation (Blueprint for Development):

Requirement Analysis serves as the essential blueprint for all subsequent SDLC phases. Clear, well-defined requirements guide the design team in creating the system architecture, inform developers on what code to write, and provide testers with the criteria to validate the software. Without this foundation, development can become aimless, leading to a product that doesn't meet its intended purpose.

Mitigates Risks and Reduces Costs:

Identifying and correcting errors or misunderstandings during the requirements phase is significantly cheaper than fixing them later in the development cycle (e.g., during coding or testing). Thorough analysis helps prevent "scope creep" (uncontrolled expansion of project requirements) and reduces the likelihood of costly rework, project delays, or even outright project failure.

Ensures Stakeholder Alignment and Effective Communication:

This phase forces all stakeholders—from clients and end-users to developers and project managers—to articulate and agree upon a shared vision for the software. It establishes a common understanding of what needs to be built, fostering better communication and collaboration throughout the project and minimizing misinterpretations that can lead to dissatisfaction.

Quality: Leads to a higher quality product that truly meets user needs.

In essence, it's about building the right product by thoroughly understanding what needs to be built before starting development.

[Key activities in the Requirements Analysis] 

The Requirement Analysis phase is a comprehensive process that involves several interconnected activities to ensure a thorough understanding of stakeholder needs. While terminology can sometimes overlap, here are five distinct and crucial activities:

1. Requirement Elicitation (often referred to as Requirement Gathering)
Description: This is the initial and most active part of collecting requirements. It involves drawing out, discovering, and extracting needs from various sources. It's not just about passively receiving information, but actively engaging with stakeholders to uncover both explicit and implicit requirements.

Purpose: To identify all relevant needs, expectations, constraints, and features that the new or modified software system must address.

Techniques: Interviews, workshops (e.g., JAD sessions), brainstorming, surveys, questionnaires, observation of existing processes, prototyping, use case analysis, and analyzing existing documentation.

2. Requirement Analysis and Modeling
Description: Once requirements are elicited, they need to be thoroughly examined, refined, and structured. This activity involves scrutinizing the gathered requirements for consistency, completeness, feasibility, clarity, and ambiguity. Modeling then involves creating visual or structured representations of these requirements.

Purpose: To resolve conflicts, identify gaps, eliminate redundancies, prioritize needs, and translate abstract ideas into a more precise and understandable form for technical teams. Modeling helps visualize relationships and system behavior.

Techniques: Creating Data Flow Diagrams (DFDs), Use Case Diagrams, Entity-Relationship Diagrams (ERDs), process flowcharts, state diagrams, data dictionaries, and performing feasibility studies.

3. Requirement Documentation
Description: This activity involves formally recording and organizing the analyzed and agreed-upon requirements. It's about creating a single, authoritative source of truth for the project's requirements.

Purpose: To provide a clear, unambiguous, and verifiable record of what the system is supposed to do. This document serves as a reference for all project stakeholders throughout the SDLC, facilitating communication and ensuring everyone is working towards the same goals.

Outputs: A Software Requirements Specification (SRS) document, user stories, use case specifications, a requirements traceability matrix, or a product backlog (in agile methodologies).

4. Requirement Validation
Description: This is the process of reviewing and verifying the documented requirements with stakeholders to ensure they accurately reflect their actual needs and that the proposed system will meet the overall business objectives. It's about confirming that the right requirements have been captured.

Purpose: To catch errors, omissions, misunderstandings, and inconsistencies early in the lifecycle, before they become expensive to fix in later development stages. It also ensures stakeholder buy-in and agreement.

Techniques: Requirement reviews, walkthroughs, inspections, prototyping (to get early feedback), and developing acceptance criteria.

5. Requirement Management
Description: Requirements are rarely static; they often change throughout a project due to evolving business needs, new insights, or external factors. Requirement Management is the ongoing process of tracking, controlling, and communicating these changes.

Purpose: To ensure that changes to requirements are handled systematically, their impact is assessed, and all affected stakeholders are informed. This prevents "scope creep" and maintains consistency between the requirements and the evolving software product.

Techniques: Using a requirements traceability matrix, version control for requirement documents, change control boards, and dedicated requirements management tools.

These five activities work in concert to build a robust and reliable foundation for successful software development.

[Differentiate between functional and non-functional requirements] 
[Types of requirements ]

Functional and Non-functional Requirements for a Booking Management Project
In the context of the provided hotel booking app case study, understanding the system's requirements is crucial. Requirements specify what the system does (functional) and how well it does it (non-functional).

Functional Requirements
Definition: Functional requirements define the specific actions or behaviors that a system must perform. They describe the features and services that the users expect from the software.

Examples from the Case Study:

Hotel Information Management:

Description: The system shall allow hotel managers/owners to create, update, and delete hotel-related information, including hotel details (e.g., name, address, contact), room types, pricing, and availability.

Case Study Link: "This is the service that will be given to hotel managers/owners. In this managers can manage their hotel's related information. Here managers have a separate portal to access the data and update it."

Customer Search and Filtering:

Description: The system shall enable customers to search for hotels based on various criteria such as location, check-in/check-out dates, number of guests, price range, and amenities.

Case Study Link: "This is the service that will be given to customers. In this customers can search and book a hotel." and "The search service has to get the data from Elastic Search."

Booking and Payment Processing:

Description: The system shall allow customers to select available rooms, initiate a booking, and securely process payments through an integrated third-party payment service.

Case Study Link: "a booking service to book the hotel and booking service also interacts with the payment service which will be a third-party service."

Booking History Viewing:

Description: The system shall provide functionalities for both customers and hotel managers to view their current and historical booking details.

Case Study Link: "Here all current and old booking details are shown to the user. Both managers and customers use this service."

Non-functional Requirements
Definition: Non-functional requirements (NFRs) specify criteria that can be used to judge the operation of a system, rather than specific behaviors. They define the quality attributes of the system.

Examples from the Case Study:

Performance (Response Time & Throughput):

Description: The system shall process a high amount of user traffic smoothly, ensuring fast delivery of content (via CDN) and reduced API response times for customer searches and booking operations (leveraging caching like Redis).

Case Study Link: "These are so huge that they have a high amount of user traffic that needs to be processed." "A CDN is a geographically distributed group of servers that work together to provide fast delivery of Internet content." "Redis is caching system... which could eventually reduce the load in the database also reduce the response time of API."

Scalability:

Description: The system shall be highly scalable to manage a continuously increasing volume of users and data, achieved through a micro-service architecture, load balancing, and distributed databases (e.g., master-slave DBs, Cassandra for archival).

Case Study Link: "to manage these we have to follow micro-service architecture. This means we have to divide the system into small chunks for each type of task." "Hotel DB cluster which follows the master-slave architecture to reduce the load in the database." "with time data size will increase in the database... Casandra is a NoSQL database that is good at handling a high volume of data."

Reliability & Data Durability:

Description: The system shall operate "without a single glitch," ensuring high availability of data and services, with data automatically replicated and archived to prevent loss and maintain consistency.

Case Study Link: "all without a single glitch!" "Hotel DB cluster which follows the master-slave architecture to reduce the load in the database. Master DB is used for a write operation and slave DB is used for reading operation only. Whenever a write operation is performed on the master database it syncs the data to the slave database." "For archival we are using Casandra because with time data size will increase in the database, increasing query time. So that’s why we may need to delete old data from the database."

Usability:

Description: The system shall provide a smooth and intuitive flow for users, from hotel listing to booking and payments, with separate, easy-to-access portals for customers and managers.

Case Study Link: "provide such a smooth flow, from hotel listing to booking, to payments." "Here managers have a separate portal to access the data and update it." "Here customers have a separate portal to access the data and process it."

[Acceptence Criteria]

Importance of Acceptance Criteria in Requirement Analysis
Acceptance Criteria are a set of predefined conditions that a software system or feature must satisfy to be accepted by a user, customer, or other stakeholders. They are typically written from the user's perspective and define the "conditions of satisfaction" for a given requirement or user story.

Why Acceptance Criteria are Critical in Requirement Analysis:
Defines "Done": Acceptance criteria provide a clear, unambiguous definition of when a requirement or feature is considered complete and successfully implemented. This eliminates guesswork and ensures that development teams know exactly what they need to deliver.

Reduces Ambiguity and Misinterpretation: By specifying concrete, testable conditions, acceptance criteria clarify vague requirements. They force stakeholders and development teams to think through the exact behavior and outcomes expected, preventing costly misunderstandings and rework later in the SDLC.

Basis for Testing: Acceptance criteria directly translate into test cases. Testers use these criteria to design and execute tests, ensuring that the developed functionality meets the agreed-upon conditions. If all acceptance criteria for a feature pass, it indicates the feature is ready for release.

Facilitates Validation and Stakeholder Alignment: They serve as a common understanding between the business (what they want) and the development team (what they will build). During requirement validation, stakeholders can easily confirm if the documented criteria truly reflect their needs, leading to earlier feedback and stronger buy-in.

Supports User-Centric Development: By being written from a user's perspective (e.g., "As a user, I can..."), acceptance criteria keep the focus on delivering value to the end-user and ensuring the system meets their real-world needs.

In essence, Acceptance Criteria bridge the gap between abstract requirements and concrete, verifiable functionality, making the entire development process more efficient, transparent, and successful.

Example of Acceptance Criteria for a "Checkout" Feature in a Booking Management System
Let's consider a functional requirement for a hotel booking system:

Functional Requirement / User Story:
"As a customer, I want to be able to complete my booking and make a payment so that my room reservation is confirmed."

Acceptance Criteria for the "Checkout" Feature:

Scenario 1: Successful Payment with Valid Details

Given a customer has selected a room and proceeds to checkout.

And the customer provides valid payment method details (e.g., credit card number, expiry date, CVV).

And the payment gateway successfully processes the transaction.

When the customer clicks "Confirm Booking."

Then the system shall display a "Booking Confirmed" message.

And the customer shall receive a confirmation email with booking details.

And the hotel manager shall receive a notification of the new booking.

And the room's availability for the booked dates shall be updated in the system.

Scenario 2: Payment Failure due to Invalid Details

Given a customer is on the checkout page.

And the customer provides invalid payment method details (e.g., incorrect CVV, expired card).

When the customer clicks "Confirm Booking."

Then the system shall display an error message indicating payment failure (e.g., "Invalid card details. Please try again.").

And the booking shall not be confirmed.

And the room's availability shall remain unchanged.

Scenario 3: Payment Gateway Timeout/Error

Given a customer is attempting to make a payment.

And the payment gateway experiences a timeout or returns a generic error.

When the system attempts to process the payment.

Then the system shall display a message indicating a temporary issue (e.g., "Payment service is currently unavailable. Please try again later.").

And the booking shall not be confirmed.

And the room's availability shall remain unchanged.

Scenario 4: Customer Navigates Away During Checkout

Given a customer has entered some details on the checkout page but has not confirmed the booking.

When the customer navigates away from the checkout page (e.g., closes tab, clicks back button).

Then the system shall not confirm the booking.
