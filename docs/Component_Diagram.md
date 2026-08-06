# Component Diagram

## AI-Powered Building Quantity Estimator & BOQ Generator

### Component Diagram

```text
                            +----------------------+
                            |      Web Browser     |
                            +----------+-----------+
                                       |
                                       |
                                       v
                     +----------------------------------+
                     |     Frontend (HTML/CSS/JS)       |
                     | - Home Page                      |
                     | - Project Form                   |
                     | - Dashboard                      |
                     | - BOQ Results                    |
                     +---------------+------------------+
                                     |
                                     |
                                     v
                     +----------------------------------+
                     |       Flask Backend API          |
                     | - Authentication                 |
                     | - Project Management             |
                     | - BOQ Generation                 |
                     | - Cost Calculation               |
                     +---------------+------------------+
                                     |
             +-----------------------+------------------------+
             |                                                |
             v                                                v
+-------------------------------+             +-------------------------------+
| AI Estimation Engine          |             | SQLite Database               |
| - Quantity Estimation         |             | - Users                       |
| - Material Calculations       |             | - Projects                    |
| - AI Assistance               |             | - BOQs                        |
+---------------+---------------+             | - Materials                   |
                |                             +-------------------------------+
                |
                v
+-------------------------------+
| Report Generator              |
| - PDF Export                  |
| - Excel Export                |
+-------------------------------+
```

---

## Components

### 1. Frontend

Responsible for collecting user input and displaying BOQ results.

### 2. Flask Backend

Handles business logic, validates user input, performs calculations, and coordinates all system components.

### 3. AI Estimation Engine

Calculates construction material quantities based on engineering formulas and supports AI-assisted estimation.

### 4. SQLite Database

Stores user accounts, project details, BOQs, and material information.

### 5. Report Generator

Creates downloadable PDF and Excel reports for users.

---

## Advantages

* Modular and easy to maintain.
* Components can be upgraded independently.
* Supports future enhancements such as BIM integration, cloud storage, and AI-based floor plan recognition.
