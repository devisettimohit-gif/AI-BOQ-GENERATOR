# Entity Relationship (ER) Diagram

## AI-Powered Building Quantity Estimator & BOQ Generator

### ER Diagram

```text
                    +----------------------+
                    |        USER          |
                    +----------------------+
                    | User_ID (PK)         |
                    | Name                 |
                    | Email                |
                    | Password             |
                    +----------+-----------+
                               |
                         Creates
                               |
                               v
                    +----------------------+
                    |      PROJECT         |
                    +----------------------+
                    | Project_ID (PK)      |
                    | User_ID (FK)         |
                    | Project_Name         |
                    | Building_Type        |
                    | Length               |
                    | Width                |
                    | Floors               |
                    | Created_Date         |
                    +----------+-----------+
                               |
                     Generates
                               |
                               v
                    +----------------------+
                    |        BOQ           |
                    +----------------------+
                    | BOQ_ID (PK)          |
                    | Project_ID (FK)      |
                    | Total_Cost           |
                    | Generated_Date       |
                    +----------+-----------+
                               |
                        Contains
                               |
                               v
                    +----------------------+
                    |      MATERIAL        |
                    +----------------------+
                    | Material_ID (PK)     |
                    | BOQ_ID (FK)          |
                    | Material_Name        |
                    | Quantity             |
                    | Unit                 |
                    | Unit_Price           |
                    | Total_Price          |
                    +----------------------+
```

---

## Relationships

* One **User** can create **many Projects**.
* One **Project** generates **one BOQ**.
* One **BOQ** contains **many Materials**.

---

## Database Tables

### USER

Stores account information.

### PROJECT

Stores building details entered by the user.

### BOQ

Stores generated Bills of Quantities and total estimated cost.

### MATERIAL

Stores the estimated quantity and cost of each construction material.

---

## Primary Keys (PK)

* User_ID
* Project_ID
* BOQ_ID
* Material_ID

## Foreign Keys (FK)

* User_ID → PROJECT
* Project_ID → BOQ
* BOQ_ID → MATERIAL

