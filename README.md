# UrbandFoods - Food Ordering Platform (Group 15)

UrbandFoods is a comprehensive food ordering and delivery management platform designed with a microservices-inspired architecture. The system enables seamless interaction between Customers, Delivery Personnel, and Suppliers through dedicated applications.

## 📂 Project Architecture

The solution is divided into three core modules, each comprising a dedicated Frontend and Backend service:

### 1. Customer Module
* **Purpose:** Allows users to browse food items, manage carts, place orders, and track history.
* **Frontend:** React + Vite
* **Backend:** Spring Boot (Java)
* **Database:** Oracle & MongoDB

### 2. Delivery Module
* **Purpose:** specialized interface for delivery personnel to manage and track assigned deliveries.
* **Frontend:** React + Vite
* **Backend:** Spring Boot (Java)
* **Database:** Oracle

### 3. Supplier Module
* **Purpose:** Admin-like interface for suppliers to manage product inventory and view sales data.
* **Frontend:** React + Vite
* **Backend:** Spring Boot (Java)
* **Database:** Oracle

---

## 🚀 Technology Stack

### Backend
* **Framework:** Spring Boot 3.4.4
* **Language:** Java 17
* **Build Tool:** Maven
* **Data Access:** Spring Data JPA
* **Databases:** * Oracle Database (Primary Relational DB)
  * MongoDB (Used in Customer module)

### Frontend
* **Framework:** React 19
* **Build Tool:** Vite
* **Styling:** Bootstrap 5.3 & React-Bootstrap
* **HTTP Client:** Axios
* **Routing:** React Router DOM

---

## 🛠️ Installation & Setup Guide

### Prerequisites
Ensure you have the following installed on your machine:
* **Java Development Kit (JDK) 17** or higher
* **Node.js** (LTS Version)
* **Maven**
* **Oracle Database**
* **MongoDB** (Running locally or cloud)

### Step 1: Database Initialization
Before running the backend services, execute the SQL scripts located in the `PL-SQL` folder to set up your Oracle database schemas.

1. **Customer Tables:** Run scripts from `PL-SQL/Customer/`
2. **Delivery Tables:** Run scripts from `PL-SQL/Delivery/`
3. **Supplier Tables:** Run scripts from `PL-SQL/Supplier/`

### Step 2: Backend Configuration & Execution
Navigate to each backend directory and start the Spring Boot application.

**1. Customer Backend**
cd Backend/Customer-Backend/UrbanFood/UrbanFood
# Update src/main/resources/application.properties with your DB credentials
./mvnw spring-boot:run
2. Delivery Backend

Bash

cd Backend/Delivery-Backend/Delivery/Delivery
# Update src/main/resources/application.properties with your DB credentials
./mvnw spring-boot:run
3. Supplier Backend

Bash

cd Backend/Supplier-Backend
# Update src/main/resources/application.properties with your DB credentials
./mvnw spring-boot:run
Step 3: Frontend Installation & Execution
Open three separate terminal windows to run the frontend applications simultaneously.

1. Customer Web App

Bash

cd Frontend/Customer-Frontend
npm install
npm run dev
2. Delivery Web App

Bash

cd "Frontend/Delivery-Frontend/Delivery - Frontend"
npm install
npm run dev
3. Supplier Web App

Bash

cd Frontend/Supplier-Frontend/urbanfood
npm install
npm run dev
🔮 Key Features
User Authentication: Secure login and registration for Customers, Suppliers, and Delivery staff.

Product Management: Suppliers can add, update, and remove food items.

Shopping Cart: Customers can add items to a cart and place orders.

Order & Delivery Tracking: Real-time status updates for orders.

Review System: Customers can leave reviews for products.

Sales Dashboard: Suppliers can view high-demand products and sales summaries.

👥 Contributors
Group 15
