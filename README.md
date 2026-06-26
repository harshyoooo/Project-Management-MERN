# 🚀 TaskForge

A modern **Project Management System** built using the **PERN Stack** (PostgreSQL, Express.js, React.js, Node.js). TaskForge enables teams to collaborate efficiently by organizing workspaces, managing projects, assigning tasks, tracking progress, and working together in a secure environment.

The application integrates **Clerk** for authentication and organization management, **Inngest** for event-driven synchronization, **Prisma ORM** for database operations, and **Neon PostgreSQL** for cloud-hosted data storage.

---

## 🌐 Live Demo

🔗 **https://taskforgefrontend.vercel.app/**

---

# ✨ Features

* 🏢 **Multiple Workspaces**

  * Create and manage multiple workspaces independently.
  * Each workspace contains its own projects, tasks, and team members.

* 📁 **Project Management**

  * Create, update, and organize projects.
  * Track project progress, status, and priority.
  * Assign project leads and manage project members.

* ✅ **Task Management**

  * Create and assign tasks to team members.
  * Set deadlines and priorities.
  * Track task status from planning to completion.
  * Add comments for better collaboration.

* 👥 **User & Team Management**

  * Invite members to workspaces.
  * Manage workspace roles (Admin / Member).
  * Add project-specific members.
  * View project teams and workspace members.

* 📊 **Analytics Dashboard**

  * Track completed projects.
  * Monitor overdue tasks.
  * View personal assigned tasks.
  * Analyze project progress and workspace activity.

* 🔐 **Secure Authentication**

  * User authentication powered by Clerk.
  * Organization-based access control.
  * Protected API routes.

* ⚡ **Event-Driven Synchronization**

  * Automatic synchronization of users.
  * Workspace synchronization.
  * Membership synchronization.
  * Powered by Inngest event functions.

* 🌙 **Modern User Experience**

  * Responsive design.
  * Dark mode support.
  * Clean dashboard interface.
  * Toast notifications.

---

# 🛠 Tech Stack

### Frontend

* React.js
* Redux Toolkit
* React Router DOM
* Tailwind CSS
* Axios
* React Hot Toast
* Lucide React

### Backend

* Node.js
* Express.js

### Database

* PostgreSQL
* Prisma ORM
* Neon Database

### Authentication

* Clerk Authentication
* Clerk Organizations

### Event Processing

* Inngest

### Deployment

* Vercel

---

# 📂 Project Structure

```
TaskForge
│
├── project-management
│   ├── src
│   ├── public
│   └── ...
│
├── server
│   ├── configs
│   ├── controllers
│   ├── middleware
│   ├── prisma
│   ├── routes
│   ├── inngest
│   └── ...
│
└── README.md
```

---

# 🚀 Getting Started

## Clone the Repository

```bash
git clone https://github.com/harshyoooo/Project-Management-MERN.git

```

---

## Install Dependencies

### project-management

```bash
cd project-management
npm install
```

### Server

```bash
cd server
npm install
```

---

# 🔑 Environment Variables

## Client (.env)

```env
VITE_API_URL=

VITE_CLERK_PUBLISHABLE_KEY=
```

---

## Server (.env)

```env
DATABASE_URL=

CLERK_SECRET_KEY=

CLERK_WEBHOOK_SECRET=

INNGEST_EVENT_KEY=

INNGEST_SIGNING_KEY=
```

---

# ⚙️ Setup

## 1. PostgreSQL Database

Create a PostgreSQL database using **Neon** (or any PostgreSQL provider).

Update

```env
DATABASE_URL=
```

Generate Prisma Client

```bash
npx prisma generate
```

Run Migrations

```bash
npx prisma migrate dev
```

---

## 2. Clerk

Create a project on Clerk.

Copy the following credentials:

* Publishable Key
* Secret Key
* Webhook Secret

Enable **Organizations** in the Clerk Dashboard.

Paste the keys into your environment variables.

---

## 3. Inngest

Create an account on Inngest.

Create a new application.

Copy:

* Event Key
* Signing Key

Add them to your backend `.env`.

Start the Inngest development server:

```bash
npx inngest-cli@latest dev
```

Inngest automatically synchronizes users, organizations, and workspace memberships between Clerk and PostgreSQL.

---

# ▶️ Run the Application

## Backend

```bash
cd server

npm run start
```

---

## Frontend

```bash
cd project-management

npm run dev
```

---

# 🚀 Deployment

The frontend is deployed using **Vercel**.

For production deployment:

* Deploy the frontend to Vercel.
* Deploy the backend to your preferred Node.js hosting provider.
* Configure all environment variables.
* Update the frontend API URL.
* Configure Clerk production keys.
* Configure Inngest production keys.

---

# 👨‍💻 Author

**Harsh Bhosale**

Feel free to connect or contribute to the project!

---

## ⭐ Support

If you found this project helpful, consider giving it a ⭐ on GitHub. It helps others discover the project and motivates future development.
