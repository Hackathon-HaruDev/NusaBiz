# NusaBiz

<p align="center">
  <img src="https://img.shields.io/badge/React-19.2.0-61DAFB?style=for-the-badge&logo=react&logoColor=white" alt="React"/>
  <img src="https://img.shields.io/badge/Vite-7.2.4-646CFF?style=for-the-badge&logo=vite&logoColor=white" alt="Vite"/>
  <img src="https://img.shields.io/badge/Express-5.2.1-000000?style=for-the-badge&logo=express&logoColor=white" alt="Express"/>
  <img src="https://img.shields.io/badge/TypeScript-5.9.3-3178C6?style=for-the-badge&logo=typescript&logoColor=white" alt="TypeScript"/>
  <img src="https://img.shields.io/badge/Supabase-Database-3ECF8E?style=for-the-badge&logo=supabase&logoColor=white" alt="Supabase"/>
</p>

This repository serves as the monorepo for NusaBiz application. It encompasses two main services:

| Service        | Description                                                                                                                                                      |
| -------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| **NusaBiz-FE** | Frontend application built with React + Vite + TypeScript. Provides the user interface for business management, transactions, products, and AI-powered features. |
| **NusaBiz-BE** | Backend API service built with Express.js + TypeScript. Handles authentication, business logic, and integrates with Supabase database and Kolosal AI.            |

## 🚀 Features

- 📊 **Dashboard** - Business analytics and overview
- 💰 **Transaction Management** - Track income and expenses
- 📦 **Product Management** - CRUD operations for products with image upload
- 🤖 **AI Assistant** - Powered by Kolosal AI for business insights
- 🔐 **Authentication** - Secure user authentication system
- 🏢 **Multi-Business Support** - Manage multiple businesses

## 📁 Project Structure

```
NusaBiz/
├── NusaBiz-FE/          # Frontend (React + Vite)
│   ├── src/
│   │   ├── components/  # Reusable UI components
│   │   ├── pages/       # Page components
│   │   ├── functions/   # API functions and utilities
│   │   └── constant/    # Constants and routes
│   └── ...
├── NusaBiz-BE/          # Backend (Express.js)
│   ├── src/
│   │   ├── routes/      # API routes
│   │   ├── utils/       # Utility functions
│   │   └── index.ts     # Entry point
│   └── ...
└── README.md
```

## 🛠️ How to Install

### Prerequisites

- Node.js (v18 or higher)
- npm or yarn
- Supabase account (for database)
- Kolosal API key (for AI features)

### Clone the Repository

```bash
git clone https://github.com/Hackathon-HaruDev/NusaBiz.git
cd NusaBiz
```

### Backend Setup

1. Navigate to backend directory:

   ```bash
   cd NusaBiz-BE
   ```

2. Copy the environment file:

   ```bash
   # Unix/Mac
   cp .env.example .env

   # Windows (PowerShell)
   Copy-Item .env.example .env
   ```

3. Configure your `.env` file:

   ```env
   VITE_SUPABASE_URL=your_supabase_url
   VITE_SUPABASE_ANON_KEY=your_supabase_anon_key
   VITE_KOLOSAL_API=your_kolosal_api_key
   ```

4. Install dependencies:
   ```bash
   npm install
   ```

### Frontend Setup

1. Navigate to frontend directory:

   ```bash
   cd NusaBiz-FE
   ```

2. Copy the environment file:

   ```bash
   # Unix/Mac
   cp .env.example .env

   # Windows (PowerShell)
   Copy-Item .env.example .env
   ```

3. Configure your `.env` file:

   ```env
   VITE_BASE_URL=http://localhost:3000/api/v1
   ```

4. Install dependencies:
   ```bash
   npm install
   ```

## ▶️ How to Run

### Development

**Start Backend:**

```bash
cd NusaBiz-BE
npm run dev
```

Backend will run on `http://localhost:3000`

**Start Frontend:**

```bash
cd NusaBiz-FE
npm run dev
```

Frontend will run on `http://localhost:5173`

### Production

**Build Backend:**

```bash
cd NusaBiz-BE
npm run build
npm start
```

**Build Frontend:**

```bash
cd NusaBiz-FE
npm run build
npm run preview
```

## 🌐 Deployment

| Service  | Recommended Platform    |
| -------- | ----------------------- |
| Frontend | Vercel, Netlify         |
| Backend  | Railway, Render, Fly.io |
| Database | Supabase                |

### Deploy Frontend to Vercel

1. Import your GitHub repository to Vercel
2. Set **Root Directory** to `NusaBiz-FE`
3. Configure environment variables
4. Deploy!

### Deploy Backend to Railway

1. Create a new project on Railway
2. Connect your GitHub repository
3. Set **Root Directory** to `NusaBiz-BE`
4. Configure environment variables
5. Deploy!

## 🤝 How to Contribute

1. Fork the repository and clone it locally

2. Create a new branch for your feature:

   ```bash
   git checkout -b feat/your-feature-name
   ```

3. Make your changes, commit them, and push to your forked repository:

   ```bash
   git add .
   git commit -m "feat: add your feature description"
   git push origin feat/your-feature-name
   ```

4. Create a pull request to the `main` branch of this repository

## 📝 License

This project is licensed under the ISC License.

## 👥 Team

**Hackathon-HaruDev**

---

<p align="center">
  Made with ❤️ for Indonesian UMKM
</p>
