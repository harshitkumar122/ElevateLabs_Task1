# ElevateLabs_Task1
# 🛒 E-commerce Database Design - Task 1

## 🎯 Objective

The goal of this task is to design a structured and scalable relational database schema for an e-commerce platform. This helps build foundational skills in database modeling, table creation, and setting up relationships using keys.

## 🛠 Tools Used

- MySQL Workbench 
- SQL (Structured Query Language)

---

## 📌 Task Details

### Task 1: Database Setup and Schema Design

## 🧱 Entities & Relationships

- *Customers* can place multiple *Orders*
- Each *Order* can contain multiple *Products* through *Order_Items*
- Each *Order* has related *Payment(s)*

---

## 🧾 Database Schema (Tables)

1. *Customers*
2. *Products*
3. *Orders*
4. *Order_Items*
5. *Payments*

## 🔐 Keys Used

- Primary Keys (customer_id, product_id, etc.)
- Foreign Keys to maintain referential integrity
  - Orders.customer_id → Customers.customer_id
  - Order_Items.order_id → Orders.order_id
  - Order_Items.product_id → Products.product_id
  - Payments.order_id → Orders.order_id
