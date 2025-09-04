
# 🔐 Secure File Sharing System

A **full-stack web application** that enables users to securely upload files, generate unique shareable links, and set expiration times for controlled access. The system emphasizes **backend security**, featuring authentication, encrypted file storage, and API-driven architecture, with a minimal frontend for interaction.

---

## 🚀 Features

* 🔑 **User Authentication** – Secure login & signup with JWT
* 📤 **File Upload** – Upload multiple file types
* 🔗 **Shareable Links** – Auto-generated with expiry time
* 🛡️ **Encrypted Storage** – Files are stored securely (optional AES encryption)
* 📥 **Secure Downloads** – Access controlled by link validity & expiry
* 🗄️ **Database Integration** – Tracks users, files, and link metadata
* 🌐 **Frontend Interface** – Simple upload/download UI

---

## 🏗️ Tech Stack

**Frontend:**

* React.js (Vercel/Netlify deployment)
* Tailwind CSS (styling)

**Backend:**

* Node.js + Express.js
* Multer (file handling)
* JWT (authentication)
* Crypto (encryption/decryption)

**Database:**

* MongoDB Atlas (NoSQL cloud database)

**Storage:**

* Local server storage (development)
* AWS S3 (optional for production)

---

## ⚙️ Installation & Setup

### 1️⃣ Clone the Repository

```bash
git clone https://github.com/your-username/secure-file-sharing-system.git
cd secure-file-sharing-system
```

### 2️⃣ Backend Setup

```bash
cd backend
npm install
```

Create a `.env` file inside `backend/` with:

```
PORT=5000
MONGO_URI=your_mongodb_atlas_connection_string
JWT_SECRET=your_secret_key
FILE_STORAGE=uploads/
```

Start backend server:

```bash
npm start
```

### 3️⃣ Frontend Setup

```bash
cd frontend
npm install
npm start
```

---

## 🔗 API Endpoints

### Auth Routes

* `POST /api/auth/signup` → Register new user
* `POST /api/auth/login` → Authenticate & get token

### File Routes

* `POST /api/files/upload` → Upload a file
* `GET /api/files/:id` → Download a file

### Link Routes

* `POST /api/links/create` → Generate shareable link with expiry
* `GET /api/links/:id` → Access file via link

---

## 🚀 Deployment

* **Backend:** Render / Railway
* **Frontend:** Vercel / Netlify
* **Database:** MongoDB Atlas
* **Storage:** AWS S3 (optional, for production)
---

## 👩‍💻 Author

Developed by **\Pallawi Hansdak** ✨

---

👉 Do you want me to also include a **project architecture diagram (workflow)** inside the README (in markdown with ASCII/mermaid) so it’s visually clear for your teacher?
