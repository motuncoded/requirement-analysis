# Requirement Analysis in Software Development.
Requirement Analysis is a critical phase in the software development lifecycle (SDLC) where the project team gathers, analyzes, and defines the requirements of the software product to be developed.

## Introduction
The purpose of this respository is to focus on crafting a comprehensive foundation for software development by documenting, analyzing, and structuring requirements. 

## What is Requirement Analysis ?

Requirement Analysis is a critical phase in the software development lifecycle (SDLC) where the project team gathers, analyzes, and defines the requirements of the software product to be developed. This process ensures that all stakeholders have a clear and mutual understanding of what the system should do and how it should perform.

## Why is Requirement Analysis Important?

![requirement drawio](https://github.com/user-attachments/assets/0c10091a-1e1f-468d-9e52-035f061ec7cc)


- **Clarity and Understanding**: It helps in understanding what the stakeholders expect from the software, reducing ambiguity.
- **Scope Definition**: Clearly defines the scope of the project, which helps in preventing scope creep.
- **Basis for Design and Development**: Provides a solid foundation for designing and developing the system.
- **Cost and Time Estimation**: Facilitates accurate estimation of project cost, resources, and time.
- **Quality Assurance**: Ensures that the final product meets the specified requirements, leading to higher customer satisfaction.

## Key Activities in Requirement Analysis.

### 1. Requirement Gathering 🗂️

- Interviews: Conducting interviews with stakeholders to gather detailed information about their needs and expectations.
- Surveys/Questionnaires: Distributing surveys to collect requirements from a larger audience.
- Workshops: Organizing workshops with stakeholders to discuss and gather requirements.
- Observation: Observing end-users in their working environment to understand their needs.
- Document Analysis: Reviewing existing documentation and systems to understand current functionalities and requirements.
  
### 2. Requirement Elicitation ✍️
- Brainstorming: Conducting brainstorming sessions to generate ideas and gather requirements.
- Focus Groups: Holding focus group discussions with selected stakeholders to gather detailed requirements.
- Prototyping: Creating prototypes to help stakeholders visualize the system and refine their requirements.
  
### 3. Requirement Documentation 📚
- Requirement Specification Document: Creating a detailed document that lists all functional and non-functional requirements.
- User Stories: Writing user stories to describe functionalities from the user’s perspective.
- Use Cases: Creating use case diagrams to show interactions between users and the system. 

### 4. Requirement Analysis and Modeling 📊
- Requirement Prioritization: Prioritizing requirements based on their importance and impact on the project.
- Feasibility Analysis: Assessing the feasibility of requirements in terms of technical, financial, and time constraints.
- Modeling: Creating models (e.g., data flow diagrams, entity-relationship diagrams) to visualize and analyze requirements.

### 5. Requirement Validation ✅
- Review and Approval: Reviewing the documented requirements with stakeholders to ensure accuracy and completeness.
- Acceptance Criteria: Defining clear acceptance criteria for each requirement to ensure they meet the expected standards.
- Traceability: Establishing traceability matrices to ensure all requirements are addressed during development and testing.

## Types of Requirements
### Functional Requirements ⚙️

- **Definition**: Describe what the system should do.
- **Examples**: User authentication, property search, booking system, user registration.

#### Key Functional Requirements:

- **Search Properties**: Users should be able to search for properties based on various criteria such as location, price, and availability.
- **User Registration**: New users should be able to create an account with personal details and login credentials.
- **Property Listings**: Display properties with essential details and images.
- **Booking System**: Users should be able to book properties, view booking details, and manage their bookings.
- **User Authentication**: Secure login and registration process for users.


###  Non-functional Requirements 🛡️
- **Definition**: Describe how the system should perform.
- **Examples**: Performance, security, scalability, usability, reliability.

#### Key Non-functional Requirements:

- **Performance**: The system should load pages within 2 seconds and handle up to 1000 concurrent users.
- **Security**: Ensure data encryption, secure login, and protect against common vulnerabilities.
- **Scalability**: The system should be able to scale horizontally to handle increased traffic.
- **Usability**: The application should have an intuitive UI/UX, making it easy for users to navigate and perform tasks.
- **Reliability**: The system should have an uptime of 99.9% and recover quickly from any failures.


## Use Case Diagrams 📊
Objective: Visual representation of interactions between users and the system.

### What are Use Case Diagrams?

Use case diagrams show how different users (actors) interact with the system to achieve specific goals (use cases).
Creating Use Case Diagrams:

- Identify actors (e.g., guest, registered user, admin).
- Define use cases (e.g., search properties, book property, manage listings).
- Draw interactions between actors and use cases.

  
### Benefits of Use Case Diagrams:

- Provide a clear visual representation of system functionalities.
- Help in identifying and organizing system requirements.
- Facilitate communication among stakeholders and development team.

![alx-booking-uc](https://github.com/user-attachments/assets/041998a4-168b-4acb-a6af-969f89e33b2a)

## Acceptance Criteria

Objective: Establishing clear criteria for feature completion.

### What is Acceptance Criteria?

Acceptance criteria are conditions that a feature must meet to be accepted by the stakeholders.

### How to Define Acceptance Criteria:

- Be specific and measurable.
- Include functional and non-functional aspects.
  

### Benefits of Acceptance Criteria:

- Ensure all parties have a clear understanding of feature requirements.
- Provide a basis for testing and validation.
- Help in maintaining quality and meeting user expectations.


#### ✅ **Feature: Checkout**

##### **User Story**

*As a registered user, I want to securely complete a booking and make a payment so that I can confirm my stay at a selected property.*

##### **Acceptance Criteria**

1. **Property and Date Validation**

   * Given a user selects a property and date range,
     When they proceed to checkout,
     Then the system must verify the property is still available for the selected dates.

2. **User Authentication**

   * Given a user is not logged in,
     When they attempt to access the checkout page,
     Then they are redirected to the login page.

3. **Pricing Summary**

   * Given a user is on the checkout page,
     When the page loads,
     Then the system should display the full booking summary, including:

     * Property name
     * Stay duration
     * Base price
     * Taxes/fees
     * Total amount due

4. **Payment Information Input**

   * Given a user is on the checkout page,
     When they enter payment details,
     Then the form must validate card number, expiration, and CVV.

5. **Successful Payment**

   * Given a user submits valid payment details,
     When the payment is processed successfully,
     Then:

     * A booking confirmation is displayed
     * A confirmation email is sent
     * The property’s availability is updated

6. **Failed Payment**

   * Given a user submits invalid or declined payment details,
     When the payment fails,
     Then an error message is displayed, and the user is prompted to try again.

7. **Cancellation Option**

   * Given a booking is completed,
     When the user views their booking details,
     Then a "Cancel Booking" button is shown (based on cancellation policy).



