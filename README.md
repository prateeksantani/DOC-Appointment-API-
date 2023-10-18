# DOC-Appointment-API-

# Project README

This README provides an overview of the project structure and the roles of the three primary controller classes: `AdminController`, `DoctorController`, and `PatientController`. These controllers are crucial components of the project, responsible for handling various endpoints and facilitating communication with the associated services. Below, we'll briefly describe each controller class and their respective functions.

## Project Overview

This project is designed to manage and provide services related to doctors and patients. It employs a Spring Boot framework, which simplifies the development of Java-based enterprise applications. The controllers are essential for handling HTTP requests and interfacing with the relevant services. Here are the primary controller classes:

## `AdminController`

### Responsibilities
- Manages administrative functions related to the application.
- Provides endpoints for adding new doctors.
- Retrieves a list of all patients.
- Retrieves a list of patients based on their blood group.

### Endpoints
- `GET /patients`: Retrieves a list of all patients.
- `POST /doctor`: Adds a new doctor to the system.
- `GET /patients/bloodGroup/{bloodGroup}`: Retrieves a list of patients with a specific blood group.

## `DoctorController`

### Responsibilities
- Manages doctor-related functions.
- Provides endpoints for retrieving all doctors.
- Retrieves a specific doctor by their ID.

### Endpoints
- `GET /doctors`: Retrieves a list of all doctors. 
- `GET /doctor/{id}`: Retrieves a specific doctor by their ID.

## `PatientController`

### Responsibilities
- Manages patient-related functions.
- Provides endpoints for retrieving all patients.

### Endpoints
- `GET /patients`: Retrieves a list of all patients.

## Controller Structure

All controllers are annotated with `@RestController`, indicating that they handle incoming HTTP requests and produce JSON responses. Additionally, the `@Validated` annotation is used for input validation. Each controller relies on a relevant service to execute business logic.

## Dependencies

These controllers have dependencies on the following services:
- `DoctorService`: Handles doctor-related operations.
- `PatientService`: Manages patient-related operations.

## Documentation

Ensure that comprehensive documentation is provided for each endpoint, including input parameters, expected responses, and potential error conditions. This documentation is vital for developers and clients who interact with the API.

## Conclusion

These controller classes are fundamental to the project's architecture. They manage the flow of information between the API endpoints and the business logic contained in the services. Understanding the responsibilities and endpoints of each controller is crucial for developing, testing, and maintaining this application. Additionally, it is important to document the API to make it more accessible to other developers and clients.
