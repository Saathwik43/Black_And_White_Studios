# Black & White Studios — StudioGallery

A premium photography portfolio website and staff upload backend created for **Black and White Stories** (Photography Studio, Hyderabad). It features public-facing event galleries, a responsive lightbox, automated WhatsApp inquiries, and a login-protected admin panel for uploading and managing gallery images.

🔗 **Live Website:** [black-and-white-studios-fe.onrender.com](https://black-and-white-studios-fe.onrender.com)

---

## 🛠️ Technology Stack

| Layer | Technology |
| :--- | :--- |
| **Frontend** | React (Vite), TailwindCSS, React Router, Lucide Icons |
| **Backend** | Node.js, Express, Mongoose (MongoDB) |
| **Storage** | Cloudinary (for compressed image hosting) |
| **Authentication** | JSON Web Tokens (JWT) & BcryptJS |

---

## 🚀 Getting Started & Running the Project

You can run both the frontend and backend concurrently from the root directory using a single command.

### 1. Prerequisites
Ensure you have **Node.js** (v16+) and **npm** installed on your system.

### 2. Configure Environment Variables
Create a `.env` file inside the `backend/` directory:
```env
PORT=5000
MONGO_URI=your_mongodb_connection_string
JWT_SECRET=your_jwt_secret_key
CLOUDINARY_CLOUD_NAME=your_cloudinary_name
CLOUDINARY_API_KEY=your_cloudinary_key
CLOUDINARY_API_SECRET=your_cloudinary_secret
```

### 3. Installation
Install dependencies for both the frontend and backend at once from the root directory:
```bash
npm run install:all
```

### 4. Running the Application
To run the frontend and backend servers concurrently:
```bash
npm run dev
```

This command will automatically:
* Start the **Backend Server** (runs on `http://localhost:5000` or the configured `PORT`)
* Start the **Frontend Dev Server** (runs on `http://localhost:5173`)

#### Individual Scripts
If you want to run them separately from the root directory:
* Run only the Backend: `npm run backend`
* Run only the Frontend: `npm run frontend`

---

## 📁 Directory Structure

```text
├── backend/               # Node/Express API, database models, and routes
├── frontend/              # React/Vite/Tailwind frontend client
├── package.json           # Root package file orchestrating scripts
├── requirements_checklist.md # Client requirements checklist
└── README.md              # Project documentation
```

---

## 🖼️ Features & Checklist Status

### 🏠 Public Site
- [x] **Home Page:** Prominent studio branding, hero banner, intro text, and WhatsApp CTA.
- [x] **Event Galleries:** Interactive masonry/grid layout for categories (Weddings, Portraits, Corporate, etc.).
- [x] **Lightbox:** Mobile-responsive full-screen preview with previous/next image navigation.
- [x] **WhatsApp Inquiry:** "Inquire for this event type" button pre-filling text template based on the current gallery.
- [x] **Contact Page:** Functional contact form that redirects to WhatsApp with filled details.

### 🔐 Admin Panel (Staff Upload)
- [x] **Secure Login:** Protected dashboard using JWT auth.
- [x] **Image Upload:** Upload interface (file picker/drag-and-drop) with automated compression.
- [x] **Image Management:** Delete existing images from active galleries.
- [x] **Category Management:** Ability to dynamically add/remove new event categories.
