<div align="center">

<img src="https://capsule-render.vercel.app/api?type=waving&color=gradient&customColorList=0,2,2,5,30&height=200&section=header&text=PHARMACY%20%E2%80%94%20SERVER&fontSize=54&fontColor=FFD700&fontAlignY=42&desc=⚡%20Node.js%20%2B%20Express%20REST%20API%20%C2%B7%20Dockerized%20Backend&descAlignY=62&descColor=DCDCDC&animation=fadeIn" width="100%"/>

[![Typing SVG](https://readme-typing-svg.demolab.com?font=Share+Tech+Mono&weight=700&size=20&duration=2800&pause=900&color=FFD700&center=true&vCenter=true&width=760&lines=%E2%9A%A1+RESTful+API+for+Orders+%26+Products;%F0%9F%A7%BE+Prescription+File+Handling;%F0%9F%94%92+JWT+Auth+%2B+Admin+Passphrase;%F0%9F%90%B3+Fully+Dockerized+Backend)](https://git.io/typing-svg)

<br/>

<p align="center">
  <a href="https://nodejs.org/">
    <img src="https://img.shields.io/badge/Backend-Node.js-339933?style=for-the-badge&logo=node.js&logoColor=white"/>
  </a>
  <a href="https://expressjs.com/">
    <img src="https://img.shields.io/badge/Framework-Express.js-lightgrey?style=for-the-badge&logo=express"/>
  </a>
  <a href="https://www.mongodb.com/">
    <img src="https://img.shields.io/badge/Database-MongoDB-47A248?style=for-the-badge&logo=mongodb&logoColor=white"/>
  </a>
  <a href="https://www.docker.com/">
    <img src="https://img.shields.io/badge/Docker-Containerized-2496ED?style=for-the-badge&logo=docker&logoColor=white"/>
  </a>
  <a href="https://opensource.org/licenses/MIT">
    <img src="https://img.shields.io/badge/License-MIT-yellow.svg?style=for-the-badge"/>
  </a>
</p>

<p align="center">
  <a href="https://github.com/NietoDeveloper/Pharmacy/tree/main/server">
    <img src="https://img.shields.io/badge/📂_Source-NietoDeveloper%2FPharmacy%2Fserver-000000?style=for-the-badge&logo=github&logoColor=FFD700"/>
  </a>
</p>

</div>

---

## 📋 Overview

The **server** for the **Pharmacy** application. Built with **Node.js** and **Express.js**, it exposes RESTful endpoints for user authentication, product management, cart and order processing, and prescription file handling, backed by **MongoDB** and secured with **JWT** authentication and an admin passphrase.

---

## 🗂️ Project Structure

```text
server/
├── middleware/       # JWT auth guards and request validation
├── models/            # Mongoose schemas (Users, Products, Orders, Messages)
├── prescriptions/       # Uploaded prescription files (Multer storage)
└── routes/               # RESTful API endpoint definitions
```

---

## 🔄 Order & Prescription Flow

```mermaid
flowchart LR
    A([🌐 Client Request]) --> B[Routes]
    B --> C[Middleware]
    C -->|JWT Validated| D[Business Logic]
    D -->|CRUD| E[(Models\nProducts / Orders / Users)]
    D -->|Upload| F[(Prescriptions\nMulter Storage)]
    E -->|Response| G([📦 JSON Payload])
    F -->|Reference| G

    style A fill:#FFD700,color:#000,stroke:#FFD700
    style D fill:#0a0a0a,color:#FFD700,stroke:#FFD700
    style E fill:#47A248,color:#fff,stroke:#47A248
    style G fill:#000,color:#FFD700,stroke:#FFD700
```

---

## ⚙️ Core Modules

- **Middleware:** JWT authentication guards and request validation, including admin passphrase checks.
- **Models:** Mongoose schemas for users, products, orders, and messages.
- **Prescriptions:** Storage for prescription files uploaded during checkout.
- **Routes:** RESTful endpoints consumed by the client and admin dashboard.

---

## 🛠️ Technologies

<div align="center">

| Layer | Technologies |
|:------|:-------------|
| 🏃 **Runtime** | Node.js |
| ⚙️ **Framework** | Express.js |
| 🗄️ **Database** | MongoDB |
| 🔐 **Auth** | JWT (JSON Web Tokens), Admin Passphrase |
| 📤 **File Uploads** | Multer |
| 🐳 **Containerization** | Docker |

</div>

---

## 🚀 Getting Started

### Prerequisites

- Node.js (v16 or higher)
- Docker (optional, for containerized setup)

### Installation & Execution

**Step 1 — Clone the repository**

```bash
git clone https://github.com/NietoDeveloper/Pharmacy
```

**Step 2 — Navigate to the server directory**

```bash
cd server
```

**Step 3 — Install dependencies**

```bash
npm install
```

**Step 4 — Configure environment variables**

Create a `.env` file in the `server` directory with your MongoDB connection string, JWT secret, and admin passphrase.

**Step 5 — Start the server**

```bash
npm start
```

**Step 6 — (Optional) Run with Docker**

```bash
docker-compose up --build
```

Once the containers are up, the API is accessible on its configured port.

---

## 👨‍💻 Author

**Manuel Nieto (NietoDeveloper)**

---

## 📄 License

This project is licensed under the **MIT License**.

<div align="center">

<br/>

<img src="https://capsule-render.vercel.app/api?type=waving&color=gradient&customColorList=0,2,2,5,30&height=120&section=footer&animation=fadeIn" width="100%"/>

</div>
