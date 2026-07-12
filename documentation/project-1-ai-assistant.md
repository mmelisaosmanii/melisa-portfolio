# AI Assistant for NGOs

## 1. Project Vision

AI Assistant for NGOs is a digital platform designed to help non-governmental organizations improve their daily work using artificial intelligence.

The system helps NGO staff manage documents, generate reports, translate content, and receive information through an AI-powered chatbot.

The goal of this project is to reduce manual work, save time, and support NGOs in making better decisions through AI technology.

## 2. Problem Statement

Many NGOs work with large amounts of information, including reports, project documents, research papers, and communication materials.

Managing and analyzing these documents manually requires significant time and effort. NGOs also need to create reports, translate information into different languages, and quickly access important data for decision-making.

This project aims to solve these challenges by providing an AI-powered assistant that helps NGO staff automate repetitive tasks, improve productivity, and focus more on their social impact activities.

## 3. Target Users

## 3. Target Users

### NGO Staff
Employees who work with documents, reports, and project information. They use the AI assistant to summarize documents, generate reports, translate content, and quickly find information.

### Project Managers
People responsible for managing NGO projects. They use the system to prepare reports, analyze information, and support decision-making.

### Administrators
System administrators who manage users, permissions, and platform settings.

### External Partners (Future Improvement)
Organizations or partners who may interact with the platform to access shared information or collaborate on projects.

## 4. Main Features

## 4. Main Features

### AI Chatbot
An AI-powered assistant that allows NGO staff to ask questions, receive information, and get support with daily tasks.

### Document Summarization
The system can analyze uploaded documents and generate short summaries to help users understand large amounts of information quickly.

### Document Translation
Users can translate documents and content into different languages to support international communication and collaboration.

### AI Report Generation
The system can generate structured reports based on provided information, reducing manual report writing time.

### User Authentication and Roles
The platform provides secure login and different access levels for NGO staff, project managers, and administrators.

### Document Management
Users can upload, store, organize, and manage important NGO documents inside the platform.

### Dashboard and Activity Overview
Users can view important information, recent activities, and AI assistant usage statistics through a dashboard.

## 5. Technology Stack
## 5. Technology Stack

### Frontend
**React.js**

React is used to build a modern, interactive, and responsive user interface. It allows the application to be organized into reusable components and provides a better user experience.

### Backend
**Node.js + Express.js**

Node.js is used to build the backend API and handle communication between the frontend, database, and AI services. Express.js helps create structured and scalable REST APIs.

### Database
**MySQL**

MySQL is used to store application data such as users, roles, documents, conversations, and generated reports.

### Artificial Intelligence
**OpenAI API or Alternative AI Model**

An AI model is integrated to provide chatbot functionality, document summarization, translation, and automated report generation.

### Authentication
**JWT (JSON Web Token)**

JWT is used to provide secure user authentication and role-based access control.

### Development Tools
- Visual Studio Code
- Git and GitHub
- Postman for API testing
- Figma for UI/UX design

### Future Technologies
- Docker for containerization
- Cloud deployment platforms
- Advanced AI models

## 6. System Architecture

## 6. System Architecture

The AI Assistant for NGOs follows a client-server architecture where the frontend, backend, database, and AI services communicate with each other.

### Architecture Components

### 1. Frontend Layer - React.js
The frontend provides the user interface where NGO staff can:
- interact with the AI chatbot
- upload documents
- view generated reports
- manage their account

The frontend communicates with the backend through REST API requests.

### 2. Backend Layer - Node.js + Express.js
The backend acts as the main application server.

Responsibilities:
- handle user authentication
- manage business logic
- process API requests
- communicate with the database
- communicate with the AI service

### 3. Database Layer - MySQL
The database stores:
- user information
- roles and permissions
- uploaded documents
- chat history
- generated reports

### 4. AI Service Layer
The AI service provides intelligent features:

- chatbot responses
- document summarization
- translation
- report generation

### System Communication Flow

1. User interacts with the React frontend.
2. Frontend sends requests to the Node.js backend API.
3. Backend validates requests and processes the required operation.
4. Backend communicates with MySQL database and AI service.
5. Results are returned back to the user through the frontend.


## 7. Database Design

## 7. Database Design

The system uses MySQL as a relational database to store and manage application data.

### Database Tables

### 1. Users Table

Stores information about registered users.

Fields:
- user_id (Primary Key)
- full_name
- email
- password_hash
- role_id (Foreign Key)
- created_at

Purpose:
Stores NGO staff, project managers, and administrators.

---

### 2. Roles Table

Stores different user roles and permissions.

Fields:
- role_id (Primary Key)
- role_name

Examples:
- Admin
- Project Manager
- NGO Staff

---

### 3. Documents Table

Stores uploaded NGO documents.

Fields:
- document_id (Primary Key)
- user_id (Foreign Key)
- title
- file_path
- document_type
- uploaded_at

Purpose:
Stores documents that will be analyzed by the AI assistant.

---

### 4. Conversations Table

Stores chatbot interactions.

Fields:
- conversation_id (Primary Key)
- user_id (Foreign Key)
- user_message
- ai_response
- created_at

Purpose:
Keeps history of conversations between users and the AI assistant.

---

### 5. Reports Table

Stores generated AI reports.

Fields:
- report_id (Primary Key)
- user_id (Foreign Key)
- title
- content
- created_at

Purpose:
Stores reports created by the AI system.

---

## Database Relationships

- One role can have many users.
- One user can upload many documents.
- One user can have many conversations.
- One user can generate many reports.

## 8. Future Improvements

## 8. Future Improvements

The AI Assistant for NGOs can be improved and expanded with additional features in the future.

### Advanced AI Capabilities
- Integration with more advanced AI models.
- Better document understanding and analysis.
- Personalized AI assistance based on NGO activities.

### Cloud Deployment
- Deploy the application using cloud platforms.
- Improve scalability and availability.
- Implement cloud storage for documents.

### Mobile Application
- Develop a mobile application for NGO staff.
- Allow users to access the AI assistant from anywhere.

### Data Analytics Dashboard
- Provide insights about documents, reports, and organizational activities.
- Visualize important information through charts and dashboards.

### Enhanced Security
- Implement stronger authentication methods.
- Add advanced permission management.
- Improve data protection and privacy.

### Multi-language Support
- Support more languages to help international organizations collaborate more effectively.