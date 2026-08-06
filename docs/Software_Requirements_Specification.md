# Software Requirements Specification (SRS)

# AI-Powered Building Quantity Estimator & BOQ Generator

## Version

1.0

---

# 1. Introduction

## 1.1 Purpose

The purpose of this project is to develop an AI-powered web application that automatically estimates construction material quantities and generates a Bill of Quantities (BOQ). The application aims to reduce manual calculations, improve estimation accuracy, and save time for civil engineers, contractors, architects, and students.

## 1.2 Scope

The system will:

* Accept building details from users.
* Estimate quantities of construction materials.
* Generate BOQs automatically.
* Estimate project costs.
* Export reports in PDF and Excel formats.

---

# 2. Overall Description

## Product Perspective

The application is a standalone web-based system that performs quantity estimation and BOQ generation using engineering calculations and AI-assisted features.

## Product Functions

* User Registration/Login
* Create New Project
* Enter Building Dimensions
* Estimate Material Quantities
* Generate BOQ
* Cost Estimation
* Download Reports
* Save Projects

## User Classes

* Civil Engineering Students
* Civil Engineers
* Contractors
* Architects
* Quantity Surveyors

---

# 3. Functional Requirements

### FR-1 User Authentication

Users shall be able to register and log in.

### FR-2 Project Creation

Users shall be able to create and save multiple projects.

### FR-3 Building Details

Users shall enter:

* Building type
* Length
* Width
* Height
* Number of floors

### FR-4 Material Estimation

The system shall estimate:

* Cement
* Steel
* Bricks
* Sand
* Aggregate
* Concrete

### FR-5 BOQ Generation

The system shall automatically generate a Bill of Quantities.

### FR-6 Cost Estimation

The system shall estimate the total construction material cost.

### FR-7 Report Export

The system shall export reports as PDF and Excel files.

---

# 4. Non-Functional Requirements

## Performance

* Response time under 5 seconds for standard projects.

## Security

* User passwords should be encrypted.
* Access should require authentication.

## Reliability

* Calculations should be consistent and accurate.

## Availability

* The application should be accessible whenever the server is running.

## Usability

* The interface should be simple and intuitive.

---

# 5. Hardware Requirements

* Laptop/Desktop
* Minimum 4 GB RAM
* Internet connection

---

# 6. Software Requirements

Frontend:

* HTML
* CSS
* JavaScript

Backend:

* Python
* Flask

Database:

* SQLite

Development Tools:

* Visual Studio Code
* Git
* GitHub

---

# 7. Future Scope

* AI-based floor plan recognition.
* BIM integration.
* Mobile application.
* Voice input.
* Multi-language support.
* Cloud project storage.
* Live material price updates.

---

# 8. Conclusion

The AI-Powered Building Quantity Estimator & BOQ Generator will simplify quantity estimation, reduce human error, and provide an efficient digital solution for BOQ preparation. The project is designed to be scalable and can evolve into a comprehensive construction management platform.
