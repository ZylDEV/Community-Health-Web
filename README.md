# Dashboard Admin Management (Firebase)

A simple **Admin Management Dashboard** built with **HTML, CSS, and JavaScript**, using **Firebase Realtime Database** and **Firebase Hosting**. Designed for internal/admin data management.

---

## Features

* CRUD Admin accounts (Create, Read, Update, Delete)
* Search admin by name
* Responsive layout (desktop & mobile)
* Email uniqueness validation
* Firebase Realtime Database integration
* Ready for Firebase Hosting

---

## Project Structure

```bash
HAJI/
├── public/
│   ├── index.html        # Login / landing page
│   ├── admin.html        # Admin management
│   ├── users.html        # User management
│   ├── jadwal.html       # Schedule
│   ├── rekammedis.html   # Medical records
│   └── statistik.html    # Statistics
├── firebase.json         # Firebase hosting config
├── .firebaserc           # Firebase project config
└── .gitignore            # Git ignore rules
```

---

## Tech Stack

* HTML5
* CSS3
* JavaScript (ES Modules)
* Firebase Realtime Database
* Firebase Hosting

---

## Firebase Setup

Firebase is initialized directly on the frontend:

```js
import { initializeApp } from "https://www.gstatic.com/firebasejs/10.12.0/firebase-app.js";
import { getDatabase } from "https://www.gstatic.com/firebasejs/10.12.0/firebase-database.js";

const firebaseConfig = {
  apiKey: "YOUR_API_KEY",
  authDomain: "YOUR_PROJECT.firebaseapp.com",
  databaseURL: "https://YOUR_PROJECT.firebaseio.com",
  projectId: "YOUR_PROJECT",
};

const app = initializeApp(firebaseConfig);
const db = getDatabase(app);
```

> Firebase API keys are public by design. Access control is handled via Firebase Rules.

---


## Run & Deploy

```bash
firebase login
firebase deploy
```