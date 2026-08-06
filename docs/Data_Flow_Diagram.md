# Data Flow Diagram (DFD)

## Level 0 DFD (Context Diagram)

```text
                    +----------------------+
                    |        User          |
                    +----------+-----------+
                               |
          Building Details / Floor Plan
                               |
                               v
      +-------------------------------------------+
      | AI Building Quantity Estimator & BOQ App |
      +-------------------------------------------+
                               |
        Estimated Quantities / BOQ / Cost Report
                               |
                               v
                    +----------------------+
                    |        User          |
                    +----------------------+
```

---

## Level 1 DFD

```text
                     +----------------------+
                     |        User          |
                     +----------+-----------+
                                |
                                v
                 +-----------------------------+
                 | 1. Input Building Details   |
                 +-------------+---------------+
                               |
                               v
                 +-----------------------------+
                 | 2. Validate User Input      |
                 +-------------+---------------+
                               |
                               v
                 +-----------------------------+
                 | 3. Material Estimation      |
                 +-------------+---------------+
                               |
                               v
                 +-----------------------------+
                 | 4. Generate BOQ             |
                 +-------------+---------------+
                               |
                               v
                 +-----------------------------+
                 | 5. Cost Estimation          |
                 +-------------+---------------+
                               |
                               v
                 +-----------------------------+
                 | 6. PDF / Excel Report       |
                 +-------------+---------------+
                               |
                               v
                     +----------------------+
                     |        User          |
                     +----------------------+
```

---

## Data Stores

**D1 – Project Database**

* Project name
* Building dimensions
* Number of floors

**D2 – Material Database**

* Cement
* Steel
* Bricks
* Sand
* Aggregate
* Concrete

**D3 – BOQ Database**

* Material quantities
* Unit rates
* Total cost
* Generated reports

---

## Data Flow Description

1. The user enters building information.
2. The application validates the data.
3. The estimation engine calculates material quantities.
4. The BOQ module prepares the Bill of Quantities.
5. Cost estimation is performed using material rates.
6. A report is generated in PDF or Excel format.
7. Results are displayed to the user and stored for future reference.
