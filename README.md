# 📚 E-Library – Strapi Project Setup (README)

This project is a **Strapi-based E-Library CMS** created after cloning a GitHub repository and setting up the complete development environment using Node.js, Yarn, NPM, and VS Code. This README explains everything step‑by‑step in a professional and developer‑friendly format.

---

## 🚀 Project Overview

The **E-Library** project helps manage books and related metadata using Strapi’s powerful headless CMS features. It includes fields such as:

* **Book** (Short Text)
* **BookID** (UID)
* **BookTitle** (Short Text)
* **BookAuthor** (Short Text)
* Additional optional fields (cover image, status, publication year, etc.)

---

## 🛠️ Prerequisites

Before setting up the project, ensure the following tools are installed:

### ✔ Node.js (Recommended: v20 LTS)

Download from: [https://nodejs.org/](https://nodejs.org/)

### ✔ Git

Download from: [https://git-scm.com/](https://git-scm.com/)

### ✔ VS Code

Download from: [https://code.visualstudio.com/](https://code.visualstudio.com/)

### ✔ Yarn (Latest version via Corepack)

```bash
corepack enable
corepack prepare yarn@4.5.0 --activate
```

---

## 📥 Clone the GitHub Repository

Open PowerShell or VS Code terminal and run:

```bash
git clone <your-repository-url>
cd <project-folder>
```

---

## 📦 Install Dependencies

Run the following command inside the project folder:

```bash
yarn install
```

If you prefer npm:

```bash
npm install
```

---

## ▶️ Start the Strapi Development Server

To run your project locally:

```bash
yarn develop
```

Or with npm:

```bash
npm run develop
```

This will open the Strapi Admin panel at:

```
http://localhost:1337/admin
```

You will be asked to create a new **Strapi Admin Account**.

---

## 🧱 Creating the E-Library Collection Type

Inside Strapi Admin Panel:

### 1️⃣ Go to **Content-Type Builder**

### 2️⃣ Click **Create new Collection Type** → Enter name:

```
E-Library
```

### 3️⃣ Add the following fields:

#### **Book**

* Type: Text
* Description: Book category/label

#### **BookID**

* Type: UID
* Target Field: Book

#### **BookTitle**

* Type: Text
* Description: Name of the book

#### **BookAuthor**

* Type: Text
* Description: Author name

### 4️⃣ Click **Save** → Strapi will restart automatically.

---

## ✍️ Creating Your First Book Entry

### 1. Go to **E-Library** (Left Sidebar)

### 2. Click **Create New Entry**

### 3. Fill the details:

* Book: "A classic novel"
* BookID: "123"
* BookTitle: "Pride and Prejudice"
* BookAuthor: "Jane Austen"
* Status: "Published"

### 4. Click **Publish**

Your entry is now saved.

---

## 🔗 API Access

Strapi automatically generates APIs for your collection types.

### Get all books:

```
GET /api/e-libraries
```

### Get a single book by ID:

```
GET /api/e-libraries/:id
```

---

## 🧩 Optional Enhancements

You can add more fields such as:

* Cover Image (Media)
* Publication Year (Number)
* Genre (Text)
* Summary (Rich Text)
* Rating (Number)

---

## 📝 Conclusion

Your Strapi E-Library CMS is now fully set up and running. You can continue to expand your schema, connect a frontend (React, Next.js, Angular), or deploy it to Strapi Cloud, AWS, DigitalOcean, etc.

If you want, I can also generate:

* A **frontend UI** for your library
* **API documentation**
* **Deployment guide**

Just let me know! 🚀
