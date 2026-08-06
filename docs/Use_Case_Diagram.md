# Use Case Diagram

## AI-Powered Building Quantity Estimator & BOQ Generator

### Use Case Diagram (Text Representation)

```text
                           +----------------+
                           |      User      |
                           +--------+-------+
                                    |
      ----------------------------------------------------------
      |            |             |             |               |
      v            v             v             v               v
+-------------+ +-------------+ +-------------+ +-------------+ +----------------+
| Register /  | | Create New  | | Estimate    | | Generate    | | Download PDF / |
| Login       | | Project     | | Materials   | | BOQ         | | Excel Report   |
+-------------+ +-------------+ +-------------+ +-------------+ +----------------+
                                    |
                                    v
                           +------------------+
                           | View Cost Report |
                           +------------------+

                                    |

                           +----------------+
                           |     Admin      |
                           +--------+-------+
                                    |
             ---------------------------------------------
             |                   |                       |
             v                   v                       v
      +--------------+   +----------------+   +------------------+
      | Manage Users |   | Update Material|   | View Analytics   |
      |              |   | Rates          |   | & Reports        |
      +--------------+   +----------------+   +------------------+
```

---

## Actors

### User

A civil engineering student, contractor, architect, or engineer who uses the application.

### Admin

Manages system data such as material rates, users, and reports.

---

## User Use Cases

* Register/Login
* Create a new project
* Enter building details
* Estimate material quantities
* Generate BOQ
* View estimated cost
* Download reports in PDF/Excel

---

## Admin Use Cases

* Manage users
* Update material rates
* View project statistics
* Monitor generated BOQs

---

## Benefits

* Clearly defines system functionality.
* Helps developers understand user interactions.
* Simplifies software design.
* Useful for project documentation and presentations.
