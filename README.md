# Project README

## Overview

This project is a Spring Boot application with a PostgreSQL database integration. It also includes a frontend that interacts with the backend API to manage Cognitive Behavioral Therapy (CBT) records.

### Backend: Spring Boot and PostgreSQL

- **DatabaseConfig.java**: Configures the HikariCP connection pool for database management.
- **DemoApplication.java**: The main entry point for the Spring Boot application.
- **CBTController.java**: Manages HTTP requests and responses for CBT-related operations.
- **CBT.java**: A model class representing the CBT entity.
- **CBTRepository.java**: Provides CRUD operations for the CBT entity.
- **CBTService.java**: Provides business logic for handling CBT operations.

### Frontend: React

- **App.js**: The main entry point for the frontend React application.
- **FAQ.js**: A component that provides users with a modal to display FAQs related to CBT.
- **HomePage.js**: Displays the main homepage, including adding new thoughts and displaying recently added ones.
- **ThoughtForm.js**: A form component for users to submit new CBT thoughts.
- **ThoughtPreview.js**: Displays previously added thoughts.

## Key Features

- **Backend API**:
  - Create and manage CBT records.
  - Integration with PostgreSQL using HikariCP for database connection pooling.
  - RESTful API endpoints for managing CBT entries.

- **Frontend Interface**:
  - A React-based user interface with forms to add new CBT thoughts.
  - FAQ section with expandable accordion items to provide more information about CBT.
  - Displays a list of recent CBT thoughts.
  
### How to Run

#### Prerequisites

- Java 11+
- Node.js
- PostgreSQL

#### Backend Setup

1. Clone the repository.
2. Navigate to the backend directory.
3. Update `application.properties` with your PostgreSQL credentials.
4. Run the application using the following command:

   ```bash
   ./mvnw spring-boot:run
   ```

#### Frontend Setup

1. Navigate to the `frontend` directory.
2. Install dependencies:

   ```bash
   npm install
   ```

3. Start the React application:

   ```bash
   npm start
   ```

### API Endpoints

- **GET** `/api/cbt`: Fetches all CBT records.
- **POST** `/api/cbt`: Creates a new CBT record.

### Technologies Used

- **Spring Boot**: Backend framework for building RESTful APIs.
- **PostgreSQL**: Database management system.
- **HikariCP**: JDBC connection pool for efficient database connections.
- **React**: Frontend framework.
- **Material-UI**: UI framework for styling the frontend.

### Testing

- Unit and integration tests are written using JUnit and Mockito.
- **CBTControllerTest.java** and **CBTServiceTest.java** provide tests for the backend API.

### License

© 2021 Thoughtworks, Inc.
