# 🚗 Fleet Vehicle Management System — DBMS Project

> A comprehensive software-based solution to monitor, manage, and optimize fleet vehicle operations using Database Management System concepts.

**Student:** Jeevithasri R (927623BEC091)  
**Course:** Database Management Systems  
**Institution:** M. Kumarasamy College of Engineering (Autonomous)

---

## 📌 Abstract

The Fleet Vehicle Management System integrates GPS tracking, real-time vehicle diagnostics, route optimization, fuel usage monitoring, driver behavior analysis, and maintenance scheduling. By leveraging cloud computing and IoT technologies, it ensures effective fleet coordination, enhances operational efficiency, reduces fuel costs, and improves safety.

**Suitable for:** Delivery services, logistics, public transportation, and field service operations.

---

## 🎯 Objective

- Automate monitoring, control, and optimization of fleet operations
- Enable real-time vehicle tracking and driver behaviour analysis
- Provide route planning and maintenance scheduling from a centralized dashboard
- Reduce operational costs and improve vehicle safety using GPS, IoT, and cloud computing

---

## ⚙️ System Architecture

The system architecture consists of:

- **UI Proxy** – Connects user interfaces to backend services
- **Fleet Location Services** – Fetches real-time data from fleet databases
- **Service Station Services** – Fetches data from service station databases
- **Fleet Location Simulator** – Generates vehicle movement data
- **Location Ingest Module** – Processes and stores movement data
- **Dashboards & Configuration Interfaces** – Displays live data to managers
- **Alert System** – Notifies on vehicle failures or issues

---

## 🗃️ Database Concepts Used

| Concept | Description |
|--------|-------------|
| ER Model | Visual representation of entities (Vehicle, Driver, Trip) and their relationships |
| Relational Model | Data organized into tables with primary and foreign keys |
| Normalization | 1NF, 2NF, 3NF applied to reduce redundancy and ensure data integrity |
| Indexing | Indexed fields: `driver_id`, `vehicle_id`, `trip_id` for faster queries |
| SQL | SELECT, INSERT, UPDATE, DELETE operations |
| ACID Properties | Atomicity, Consistency, Isolation, Durability for transactions |
| Data Integrity | Enforced via NOT NULL, UNIQUE constraints and validation rules |
| Access Control | Role-based access — Admins (full), Mechanics (maintenance only) |

---

## 🔗 E-R Diagram Entities

### Driver
- Attributes: ID, Firstname, Phone Number, Status, License No

### Vehicle
- Attributes: ID, Make, Model, Year

### Trip
- Attributes: Trip ID, Driver ID, Vehicle ID, Start Date, Start Location

### Relationships
- **VEHICLES** — Driver assigned to one or more vehicles (Many-to-Many)
- **TRIP** — Links Driver and Vehicle through Driver ID and Vehicle ID

---

## 📦 Modules

### 1. User Interface Module
- Welcome page collecting customer name and contact number
- Trip booking form with vehicle, driver, date, pickup, and destination fields
- Built with HTML, CSS, and JavaScript with form validation

### 2. Vehicle & Driver Management Module
- Storage and retrieval of vehicle and driver details
- Driver availability and assignment tracking

### 3. Trip Scheduling Module
- Accepts trip date, pickup point, and destination
- Validates entries and connects driver and vehicle data to each trip

### 4. Database Management Module
- Performs CRUD operations (Create, Read, Update, Delete)
- Ensures data consistency and integrity across all modules

### 5. Report & Confirmation Module
- Displays trip summary after submission
- Generates logs of completed and pending trips
- Extendable to email/SMS confirmations

---

## 🖥️ Results

### Welcome Page
Users enter their **name** and **contact number** to access the system. A clean, centered layout with a "Start" button leads to the trip booking section.

### Trip Detail Form
Allows users to select:
- Vehicle name
- Driver name (dropdown)
- Trip start and end dates
- Pickup point and destination

### Trip History Page
Displays a table of all booked trips with:
- Trip ID, Vehicle, Driver, Start/End Dates, Pickup, Endpoint, Status
- Option to **cancel** a trip

---

## 🛠️ Tech Stack

| Layer | Technology |
|-------|-----------|
| Frontend | HTML, CSS, JavaScript |
| Backend | Python (Flask) |
| Templating | Jinja2 |
| Database | MySQL / PostgreSQL |
| Architecture | MVC Pattern |

---

## ✅ Conclusion

The Fleet Vehicle Management System provides an efficient, centralized solution for fleet operations. Automation of routine tasks and real-time data access empower fleet managers to make informed decisions — optimizing resource utilization, minimizing downtime, and ensuring reliable fleet operation.

---

## 📚 References

1. Patel, R., & Mehta, S. (2020). A Smart Fleet Management System Using GPS and GSM. *IJSREM*, 4(8), 23–29.
2. Kumar, V., & Singh, A. (2021). Design and Implementation of Vehicle Tracking System Using IoT. *JETIR*, 8(3), 66–72.
3. Bharathi, V., & Rajkumar, S. (2019). Fleet Management Using Database Systems. *IJCA*, 178(5), 12–18.
4. Zhang, Y., & Tan, W. (2018). Optimizing Fleet Routing and Scheduling Using Software Systems. *Transportation Research Procedia*, 32, 142–149.
5. Mohan, K., & Saran, R. (2022). Web-Based Fleet Management Application Using MERN Stack. *IJARCS*, 13(2), 90–97.

---

## 📜 License

Submitted for academic purposes — Database Management Systems, B.E. (ECE)  
M. Kumarasamy College of Engineering (Autonomous), Anna University Chennai.
