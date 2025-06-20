# 🧠 DevLog – A Software Development Blog (Next.js + MongoDB)

A modern blog application tailored for software development content. Built with **Next.js** for performance and SEO, and **MongoDB** for flexible content storage. Ideal for developers sharing tutorials, articles, and engineering insights.

---

## 🎯 Objectives

- Share developer insights, guides, and tutorials in a clean, structured format.
- Provide an intuitive interface for writing and managing blog posts.
- Deliver high performance, SEO-optimized pages with scalable backend logic.
- Embrace full-stack development best practices with modern tools.

---

## 🛠 Tech Stack

### Frontend:
- **Next.js 14** – Full-stack React framework
- **TypeScript** – Type safety and clean architecture
- **Tailwind CSS** – Rapid UI development
- **Markdown / MDX** – Rich content formatting

### Backend:
- **Next.js API Routes** – Built-in backend support
- **Mongoose** – MongoDB ODM for schema modeling
- **JWT** – Authentication & session management

### Database:
- **MongoDB Atlas** – Cloud-hosted NoSQL database

---

## 🗂 Database Design

**Users Collection**
| Field      | Type     | Description                |
|------------|----------|----------------------------|
| _id        | ObjectId | Primary key                |
| name       | String   | Author's full name         |
| email      | String   | Unique user email          |
| password   | String   | Hashed password            |
| role       | String   | 'admin' or 'user'          |
| createdAt  | Date     | Registration timestamp     |

**Posts Collection**
| Field      | Type     | Description                |
|------------|----------|----------------------------|
| _id        | ObjectId | Primary key                |
| title      | String   | Title of the blog post     |
| slug       | String   | URL-friendly identifier    |
| content    | String   | Markdown-formatted content |
| authorId   | ObjectId | Ref → Users._id            |
| tags       | [String] | Technology tags (e.g. JS)  |
| published  | Boolean  | Visibility flag            |
| createdAt  | Date     | Created timestamp          |
| updatedAt  | Date     | Last modified              |

---

✨ Features
🔐 Authentication – Signup, login, JWT tokens

✍️ Markdown Support – Developer-friendly writing experience

🧑‍💻 Author Dashboard – Create, edit, delete posts

🌍 Public Blog Feed – View published articles

🧭 Dynamic Routing – Slug-based post URLs

🔍 SEO Ready – Meta tags, Open Graph, sitemap

📱 Responsive UI – Mobile-first design

🏷 Tags & Filtering – Find posts by tech stack

---

## ✅ Testing

- **Jest** – Unit and integration testing
- **React Testing Library** – UI interaction testing
- **Supertest** – API testing
- **MongoMemoryServer** – In-memory MongoDB for isolated tests

```bash
npm run test

---

## 🚀 Deployment

Recommended: **Vercel + MongoDB Atlas**

### Vercel Deployment Steps
1. Push your code to GitHub
2. Go to [https://vercel.com](https://vercel.com)
3. Import your repo
4. Add these environment variables:

---

📌 Future Enhancements
🔁 Social login (GitHub, Google)

📊 Post analytics (views, likes)

💬 Comments with moderation

🧑‍🤝‍🧑 Multi-author support

🌙 Dark mode

---

🧑 Author
Built with ❤️ by Elaine



