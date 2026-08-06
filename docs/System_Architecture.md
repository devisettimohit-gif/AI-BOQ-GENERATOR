# System Architecture

## AI-Powered Building Quantity Estimator & BOQ Generator

```text
                    +----------------------+
                    |      User            |
                    +----------+-----------+
                               |
                               v
                 +---------------------------+
                 |   Web Application (UI)    |
                 | (HTML, CSS, JavaScript)   |
                 +------------+--------------+
                              |
                              v
                 +---------------------------+
                 |      Flask Backend        |
                 |    (Business Logic)       |
                 +------------+--------------+
                              |
          +-------------------+-------------------+
          |                                       |
          v                                       v
+----------------------+              +------------------------+
|  AI Estimation       |              |     SQLite Database    |
|  Module              |              | Project & BOQ Storage  |
+----------+-----------+              +-----------+------------+
           |                                       |
           +-------------------+-------------------+
                               |
                               v
                +------------------------------+
                | BOQ & Cost Generation Module |
                +--------------+---------------+
                               |
                               v
                  +----------------------------+
                  | PDF / Excel Report Export  |
                  +----------------------------+
```

## Module Description

### 1. User Interface

Allows users to:

* Enter building dimensions.
* Upload building plans (future enhancement).
* View estimation results.
* Download reports.

### 2. Flask Backend

Processes user requests, validates inputs, performs calculations, and coordinates communication between all modules.

### 3. AI Estimation Module

Uses predefined engineering formulas and, in future versions, AI models to estimate construction materials accurately.

### 4. SQLite Database

Stores project information, generated BOQs, material estimates, and report history.

### 5. BOQ Generation Module

Converts calculated quantities into a structured Bill of Quantities with estimated costs.

### 6. Report Generator

Creates downloadable PDF and Excel reports for users.
