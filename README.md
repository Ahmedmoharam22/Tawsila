# 🚕 Tawsila (توصيلة) — Inter-City Travel & Logistics Platform

> **A full-stack MERN application that connects freelance drivers with passengers through real-time trip management, flexible booking, and role-based dashboards.**

[![React](https://img.shields.io/badge/React-18-blue?style=for-the-badge&logo=react)](https://reactjs.org/)
[![TypeScript](https://img.shields.io/badge/TypeScript-5.0-blue?style=for-the-badge&logo=typescript)](https://www.typescriptlang.org/)
[![Node.js](https://img.shields.io/badge/Backend-Node.js_|_Express_|_MongoDB-green?style=for-the-badge&logo=node.js)](https://nodejs.org/)
[![TailwindCSS](https://img.shields.io/badge/TailwindCSS-3.0-38B2AC?style=for-the-badge&logo=tailwind-css)](https://tailwindcss.com/)
[![React Query](https://img.shields.io/badge/React%20Query-TanStack-FF4154?style=for-the-badge&logo=react-query)](https://tanstack.com/query/latest)

---

## 📌 Project Overview

### **The Problem We Solve:**
Inter-city travel often lacks direct communication between passengers looking for custom rides and freelance drivers seeking full trip schedules without relying on rigid traditional agencies.

### **The Solution:**
**Tawsila** establishes a dynamic two-sided marketplace for rides:
* **Passenger Requests:** Passengers browse scheduled trips or submit custom ride requests.
* **Driver Claiming Engine:** Drivers view open requests and claim them with one click, auto-generating trips.
* **Role-Based Access Control (RBAC):** Strict JWT separation ensuring customized experiences for Client and Driver accounts.
* **Data Efficiency:** Optimized server state using TanStack Query and lean MongoDB schema queries (`.populate()` & `.select()`).

---

## 📸 Screenshots & Showcase

| **🚕 Platform Landing & Overview** | **📋 Available Trips & Booking System** |
| :---: | :---: |
| <img src="https://github.com/user-attachments/assets/c6a203a5-c525-437f-9dd9-52f9e6ee10e0" alt="Tawsila Landing Page" width="100%" /> |<img width="1920" height="956" alt="APEXSTORE - Brave 4_30_2026 5_51_24 AM" src="https://github.com/user-attachments/assets/577a0251-9fa5-4ea6-bd68-876520a582b0" />  |

| **👨‍✈️ About Us & Ride Claiming** |
| :---: |
| <img width="1920" height="968" alt="APEXSTORE - Brave 4_30_2026 5_51_34 AM" src="https://github.com/user-attachments/assets/238c12f6-2a83-4b98-a0d6-be1a6dccc902" /> |

---

## 🛠️ Tech Stack & Architecture

| Layer | Technologies |
|---|---|
| **Frontend** | React.js, TypeScript, Tailwind CSS, Lucide React, Framer Motion |
| **State Management** | TanStack Query (React Query), React Context API |
| **Backend** | Node.js, Express.js |
| **Database** | MongoDB (Mongoose ODM) |
| **Authentication** | JWT (JSON Web Tokens) with RBAC |
| **Tooling & Utilities** | Vite, Axios, React Hook Form |

---

## 🏗️ System Architecture

The backend follows a clean **Controller → Service → Repository** pattern to maintain high scalability:

* **Auth Middleware:** Validates JWT tokens and attaches authenticated identities to `req.user`.
* **Route Protection:** Limits access strictly by role (e.g., claiming custom requests is restricted solely to Drivers).
* **Data Layer Optimization:** Mongoose queries leverage field selection and relationship population to minimize network payload size.

---

## ⚙️ Getting Started

### Prerequisites
* Node.js ≥ 18
* MongoDB Instance (Local or Atlas)

### 1. Clone the Repository
```bash
git clone [https://github.com/Ahmedmoharam22/Taswsila.git](https://github.com/Ahmedmoharam22/Taswsila.git)
cd Taswsila
