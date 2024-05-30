# lab-mandaroty09

## Tasks:
### Design Exercise:
  * **Application Brief:** Participants are given a description of a monolithic e-commerce application handling user management, product catalog, order processing, and customer support.
  * **Task:** Identify and outline potential microservices based on domain-driven design principles. Participants will determine service boundaries, define how services will communicate, and plan how to handle shared data.

### Monolithic E-Commerce Application Description:
The application is a traditional e-commerce platform that encompasses all functionalities within a single, unified software architecture. The application handles the following key operations:

  * **User Management:** Manages user profiles, authentication, and authorization. It stores personal information, manages login sessions, and handles user preferences.

  * **Product Catalog:** Maintains a comprehensive list of products, including descriptions, pricing, images, and inventory levels. It supports product search and categorization functionalities.

  * **Order Processing:** Manages all aspects of the ordering process, from cart management to order placement, payment processing, and order history tracking.

  * **Customer Support:** Handles customer inquiries, returns, complaints, and feedback through a ticket-based system integrated with the user and order databases.

The application is built on a single relational database that holds all user data, product information, orders, and customer support interactions. It currently operates on a single code base with a web-based frontend that communicates directly with the backend server.

The platform has been experiencing challenges with scaling during high-traffic periods, frequent downtimes during updates, and increasing difficulty in implementing new features without affecting existing functionalities. The goal is to decompose this monolithic architecture into a microservices-based architecture to address these issues and improve overall agility and scalability.

# Implementation Simulation:
  * **Migration Roadmap:** Develop a detailed plan for migrating the identified monolithic components to microservices. This plan should include prioritization of services to be migrated, identification of dependencies, and a strategy for data migration.
  * **Architecture Documentation:** Document the proposed microservices architecture, illustrating the interaction between services and the migration steps. Include a brief narrative explaining the rationale behind key decisions.

# Simulation

  * **Roadmap:** Under the given monolith definition, we can identify 5 microservices **User Management, Products, Orders, Customer Support, Security** each of them with their own database and domain. Orders has the greatest dependency between microservices by requiring users, products.

To begin the migration, it is proposed to start with Users, then Products and Orders, and finally add Customer Support.

* **Documentation:**
![image](https://github.com/LuisGutierrezRdz/lab-mandaroty09/assets/115661340/c1e1a4c4-c286-44d1-a14c-2938b7fbcd13)



