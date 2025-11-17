# 📘 SafeSpace Admin Web

Comprehensive admin dashboard and management platform for SafeSpace healthcare services.

## 📑 Table of Contents

- [About the Project](#-about-the-project)
- [Features](#-features)
- [Tech Stack](#-tech-stack)
- [Project Structure](#-project-structure)
- [Installation](#️-installation)
- [Usage](#️-usage)
- [API Endpoints](#-api-endpoints-optional)
- [Screenshots](#-screenshots)
- [Environment Variables](#-environment-variables)
- [Contributing](#-contributing)
- [License](#-license)
- [Contact](#contact)

## 📖 About the Project

SafeSpace Admin Web is a modern, secure admin dashboard built to manage users, doctors, entertainment content, and analytics for the SafeSpace healthcare platform. It provides administrators with powerful tools to:

* Manage user accounts and roles
* Oversee doctor profiles and availability
* Monitor entertainment content
* Track analytics and generate reports
* Ensure data security and authentication

Built with React, TypeScript, and Supabase for real-time data management and enterprise-grade security.

This admin web is part of the SafeSpace platform ecosystem, which includes:

- **SafeSpace Main App**: [https://github.com/DhanukaRathnayaka/Final_Year_Project.git](https://github.com/DhanukaRathnayaka/Final_Year_Project.git)
- **SafeSpace Doctor App**: [https://github.com/SarithDedunu/safespace-doctor-app.git](https://github.com/SarithDedunu/safespace-doctor-app.git)

## ⭐ Features

* **User Management** - Create, update, and manage user accounts with role-based access control
* **Doctor Management** - Oversee doctor profiles, credentials, and availability
* **Entertainment Module** - Manage and moderate entertainment content
* **Admin Dashboard** - View comprehensive analytics and system metrics
* **Reports Generation** - Create and export detailed reports
* **Real-time Authentication** - Secure login and session management
* **Responsive Design** - Mobile-friendly admin interface
* **Role-Based Access Control** - Different permission levels for admin users

## 🛠 Tech Stack

* **Frontend:** React 18+, TypeScript, Tailwind CSS, Vite
* **Runtime:** Node.js v23.5.0
* **State Management:** Zustand
* **Backend/Database:** Supabase (PostgreSQL)
* **Authentication:** JWT-based with Supabase Auth
* **API Communication:** RESTful APIs
* **Build Tools:** Vite, PostCSS, ESLint
* **Deployment:** Vercel
* **Version Control:** Git

## 📂 Project Structure

```
safespace-admin_web/
├── src/
│   ├── components/          # Reusable UI components
│   │   ├── Layout.tsx
│   │   ├── Navbar.tsx
│   │   ├── Sidebar.tsx
│   │   └── TestConnection.tsx
│   ├── pages/              # Page components
│   │   ├── Dashboard.tsx
│   │   ├── AdminManagement.tsx
│   │   ├── Doctors.tsx
│   │   ├── Users.tsx
│   │   ├── Analytics.tsx
│   │   ├── Entertainment.tsx
│   │   ├── Reports.tsx
│   │   ├── Login.tsx
│   │   └── AdminProfile.tsx
│   ├── lib/                # Services and utilities
│   │   ├── supabase.ts
│   │   ├── authService.ts
│   │   ├── adminService.ts
│   │   ├── userService.ts
│   │   └── entertainmentService.ts
│   ├── providers/          # Context providers
│   │   ├── AuthContext.ts
│   │   └── AuthProvider.tsx
│   ├── store/              # State management (Zustand)
│   │   ├── authStore.ts
│   │   └── adminStore.ts
│   ├── types/              # TypeScript type definitions
│   │   └── supabase.ts
│   ├── App.tsx
│   ├── main.tsx
│   └── index.css
├── public/                 # Static assets
├── supabase/              # Supabase migrations
├── package.json
├── vite.config.ts
├── tsconfig.json
├── tailwind.config.cjs
└── README.md
```

## ⚙️ Installation

1️⃣ Clone the repository
```bash
git clone https://github.com/GayangaBandara/safespace-admin_web.git
cd safespace-admin_web
```

2️⃣ Install dependencies
```bash
npm install
```

3️⃣ Set up environment variables

Create a `.env.local` file in the root directory:
```
VITE_SUPABASE_URL=your_supabase_url
VITE_SUPABASE_ANON_KEY=your_supabase_anon_key
```

4️⃣ Start the development server
```bash
npm run dev
```

The application will be available at `http://localhost:5173`

## ▶️ Usage

**Development Mode**
```bash
npm run dev
```

**Build for Production**
```bash
npm run build
```

**Preview Production Build**
```bash
npm run preview
```

**Lint Code**
```bash
npm run lint
```

### Key Features Usage

* **Login** - Access the admin panel using your credentials
* **Dashboard** - View system overview and key metrics
* **Manage Users** - Create, update, and delete user accounts
* **Manage Doctors** - Handle doctor profiles and specializations
* **Entertainment** - Moderate and manage entertainment content
* **Analytics** - View detailed analytics and reports

## 📡 API Endpoints

The admin web communicates with Supabase services. Key endpoints include:

| Service      | Method | Endpoint              | Description               |
| ------------ | ------ | --------------------- | ------------------------- |
| Auth         | POST   | /auth/v1/token        | Authenticate user         |
| Users        | GET    | /users                | Fetch all users           |
| Users        | POST   | /users                | Create new user           |
| Doctors      | GET    | /doctors              | Fetch all doctors         |
| Doctors      | POST   | /doctors              | Create new doctor         |
| Entertainment| GET    | /entertainment        | Fetch entertainment items |
| Admin        | GET    | /admin/roles          | Fetch admin roles         |

## 📸 Screenshots

![Admin Dashboard](src/assets/Admin%20Dashboard.jpg)


## 🔐 Environment Variables

Create a `.env.local` file in the root directory with the following variables:

```
VITE_SUPABASE_URL=https://your-supabase-instance.supabase.co
VITE_SUPABASE_ANON_KEY=your_anon_key_here
```

**Required Variables:**
- `VITE_SUPABASE_URL` - Your Supabase project URL
- `VITE_SUPABASE_ANON_KEY` - Your Supabase anonymous/public key


### Code Style Guidelines
- Use TypeScript for type safety
- Follow ESLint configuration
- Write meaningful commit messages
- Add comments for complex logic

## 📄 License

This project is licensed under the MIT License – free to use and modify. See LICENSE file for details.

