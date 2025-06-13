#  Airport Management System

##  Project Description

The **Airport Management System** is a web-based application designed to manage and display flight-related information such as flight schedules, arrivals, departures, and registrations. It provides a user-friendly interface built with **HTML**, **CSS**, and **JavaScript**, and uses **Java Servlets** and **JSP (Java Server Pages)** for backend processing. Data is stored and retrieved from a **MySQL** database.

---

## 🛠 Technologies Used

- **Frontend**:
  - HTML5
  - CSS3
  - JavaScript
- **Backend**:
  - Java Servlets
  - JSP (Java Server Pages)
- **Database**:
  - MySQL
- **Tools/Server**:
  - Apache Tomcat
  - Eclipse/NetBeans (Java IDE)
  - JDBC Connector

---

## 🚀 Features

- 🛫 **Flight Departure Schedule**
  - Display departure time, date, onboard status, flight name, ID, destination, and registration number.
  - Dynamic data fetched from MySQL database via Servlet.

- 🛬 **Flight Arrival Schedule**
  - View incoming flights with details like source, flight status, and time.

- 📅 **Add/Update Flight Schedules**
  - Admin interface to manage flight data.

- 🔍 **Search Flights**
  - Filter flights by ID, name, destination, or date.

- 📊 **Dashboard**
  - View summary information and access main modules.

- 📂 **Responsive Design**
  - Clean, simple UI using CSS Grid/Flexbox and JavaScript interactions.

---

## 🧱 Database Schema

**Database Name**: `airportdb`

**Example Table**: `flights`
```sql
CREATE TABLE flights (
  id INT AUTO_INCREMENT PRIMARY KEY,
  flight_id VARCHAR(50),
  flight_name VARCHAR(100),
  destination VARCHAR(100),
  departure_time TIME,
  departure_date DATE,
  onboard_status VARCHAR(20),
  registration_no VARCHAR(50)
);
