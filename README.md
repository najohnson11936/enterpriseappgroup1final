# Vehi-cool Rentals

Have you ever wanted to go on a road trip with your friends? Have you ever decided to rent a car so you could all ride together? Vehi-cool Rentals can help you:

- Locate nearby car rentals
- Make a reservation for any available car
- Find an affordable car within your price range
- Provide car information such as model year and mileage.

Use our web application to find and make a reservation for your future car rental. Find the perfect car for you that is nearby. In quick simple steps, you will be all set, and your car rental will be ready!

# Storyboard

![Storyboard1](https://github.com/najohnson11936/enterpriseappgroup1final/assets/100445409/0ffbca06-fd13-45c9-8c51-247522527605)
![Storyboard2](https://github.com/najohnson11936/enterpriseappgroup1final/assets/100445409/25694c3b-18f4-4c9f-9351-789da654909a)
![Storyboard3](https://github.com/najohnson11936/enterpriseappgroup1final/assets/100445409/02afec06-2df8-4049-93d6-7e74ecb61809)
![Storyboard4](https://github.com/najohnson11936/enterpriseappgroup1final/assets/100445409/a49a6bf8-77c5-42d7-ac13-003c2dded56c)

# Functional Requirements

## Requirement 1: Search for available car rentals

### Scenarios:

- As a student going on a road trip with multiple friends, I want to be able to find available car rentals.

### Dependencies:

- Car rental companies have cars to rent.

### Assumptions:

- Car rental places are legit and safe.
- Car rentals are near the student's location within 30 miles.

### Examples:

1.1
- Given a car rental place is 25 miles from my location.
- When I input car rental places within 30 miles from my location in the search bar.
- Then I can find a car rental place that is 25 miles from my location.

1.2
- Given a Jeep Wrangler is available for rental.
- When I input "Jeep Wrangler" in the search bar.
- Then I can locate the nearby car rental with a Jeep Wrangler.

1.3
- Given a Honda Civic is available for rental.
- When I input "Honda Civic" in the search bar.
- Then I can locate the nearby car rental with a Honda Civic.

## Requirement 2: Make Reservations

### Scenarios:

- As a student looking for a car rental, once I find the car I would like to rent, I would like to make a reservation.

### Dependencies:

- Students meet car rental companies' reservation policy.

### Assumptions:

- Students are eligible to rent a car.
- Students have a driver's license.

### Examples:

2.1
- Given I find a Jeep Wrangler that I would like to rent.
- When I click "rent."
- Then the website will prompt if the Jeep Wrangler is available. If so, students can input their information, such as driver's license and credit card.

2.2
- Given I find a Honda Civic that I would like to rent.
- When I click "rent."
- Then the website will prompt if the Honda Civic is available. If so, students can input their information, such as driver's license and credit card.

2.3
- Given I find a Toyota Tacoma that I would like to rent.
- When I click "rent."
- Then the website will prompt if the Toyota Tacoma is available. If so, students can input their information, such as driver's license and credit card.

# Class Diagram

![Vehi-cool Rentals UML Class Diagram](https://lucid.app/publicSegments/view/97e68e8c-2411-415a-a38f-9796cd2a8031/image.png)

## Class Diagram Description
- The class diagram consists of the following classes:
    - `Car.java`: Represents a car available for rental, with attributes such as make, model, and year.
    - `Customer.java`: Represents a customer who can rent cars, with attributes like name, email, and contact number.
    - `Rental.java`: Represents a rental transaction, with attributes such as rental ID, rental dates, and associated car and customer.
    - `Payment.java`: Represents a payment made for a rental, with attributes like payment ID, amount, and payment status.
    - `RentalService.java`: Interface for managing car-rental-related operations, such as creating rentals, calculating rental charges, and processing payments.
    - `CarService.java`: Interface for managing renting-related operations, such as checking car availability, making reservations, and canceling bookings.
    - `PaymentService.java`: Interface for managing payment-related operations, such as processing payments, generating payment receipts, and handling refunds.
    - `RentalServiceImpl.java`: Interface for accessing and manipulating rental data in the persistence layer.
    - `CarServiceImpl.java`: Interface for accessing and manipulating car data in the persistence layer.
    - `CustomerServiceImpl.java`: Interface for accessing and manipulating customer data in the persistence layer.
- The classes in the diagram have relationships as follows:
    - `Rental.java` has a one-to-one association with `Car.java`, indicating that a rental is associated with a specific car.
    - `Rental.java` has a one-to-one association with `Customer.java`, indicating that a rental is associated with a specific customer.
    - `Rental.java` has a one-to-one association with `Payment.java`, indicating that a rental is associated with a specific payment.
    - The business layer interfaces (`RentalService.java`, `CarService.java`, `PaymentService.java`, and `Customer Service.java`) depend on the persistence layer interfaces (`RentalServiceImpl.java`, `CarServiceImpl.java`, `RentalServiceImpl.java, and CustomerServiceImpl.java`.).
    - The UI layer depends on the business layer interfaces (`RentalService.java`, `CarService.java`, `PaymentService.java`, and `CustomerServiceImpl.java`) for interaction and functionality.

# Product Backlog and Sprint Goals

[Backlog for Vehi-cool Rentals](https://enterprisegroup1.atlassian.net/jira/software/projects/G1FP/boards/1/backlog)

## Milestones and Tasks for Sprint #1

Milestones:
- UI Expansion and Unit Test Implementation
- Interface and Stub/Mock Development
- Integration of Interfaces and Stubs
- Actual Implementation and Unit Testing
- Backend-UI Coordination and JSON Output
- Logic Organization and Package Refactoring
- Completion of Unit Tests

Tasks:
- UI Expansion and Unit Test Implementation
  - Research and gather requirements for UI enhancements
  - Create wireframes and design prototypes for UI improvements
  - Implement UI enhancements based on wireframes and design prototypes
  - Write unit tests for each non-UI class

- Interface and Stub/Mock Development
  - Identify the components requiring interfaces
  - Design and define interfaces for the identified components
  - Document the interfaces and their specifications
  - Determine the components that require stub/mock classes
  - Design and implement stub/mock classes based on the defined interfaces
  - Document the stub/mock classes and their purpose

- Integration of Interfaces and Stubs
  - Collaborate with team members to exchange interfaces and stubs
  - Integrate received interfaces and stubs into the project

- Actual Implementation and Unit Testing
  - Review the interfaces and stubs to understand the requirements
  - Develop implementation classes that fulfill the interface specifications
  - Test the implementation classes for functionality and integration

- Backend-UI Coordination and JSON Output
  - Identify the necessary communication points between backend and UI
  - Implement event listeners and handlers to enable communication
  - Integrate JSON output formatting for appropriate data exchange

- Logic Organization and Package Refactoring
  - Analyze the existing codebase and determine appropriate package structure
  - Refactor the codebase to organize backend, business, and persistence logic into separate packages

- Completion of Unit Tests
  - Write unit tests using Behavior Driven Design syntax for each identified class

Tasked Stories for Sprint #1:
- [Expand UI](https://enterprisegroup1.atlassian.net/jira/software/projects/G1FP/boards/1/backlog?selectedIssue=G1FP-1)
- [Create Interfaces for Business Logic and Persistence](https://enterprisegroup1.atlassian.net/jira/software/projects/G1FP/boards/1/backlog?selectedIssue=G1FP-2)
- [Create Stub/Mock Classes](https://enterprisegroup1.atlassian.net/jira/software/projects/G1FP/boards/1/backlog?selectedIssue=G1FP-3)
- [Swap Interfaces and Stubs with Team Members](https://enterprisegroup1.atlassian.net/jira/software/projects/G1FP/boards/1/backlog?selectedIssue=G1FP-4)
- [Program Actual Implementation Classes](https://enterprisegroup1.atlassian.net/jira/software/projects/G1FP/boards/1/backlog?selectedIssue=G1FP-5)
- [Coordinate Listening from Backend to UI](https://enterprisegroup1.atlassian.net/jira/software/projects/G1FP/boards/1/backlog?selectedIssue=G1FP-6)
- [Consider JSON Output](https://enterprisegroup1.atlassian.net/jira/software/projects/G1FP/boards/1/backlog?selectedIssue=G1FP-7)
- [Organize Backend, Business, and Persistence Logic](https://enterprisegroup1.atlassian.net/jira/software/projects/G1FP/boards/1/backlog?selectedIssue=G1FP-8)
- [Write Unit Tests](https://enterprisegroup1.atlassian.net/jira/software/projects/G1FP/boards/1/backlog?selectedIssue=G1FP-9)

Scrum Roles:
- Scrum Master & Product Owner: Nick Johnson
- Business Layer/Backend: Levi Huff
- UI/Frontend: Jake Plagge, Wilmer Esquivel

# Weekly team meetings
The Vehi-cool Rentals team gets together every Tuesday @ 8pm EST on Discord
