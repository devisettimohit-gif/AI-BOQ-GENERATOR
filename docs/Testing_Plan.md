# Testing Plan

# AI-Powered Building Quantity Estimator & BOQ Generator

## 1. Objective

The objective of testing is to verify that the application functions correctly, produces accurate quantity estimates, generates Bills of Quantities (BOQs), and provides a smooth user experience.

---

# 2. Testing Types

## Unit Testing

Tests each module independently.

Modules:

* User Authentication
* Project Creation
* Material Estimation
* BOQ Generation
* Cost Calculation
* Report Export

---

## Integration Testing

Verifies communication between:

* Frontend ↔ Backend
* Backend ↔ AI Estimation Module
* Backend ↔ Database
* Backend ↔ Report Generator

---

## System Testing

Tests the complete application to ensure all components work together correctly.

---

## User Acceptance Testing (UAT)

Civil engineering students, faculty members, or contractors verify that the application meets user requirements.

---

# 3. Test Cases

| Test ID | Test Scenario          | Expected Result                   | Status |
| ------- | ---------------------- | --------------------------------- | ------ |
| TC-01   | User Registration      | Account created successfully      | Pass   |
| TC-02   | User Login             | User logs in successfully         | Pass   |
| TC-03   | Create Project         | New project is saved              | Pass   |
| TC-04   | Enter Building Details | Data accepted and validated       | Pass   |
| TC-05   | Estimate Materials     | Quantities calculated correctly   | Pass   |
| TC-06   | Generate BOQ           | BOQ displayed successfully        | Pass   |
| TC-07   | Cost Estimation        | Total cost calculated correctly   | Pass   |
| TC-08   | Download PDF           | PDF generated successfully        | Pass   |
| TC-09   | Download Excel         | Excel file generated successfully | Pass   |
| TC-10   | Invalid Input          | Error message displayed           | Pass   |

---

# 4. Performance Testing

* Response time should be less than 5 seconds for standard building projects.
* The system should support multiple users without significant delays.

---

# 5. Security Testing

* User authentication required.
* Passwords stored securely.
* Prevent unauthorized access to project data.

---

# 6. Compatibility Testing

The application should work correctly on:

* Google Chrome
* Microsoft Edge
* Mozilla Firefox

It should also display properly on:

* Desktop
* Laptop
* Tablet

---

# 7. Success Criteria

The project is considered successful if:

* All test cases pass.
* BOQ calculations are accurate.
* Reports are generated without errors.
* Users can easily navigate the application.
* The system performs reliably under normal usage.
