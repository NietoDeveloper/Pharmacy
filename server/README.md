<div align="center">

<img src="https://capsule-render.vercel.app/api?type=waving&color=gradient&customColorList=0,2,2,5,30&height=200&section=header&text=PHARMACY%20%E2%80%94%20SERVER&fontSize=56&fontColor=FFD700&fontAlignY=42&desc=⚡%20Node.js%20REST%20API%20%C2%B7%20Prescriptions%20%26%20Orders%20%C2%B7%20Dockerized&descAlignY=62&descColor=DCDCDC&animation=fadeIn" width="100%"/>

[![Typing SVG](https://readme-typing-svg.demolab.com?font=Share+Tech+Mono&weight=700&size=20&duration=2800&pause=900&color=FFD700&center=true&vCenter=true&width=760&lines=%E2%9A%A1+RESTful+API+for+Products+%26+Orders;%F0%9F%A7%BE+Prescription+Upload+Handling;%F0%9F%94%92+JWT+Auth+%2B+Admin+Passphrase;%F0%9F%90%B3+Fully+Dockerized+Backend)](https://git.io/typing-svg)

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

The **server** for the Pharmacy application. Built with **Node.js**, it exposes a RESTful API handling product, order, and user management, secured with JWT authentication and an admin passphrase, with dedicated support for prescription uploads.

---

## 🗂️ Project Structure

```text
server/
├── middleware/       # Auth guards, request validation, error handling
├── models/            # Database schemas (products, users, orders)
├── prescriptions/       # Uploaded prescription storage
└── routes/               # RESTful API endpoint definitions
```

---

## 🔄 Prescription & Order Flow

```mermaid
flowchart LR
    A([👤 User]) -->|Checkout| B[Routes]
    B --> C[Middleware]
    C -->|Auth Check| D{JWT Valid?}
    D -->|Yes| E[Controller Logic]
    D -->|No| F[401 · Unauthorized]
    E -->|Store File| G[prescriptions/]
    E -->|Persist| H[(Models\nMongoDB)]
    H -->|Review| I[🔒 Admin Dashboard]

    style A fill:#FFD700,color:#000,stroke:#FFD700
    style E fill:#0a0a0a,color:#FFD700,stroke:#FFD700
    style F fill:#FF0000,color:#fff
    style H fill:#47A248,color:#fff,stroke:#47A248
    style I fill:#000,color:#FFD700,stroke:#FFD700
```

---

## ⚙️ Core Modules

- **Middleware:** Handles authentication guards, request validation, and error handling.
- **Models:** Define data structures for products, users, and orders.
- **Prescriptions:** Storage for prescription files uploaded during checkout.
- **Routes:** Expose RESTful endpoints consumed by the Pharmacy UI.

---

## 🛠️ Technologies

<div align="center">

| Layer | Technologies |
|:------|:-------------|
| 🏃 **Runtime** | Node.js |
| ⚙️ **Framework** | Express.js |
| 🗄️ **Database** | MongoDB |
| 🐳 **Containerization** | Docker |

</div>

---

## 🧰 Other Tools

- **Multer:** Handles prescription file uploads.
- **JWT (JSON Web Tokens):** Secures user authentication and manages sessions.

---

## 🚀 Getting Started

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

Create a `.env` file with your MongoDB connection string, JWT secret, and admin passphrase.

**Step 5 — Start the server**

```bash
npm start
```

**Step 6 — (Optional) Run with Docker**

```bash
docker-compose up --build
```

Once the containers are up, the API is available at `localhost:3001` (or as configured).

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








































<div align="center">

<img src="https://capsule-render.vercel.app/api?type=waving&color=gradient&customColorList=0,2,2,5,30&height=200&section=header&text=PHARMACY%20%E2%80%94%20SERVER&fontSize=56&fontColor=FFD700&fontAlignY=42&desc=⚡%20Node.js%20REST%20API%20%C2%B7%20Prescriptions%20%26%20Orders%20%C2%B7%20Dockerized&descAlignY=62&descColor=DCDCDC&animation=fadeIn" width="100%"/>

[![Typing SVG](https://readme-typing-svg.demolab.com?font=Share+Tech+Mono&weight=700&size=20&duration=2800&pause=900&color=FFD700&center=true&vCenter=true&width=760&lines=%E2%9A%A1+RESTful+API+for+Products+%26+Orders;%F0%9F%A7%BE+Prescription+Upload+Handling;%F0%9F%94%92+JWT+Auth+%2B+Admin+Passphrase;%F0%9F%90%B3+Fully+Dockerized+Backend)](https://git.io/typing-svg)

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

The **server** for the Pharmacy application. Built with **Node.js**, it exposes a RESTful API handling product, order, and user management, secured with JWT authentication and an admin passphrase, with dedicated support for prescription uploads.

---

## 🗂️ Project Structure

```text
server/
├── middleware/       # Auth guards, request validation, error handling
├── models/            # Database schemas (products, users, orders)
├── prescriptions/       # Uploaded prescription storage
└── routes/               # RESTful API endpoint definitions
```

---

## 🔄 Prescription & Order Flow

```mermaid
flowchart LR
    A([👤 User]) -->|Checkout| B[Routes]
    B --> C[Middleware]
    C -->|Auth Check| D{JWT Valid?}
    D -->|Yes| E[Controller Logic]
    D -->|No| F[401 · Unauthorized]
    E -->|Store File| G[prescriptions/]
    E -->|Persist| H[(Models\nMongoDB)]
    H -->|Review| I[🔒 Admin Dashboard]

    style A fill:#FFD700,color:#000,stroke:#FFD700
    style E fill:#0a0a0a,color:#FFD700,stroke:#FFD700
    style F fill:#FF0000,color:#fff
    style H fill:#47A248,color:#fff,stroke:#47A248
    style I fill:#000,color:#FFD700,stroke:#FFD700
```

---

## ⚙️ Core Modules

- **Middleware:** Handles authentication guards, request validation, and error handling.
- **Models:** Define data structures for products, users, and orders.
- **Prescriptions:** Storage for prescription files uploaded during checkout.
- **Routes:** Expose RESTful endpoints consumed by the 