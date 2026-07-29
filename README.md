# StudyNation (Backend)

This is the **backend/API** for StudyNation — a full-stack EdTech platform I built where anyone can either **learn** by enrolling in courses, or **teach** by creating and selling their own.

This repo powers all the core logic: authentication, course management, payments, file uploads, and emails. The frontend (React) lives in a separate repo: **[StudyNation Frontend](https://github.com/your-username/studynation-frontend)**.

**Made by [Ashadullah Haneef](https://study-nation-frontend.vercel.app)**

---

## What does this backend actually do?

- **Auth** — signup/login with email OTP verification, JWT-based sessions, forgot/reset password
- **Courses** — create/edit/publish courses, sections & sub-sections, categories
- **Ratings & Reviews** — for courses
- **Course Progress** — tracks how far a student has gotten in a course
- **Payments** — Razorpay integration for course purchases
- **Profile** — update profile, change password, delete account, upload profile picture
- **File Uploads** — course thumbnails & videos stored on Cloudinary
- **Emails** — OTP, password reset, and contact form emails via Nodemailer
- **Contact Us** — handles messages from the frontend's contact form

---

## Tech Stack

- Node.js + Express
- MongoDB with Mongoose
- JWT for authentication
- Bcrypt for password hashing
- Nodemailer for sending emails
- Cloudinary for storing images/videos
- Razorpay for payment integration

---


---

## Getting Started

### 1. Clone the repo
```bash
git clone https://github.com/asahdullahhaneef/studynation-backend.git
cd studynation-backend
```

### 2. Install dependencies
```bash
npm install
```

### 3. Set up environment variables
Create a `.env` file in the root with:
```env
MAIL_HOST=your_smtp_host
MAIL_USER=your_email
MAIL_PASS=your_email_password

JWT_SECRET=your_jwt_secret
FOLDER_NAME=your_cloudinary_folder_name

RAZORPAY_KEY=your_razorpay_key
RAZORPAY_SECRET=your_razorpay_secret

CLOUD_NAME=your_cloudinary_cloud_name
API_KEY=your_cloudinary_api_key
API_SECRET=your_cloudinary_api_secret

MONGODB_URL=your_mongodb_connection_string
PORT=4000

FRONTEND_URL=http://localhost:3000
```

### 4. Run the server
```bash
npm run dev
```

The API should now be running at `(https://studynation-eso8.onrender.com/api/v1)` 
> This backend is meant to be used with the **[StudyNation Frontend](https://studynation-eso8.onrender.com/api/v1)** — make sure the frontend's `REACT_APP_BASE_URL` points to this server.

---

## A note on secrets

None of the actual API keys, database URLs, or Razorpay credentials are included in this repo — you'll need to generate your own (Mongo Atlas, Cloudinary, Razorpay, and an SMTP email) and plug them into the `.env` file as shown above.

---

## Feedback

If you spot a bug, have a suggestion, or just want to say hi — feel free to open an issue or reach out. Always happy to improve this further!

---

<p align="center">Built with ❤️ by Ashadullah Haneef</p>
