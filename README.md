<div align="center">

<img src="https://capsule-render.vercel.app/api?type=waving&color=gradient&customColorList=0,2,2,5,30&height=220&section=header&text=PHARMACY&fontSize=80&fontColor=FFD700&fontAlignY=42&desc=💊%20Online%20Pharmacy%20%C2%B7%20MERN%20Stack%20%C2%B7%20Dockerized&descAlignY=62&descColor=DCDCDC&animation=fadeIn" width="100%"/>

[![Typing SVG](https://readme-typing-svg.demolab.com?font=Share+Tech+Mono&weight=700&size=20&duration=2800&pause=900&color=FFD700&center=true&vCenter=true&width=760&lines=%F0%9F%92%8A+Browse+%26+Buy+Medications+Online;%F0%9F%A7%BE+Prescription+Upload+at+Checkout;%F0%9F%94%92+JWT+Auth+%2B+Admin+Passphrase;%F0%9F%90%B3+Fully+Dockerized+%C2%B7+MERN+Stack;%F0%9F%8F%86+%231+GitHub+Committer+in+Colombia)](https://git.io/typing-svg)

<br/>

<p align="center">
  <a href="https://github.com/NietoDeveloper">
    <img src="https://img.shields.io/badge/Engineer-Manuel%20Nieto-blue?style=for-the-badge&logo=github"/>
  </a>
  <a href="https://committers.top/colombia#NietoDeveloper">
    <img src="https://img.shields.io/badge/Committers.top-%231%20Colombia-gold?style=for-the-badge"/>
  </a>
  <a href="https://react.dev/">
    <img src="https://img.shields.io/badge/Frontend-React-61DAFB?style=for-the-badge&logo=react&logoColor=000"/>
  </a>
  <a href="https://nodejs.org/">
    <img src="https://img.shields.io/badge/Backend-Node.js-339933?style=for-the-badge&logo=node.js&logoColor=white"/>
  </a>
  <a href="https://www.mongodb.com/">
    <img src="https://img.shields.io/badge/Database-MongoDB-47A248?style=for-the-badge&logo=mongodb&logoColor=white"/>
  </a>
  <a href="https://www.docker.com/">
    <img src="https://img.shields.io/badge/Docker-Compose-2496ED?style=for-the-badge&logo=docker&logoColor=white"/>
  </a>
  <a href="https://opensource.org/licenses/MIT">
    <img src="https://img.shields.io/badge/License-MIT-yellow.svg?style=for-the-badge"/>
  </a>
</p>

<p align="center">
  <a href="https://github.com/NietoDeveloper/Pharmacy">
    <img src="https://img.shields.io/badge/📂_Source-NietoDeveloper%2FPharmacy-000000?style=for-the-badge&logo=github&logoColor=FFD700"/>
  </a>
</p>

</div>

---

## 📋 Overview

The **Online Pharmacy Web App** enables users to digitally explore and buy medications. Developed using the **MERN stack** (MongoDB, Express.js, React, Node.js) and **Docker** for containerization, it ensures a smooth user experience for account management, order placement, and support communication. Admins handle product, prescription, and message oversight, with access secured by a unique admin passphrase.

---

## 🔄 Order & Prescription Flow

```mermaid
flowchart LR
    A([👤 User]) -->|Browse| B[Product Page]
    B -->|Add to Cart| C[Cart Management]
    C -->|Checkout| D[Upload Prescription]
    D -->|JWT Validated| E[Node.js API]
    E -->|Persist| F[(MongoDB\nOrders / Prescriptions)]
    F -->|Review| G[🔒 Admin Dashboard]
    G -->|Approve / Manage| H([✅ Order Processed])

    style A fill:#FFD700,color:#000,stroke:#FFD700
    style E fill:#0a0a0a,color:#FFD700,stroke:#FFD700
    style F fill:#47A248,color:#fff,stroke:#47A248
    style G fill:#000,color:#FFD700,stroke:#FFD700
```

---

## 🔑 Features

### 👤 User

- **Login & Signup:** Secure user authentication.
- **Home:** Product information is accessible even without signup.
- **🛒 Product Page:** Each medicine has a dedicated page with details such as name, description, price, and available stock.
- **🛍️ Cart Management:** Users can add, edit, or delete products in their cart.
- **📞 Contact Us:** A messaging system for user inquiries.
- **📝 Checkout:** A page for uploading prescriptions.
- **🚪 Logout:** End the session securely.

### 🔒 Admin

- **Admin Authentication:** Secure login through an admin passphrase.
- **📊 Dashboard:** Manage products (add, edit, delete).
- **📩 Message Management:** Access messages from users.
- **🧾 Prescription Management:** Review uploaded prescriptions during checkout.
- **🚪 Logout:** End the session securely.

---

## 🛠️ Technologies Used

<div align="center">

| Layer | Technologies |
|:------|:-------------|
| 🎨 **Frontend** | React.js |
| ⚙️ **Backend** | Node.js, Express.js |
| 🗄️ **Database** | MongoDB |
| 🐳 **Containerization** | Docker |

</div>

---

## 🧰 Other Tools

- **Multer:** Handles prescription uploads.
- **JWT (JSON Web Tokens):** Secures user authentication and manages sessions.

---

## 🚀 Getting Started

**Step 1 — Clone the repository**

```bash
git clone https://github.com/NietoDeveloper/Pharmacy
```

**Step 2 — Docker setup**

```bash
docker-compose up --build
```

**Step 3 — Access the application**

Once the containers are up, visit `localhost:3001` to access the app.

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
