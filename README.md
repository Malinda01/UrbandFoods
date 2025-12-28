# 🍔 UrbandFoods – Food Ordering Platform

**Group 15**

UrbandFoods is a comprehensive food ordering and delivery management platform built using a **microservices-inspired architecture**. The system enables seamless interaction between **Customers**, **Delivery Personnel**, and **Suppliers** through dedicated applications, each with its own frontend and backend services.

---

## 📌 Overview

The platform is designed to simulate a real-world food delivery ecosystem with clear separation of concerns. Each module operates independently while collectively supporting end-to-end food ordering, fulfillment, and delivery workflows.

---

## 🏗️ Project Architecture

The solution consists of **three core modules**, each containing a dedicated **Frontend** and **Backend** service.

### 1️⃣ Customer Module

* **Purpose:** Enables customers to browse food items, manage carts, place orders, view order history, and submit reviews.
* **Frontend:** React + Vite
* **Backend:** Spring Boot (Java)
* **Databases:** Oracle Database & MongoDB

### 2️⃣ Delivery Module

* **Purpose:** Provides delivery personnel with tools to view, manage, and track assigned deliveries.
* **Frontend:** React + Vite
* **Backend:** Spring Boot (Java)
* **Database:** Oracle Database

### 3️⃣ Supplier Module

* **Purpose:** Acts as an admin-style interface for suppliers to manage food items, inventory, and sales analytics.
* **Frontend:** React + Vite
* **Backend:** Spring Boot (Java)
* **Database:** Oracle Database

---

## 🚀 Technology Stack

### 🔙 Backend

* **Framework:** Spring Boot 3.4.4
* **Language:** Java 17
* **Build Tool:** Maven
* **ORM / Data Access:** Spring Data JPA
* **Databases:**

  * Oracle Database (Primary relational database)
  * MongoDB (Used in the Customer module)

### 🎨 Frontend

* **Framework:** React 19
* **Build Tool:** Vite
* **Styling:** Bootstrap 5.3, React-Bootstrap
* **HTTP Client:** Axios
* **Routing:** React Router DOM

---

## 🛠️ Installation & Setup Guide

### ✅ Prerequisites

Make sure the following tools are installed on your system:

* Java Development Kit (JDK) 17 or higher
* Node.js (LTS version recommended)
* Apache Maven
* Oracle Database
* MongoDB (local or cloud instance)

---

### 🗄️ Step 1: Database Initialization

Before starting the backend services, initialize the Oracle database schemas by running the provided SQL scripts.

1. **Customer Module Tables**
   Run scripts from:

   ```
   PL-SQL/Customer/
   ```

2. **Delivery Module Tables**
   Run scripts from:

   ```
   PL-SQL/Delivery/
   ```

3. **Supplier Module Tables**
   Run scripts from:

   ```
   PL-SQL/Supplier/
   ```

---

### ⚙️ Step 2: Backend Configuration & Execution

Navigate to each backend service directory, update database credentials in `application.properties`, and start the service.

#### 1. Customer Backend

```bash
cd Backend/Customer-Backend/UrbanFood/UrbanFood
# Update src/main/resources/application.properties
./mvnw spring-boot:run
```

#### 2. Delivery Backend

```bash
cd Backend/Delivery-Backend/Delivery/Delivery
# Update src/main/resources/application.properties
./mvnw spring-boot:run
```

#### 3. Supplier Backend

```bash
cd Backend/Supplier-Backend
# Update src/main/resources/application.properties
./mvnw spring-boot:run
```

---

### 🖥️ Step 3: Frontend Installation & Execution

Open **three separate terminal windows** and run the frontend applications in parallel.

#### 1. Customer Web Application

```bash
cd Frontend/Customer-Frontend
npm install
npm run dev
```

#### 2. Delivery Web Application

```bash
cd "Frontend/Delivery-Frontend/Delivery - Frontend"
npm install
npm run dev
```

#### 3. Supplier Web Application

```bash
cd Frontend/Supplier-Frontend/urbanfood
npm install
npm run dev
```

---

## ✨ Key Features

* 🔐 **User Authentication**
  Secure login and registration for Customers, Suppliers, and Delivery Personnel.

* 🛒 **Shopping Cart & Ordering**
  Customers can add items to carts and place orders seamlessly.

* 📦 **Product Management**
  Suppliers can add, update, and remove food items.

* 🚚 **Order & Delivery Tracking**
  Real-time tracking and status updates for customer orders.

* ⭐ **Review System**
  Customers can submit reviews and ratings for food items.

* 📊 **Sales Dashboard**
  Suppliers can analyze sales data and identify high-demand products.

---

