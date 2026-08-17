<div align="center">

<img src="https://capsule-render.vercel.app/api?type=waving&color=gradient&customColorList=0,2,2,5,30&height=200&section=header&text=PHARMACY%20UI&fontSize=64&fontColor=FFD700&fontAlignY=42&desc=💊%20React%20%2B%20Vite%20%2B%20Tailwind%20CSS%20%C2%B7%20Dockerized%20Frontend&descAlignY=62&descColor=DCDCDC&animation=fadeIn" width="100%"/>

[![Typing SVG](https://readme-typing-svg.demolab.com?font=Share+Tech+Mono&weight=700&size=20&duration=2800&pause=900&color=FFD700&center=true&vCenter=true&width=760&lines=%F0%9F%92%8A+Browse+%26+Select+Pharmacy+Products;%F0%9F%8E%A8+Tailwind+CSS+Utility-First+Styling;%F0%9F%93%B1+Responsive%2C+Intuitive+UI;%F0%9F%90%B3+Containerized+for+Consistent+Deployment)](https://git.io/typing-svg)

<br/>

<p align="center">
  <a href="https://react.dev/">
    <img src="https://img.shields.io/badge/Frontend-React-61DAFB?style=for-the-badge&logo=react&logoColor=000"/>
  </a>
  <a href="https://nodejs.org/">
    <img src="https://img.shields.io/badge/Runtime-Node.js-339933?style=for-the-badge&logo=node.js&logoColor=white"/>
  </a>
  <a href="https://vitejs.dev/">
    <img src="https://img.shields.io/badge/Vite-Build_Tool-646CFF?style=for-the-badge&logo=vite&logoColor=white"/>
  </a>
  <a href="https://tailwindcss.com/">
    <img src="https://img.shields.io/badge/Tailwind_CSS-Styling-06B6D4?style=for-the-badge&logo=tailwindcss&logoColor=white"/>
  </a>
  <a href="https://www.docker.com/">
    <img src="https://img.shields.io/badge/Docker-Containerized-2496ED?style=for-the-badge&logo=docker&logoColor=white"/>
  </a>
  <a href="https://opensource.org/licenses/MIT">
    <img src="https://img.shields.io/badge/License-MIT-yellow.svg?style=for-the-badge"/>
  </a>
</p>

<p align="center">
  <a href="https://github.com/NietoDeveloper/Pharmacy/tree/main/ui">
    <img src="https://img.shields.io/badge/📂_Source-NietoDeveloper%2FPharmacy%2Fui-000000?style=for-the-badge&logo=github&logoColor=FFD700"/>
  </a>
</p>

</div>

---

## 📋 Overview

**Pharmacy UI** is the frontend of an application for managing pharmacy services. It provides a modern, responsive interface for users to interact with pharmacy-related features.

---

## 🗂️ Project Structure

```text
ui/
├── public/
└── src/
    ├── assets/
    │   └── images/
    ├── components/    # Reusable UI components
    ├── layouts/        # Page layout wrappers
    └── pages/           # Page-level components
```

---

## 🔄 UI Data Flow

```mermaid
flowchart LR
    A([👤 User]) -->|Browse| B[Pages]
    B --> C[Components]
    C -->|Layout Wrapping| D[Layouts]
    C -->|API Request| E([🔗 Pharmacy Backend])

    style A fill:#FFD700,color:#000,stroke:#FFD700
    style C fill:#06B6D4,color:#000,stroke:#06B6D4
    style E fill:#000,color:#FFD700,stroke:#FFD700
```

---

## 🛠️ Technologies

<div align="center">

| Technology | Role |
|:-----------|:-----|
| **Node.js** | Runtime environment |
| **React** | Frontend library for dynamic UI |
| **Vite** | Fast build tool for development |
| **Tailwind CSS** | Utility-first CSS framework |
| **Docker** | Containerization for consistent deployment |

</div>

---

## ✨ Features

- **Responsive and Intuitive User Interface:** Clean, mobile-friendly design.
- **Product Browsing and Selection:** Structured pharmacy product exploration.
- **Clean Design:** Styled entirely with Tailwind CSS.
- **Containerized Setup:** Easy, consistent deployment via Docker.

---

## 🚀 Installation

**Step 1 — Clone the repository**

```bash
git clone https://github.com/NietoDeveloper/Pharmacy
```

**Step 2 — Navigate to the project directory**

```bash
cd pharmacy-ui
```

**Step 3 — Install dependencies**

```bash
npm install
```

**Step 4 — Start the development server**

```bash
npm run dev
```

**Step 5 — (Optional) Build and run with Docker**

```bash
docker build -t pharmacy-ui .
docker run -p 5173:5173 pharmacy-ui
```

---

## 📖 Usage

- Access the app at `http://localhost:5173`.
- Browse pharmacy products and interact with the UI.
- Use Docker for consistent deployment across environments.

---

## 🤝 Contributing

Contributions are welcome! Fork the repository and submit a pull request.

---

## 👨‍💻 Author

Created by **Manuel Nieto (NietoSoftwareDeveloper)**.

<div align="center">

<br/>

<img src="https://capsule-render.vercel.app/api?type=waving&color=gradient&customColorList=0,2,2,5,30&height=120&section=footer&animation=fadeIn" width="100%"/>

</div>
