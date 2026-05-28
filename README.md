# Inventory Movement Dashboard

A full-stack web application designed to validate, parse, and visualize stock movement data. The application requires users to upload a JSON file containing stock records, verifies the file's integrity using a SHA-256 hash calculated on the frontend, and then displays the data using interactive charts and a paginated table.

## 🚀 Features
* **Secure Uploads:** Calculates a SHA-256 hash of the selected JSON file on the client side and verifies it on the server before parsing.
* **Interactive Dashboard:** Visualizes stock movements using Recharts (Pie Chart for IN/OUT proportions, Line Chart for time-series quantity trends).
* **Dynamic Filtering:** Filter data by Date Range (From/To) and Movement Type (All, IN, OUT).
* **Paginated Data Table:** Displays raw stock movement records with 10 rows per page.

## 🛠️ Tech Stack
* **Frontend:** React 18, Vite, Axios, Recharts
* **Backend:** Java 17, Spring Boot 3, Jackson (JSON parsing)
* **Storage:** Local File System (`movements.json`)

---

## ⚙️ Prerequisites
Before you begin, ensure you have the following installed on your machine:
* **Java 17** or higher
* **Maven** (for building the backend)
* **Node.js** (v18+ recommended) and **npm**

---

## 🏃‍♂️ Getting Started

### 1. Running the Backend (Spring Boot)
The backend acts as the REST API and data validation layer.

1. Open your terminal and navigate to the backend project directory.
2. Build the project using Maven:
   ```bash
   mvn clean install
