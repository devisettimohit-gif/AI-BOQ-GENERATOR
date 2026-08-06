# Sequence Diagram

## AI-Powered Building Quantity Estimator & BOQ Generator

### Sequence Diagram

```text
+--------+     +--------------+     +---------------+     +----------------+     +---------------+
| User   |     | Web Frontend |     | Flask Backend |     | AI Estimation  |     | Database      |
+--------+     +--------------+     +---------------+     +----------------+     +---------------+
     |                 |                    |                     |                      |
     | Open Website    |                    |                     |                      |
     |---------------->|                    |                     |                      |
     |                 | Display Home Page  |                     |                      |
     |                 |------------------->|                     |                      |
     |                 |                    |                     |                      |
     | Enter Building Details               |                     |                      |
     |---------------->|                    |                     |                      |
     |                 | Send Data -------->|                     |                      |
     |                 |                    | Validate Input      |                      |
     |                 |                    |-------------------->|                      |
     |                 |                    | Estimate Materials  |                      |
     |                 |                    |-------------------->|                      |
     |                 |                    |<--------------------|                      |
     |                 |                    | Store Results ---------------------------->|
     |                 |                    |<------------------------------------------|
     |                 | Display BOQ <------|                     |                      |
     |<----------------|                    |                     |                      |
     | Download PDF    |                    |                     |                      |
     |---------------->|                    |                     |                      |
     |                 | Generate Report -->|                     |                      |
     |                 |<-------------------|                     |                      |
     | Receive Report  |                    |                     |                      |
     |<----------------|                    |                     |                      |
```

---

## Sequence Description

1. The user opens the web application.
2. The frontend displays the home page.
3. The user enters building details.
4. The frontend sends the data to the Flask backend.
5. The backend validates the input.
6. The AI estimation module calculates material quantities.
7. The backend stores the generated BOQ in the database.
8. The frontend displays the BOQ and estimated cost.
9. The user downloads the report as a PDF or Excel file.

---

## Benefits

* Clearly shows communication between system components.
* Helps developers understand the request flow.
* Useful for software design documentation.
* Demonstrates the complete BOQ generation process.

