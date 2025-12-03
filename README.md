📚 E-Library – Strapi Project Setup

This project is a Strapi-based E-Library CMS created after cloning a GitHub repository and setting up the complete development environment using Node.js, Yarn, NPM, and VS Code. This README explains everything step‑by‑step in a professional and developer‑friendly format.

🚀 Project Overview

The E-Library project helps manage books and related metadata using Strapi’s powerful headless CMS features. It includes fields such as:

Book (Short Text)

BookID (UID)

BookTitle (Short Text)

BookAuthor (Short Text)

Additional optional fields (cover image, status, publication year, etc.)

🛠️ Prerequisites

Before setting up the project, ensure the following tools are installed:

✔ Node.js (Recommended: v20 LTS)

Download from: https://nodejs.org/

✔ Git

Download from: https://git-scm.com/

✔ VS Code

Download from: https://code.visualstudio.com/

✔ Yarn (Latest version via Corepack)
corepack enable
corepack prepare yarn@4.5.0 --activate

📥 Clone the GitHub Repository
git clone <your-repository-url>
cd <project-folder>

📦 Install Dependencies
yarn install
# or
npm install

▶️ Start the Strapi Development Server
yarn develop
# or
npm run develop


Admin panel: http://localhost:1337/admin
Create your Strapi Admin Account when prompted.

🧱 Creating the E-Library Collection Type

Go to Content-Type Builder

Click Create new Collection Type → E-Library

Add fields:

Field	Type	Description
Book	Text	Book category/label
BookID	UID	Unique ID linked to Book
BookTitle	Text	Name of the book
BookAuthor	Text	Author of the book

Click Save → Strapi restarts automatically.

✍️ Creating Your First Book Entry

Go to E-Library in the sidebar

Click Create New Entry

Fill details:

Book: "A classic novel"
BookID: "123"
BookTitle: "Pride and Prejudice"
BookAuthor: "Jane Austen"
Status: "Published"


Click Publish ✅

🔗 API Access

Get all books: GET /api/e-libraries

Get a single book by ID: GET /api/e-libraries/:id

🧩 Optional Enhancements

Cover Image (Media)

Publication Year (Number)

Genre (Text)

Summary (Rich Text)

Rating (Number)

📝 Conclusion

Your Strapi E-Library CMS is fully set up. You can now expand your schema, connect a frontend, or deploy to cloud platforms.

Welcome to PearlThoughts—let's embark on this journey together!