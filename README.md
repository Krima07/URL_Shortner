# 🔗 URL Shortener

A full-stack URL Shortener web application built using **Next.js**, **JavaScript**, **MongoDB**, and **Tailwind CSS**. This project allows users to convert long URLs into concise, shareable links with automatic redirection support.

---

## 📌 Features

- 🔍 **URL shortening** — Quickly convert long URLs to short, unique identifiers.
- 📁 **MongoDB integration** — All URL data is persisted in a NoSQL database.
- 🔁 **Redirection** — Accessing a short URL automatically redirects to the original.
- ❌ **Duplicate prevention** — Prevents generation of duplicate short URLs.
- 🎨 **Responsive design** — Built with Tailwind CSS for modern styling.
- 🧠 **Error handling** — Handles invalid input, server errors, and missing URLs gracefully.

---

## 🛠️ Tech Stack

- **Frontend**: Next.js (App Router), React, JavaScript, Tailwind CSS  
- **Backend**: Next.js API Routes, MongoDB (via MongoDB Node.js client)  
- **Database**: MongoDB Atlas (cloud-hosted)  
- **Deployment**: Vercel (or any Next.js-compatible host)

---

##🗂 Project Structure

``` plaintext
/
├── app/                # App routes (Next.js 13+)
│   ├── page.jsx        # Home page
│   └── [slug]/route.js # API redirect logic
├── lib/                # MongoDB client connection
├── styles/             # Tailwind styles
├── public/             # Static assets
├── .env.local          # Environment variables
├── tailwind.config.js  # Tailwind config
└── package.json        # Project metadata
```
---
##⚙️ How It Works
1.The user submits a long URL via the input form.

2.An API route checks if the URL already exists in the database.

3.If new, a unique short path is generated and stored in MongoDB.

4.The generated short URL is displayed to the user.

5.When a short URL is visited, it triggers a redirect based on database lookup.

---
##📦 Future Improvements
-🔐 Add authentication for user-specific URL management

-📊 Add click tracking analytics

-⏳ Set expiration dates for short links

-🛡️ Add rate limiting and validation for better security

---
##📄 License
This project is open-source and available under the MIT License.


