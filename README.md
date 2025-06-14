# Heavy Vehicles Management & Billing System

A modern, full-stack web application for managing transport operations — including drivers, trucks, and client billing — designed for logistics and transport businesses. This project streamlines operations, provides a professional dashboard, and ensures secure data management.

---

## 🚚 Overview

**Heavy Vehicles Management & Billing System** is a complete solution for transport and logistics companies to:
- Track and manage drivers and trucks
- Automate billing and mark payments
- Monitor maintenance schedules and pending alerts
- Provide a professional landing page for clients and staff

---

## ✨ Features

- **Landing Page:** Professional introduction, highlights, and contact form.
- **Authentication:** Secure login for authorized users (email/password via Firebase).
- **Dashboard:** Overview of key stats (drivers, trucks, pending bills, maintenance alerts).
- **Drivers Management:** Add, edit, delete, and list drivers (license, experience, status).
- **Trucks Management:** Manage fleet data (registration, insurance, maintenance).
- **Billing Management:** Create, edit, delete, and mark bills as paid; export bills to PDF.
- **Responsive UI:** Clean, modern design using Tailwind CSS.
- **Protected Routes:** Only authenticated users access management features.
- **Customizable:** Easily adapt styling, database logic, and authentication providers.

---

## 🖼️ Screenshots

> _Add images of your UI in the `project/screenshots/` folder for best presentation!_

- **Landing Page:**  
  ![Landing Page](./screenshots/landing.png)

- **Login:**  
  ![Login](./screenshots/login.png)

- **Dashboard:**  
  ![Dashboard](./screenshots/dashboard.png)

- **Drivers Management:**  
  ![Drivers Management](./screenshots/drivers.png)

- **Trucks Management:**  
  ![Trucks Management](./screenshots/trucks.png)

- **Billing Management:**  
  ![Billing Management](./screenshots/billing.png)

---

## 🛠️ Tech Stack

- **Frontend:** React, TypeScript, Vite
- **Styling:** Tailwind CSS
- **Routing:** React Router DOM
- **State/Context:** React Context API
- **Backend/Database:** Firebase Firestore (cloud database and authentication)
- **PDF Export:** react-to-pdf
- **Icons:** lucide-react

---

## 🚀 Getting Started

### Prerequisites

- Node.js (v16+ recommended)
- npm or yarn

### Installation

1. **Clone the repository:**
   ```bash
   git clone https://github.com/mr-black1304/Heavy-vehicles-Management-Billing--Public.git
   cd Heavy-vehicles-Management-Billing--Public/project
   ```

2. **Install dependencies:**
   ```bash
   npm install
   # or
   yarn install
   ```

3. **Configure Firebase:**
   - Create a Firebase project at [Firebase Console](https://console.firebase.google.com/).
   - Enable Authentication (Email/Password) and Firestore Database.
   - Copy your Firebase config and add it to `src/lib/firebase.ts`:
     ```typescript
     import { initializeApp } from "firebase/app";
     import { getFirestore } from "firebase/firestore";
     import { getAuth } from "firebase/auth";

     const firebaseConfig = {
       apiKey: "...",
       authDomain: "...",
       projectId: "...",
       storageBucket: "...",
       messagingSenderId: "...",
       appId: "..."
     };

     const app = initializeApp(firebaseConfig);
     export const db = getFirestore(app);
     export const auth = getAuth(app);
     ```

4. **Start the development server:**
   ```bash
   npm run dev
   # or
   yarn dev
   ```

5. **Open your browser:**
   - Visit [http://localhost:5173](http://localhost:5173)

---

## 📂 Project Structure

```
project/
├── src/
│   ├── components/    # Reusable UI components
│   ├── contexts/      # React authentication context
│   ├── lib/           # Firebase configuration
│   ├── pages/         # App pages (Dashboard, Drivers, Trucks, Billing, etc.)
│   ├── App.tsx        # Main app routing
│   └── main.tsx       # App entry point
├── public/            # Static assets
├── package.json       # Project metadata and scripts
├── tailwind.config.js # Tailwind CSS configuration
└── ...
```

---

## 🏃 Available Scripts

- `npm run dev` — Start the development server
- `npm run build` — Build for production
- `npm run preview` — Preview the production build
- `npm run lint` — Lint the codebase

---

## 🎨 Customization

- **Styling:** Modify Tailwind classes or the config file for custom themes.
- **Database:** Adjust Firestore collections/fields as needed for your business logic.
- **Authentication:** Extend with more providers (Google, etc.) via Firebase.

---

## 📜 License

This project is licensed under the MIT License.

---

## 🤝 Contributing

Contributions, suggestions, and improvements are welcome! Please open an issue or submit a pull request.

---
