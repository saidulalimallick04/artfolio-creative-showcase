# 🎨 ArtFolio Creative Showcase

> **Objective**: A comprehensive, production-ready platform enabling artists to showcase their work and connect with a community. This repository houses both the robust **FastAPI Backend** and the modern **Next.js Frontend**.

[![Project Demo](https://img.shields.io/badge/Live-Demo-blue?style=for-the-badge&logo=vercel)](https://artfolio-creative-showcase.vercel.app/)

## 🚀 Overview

**ArtFolio** is a full-stack web application designed for the creative community. It combines a high-performance backend for secure data and media management with a visually stunning, responsive frontend for an immersive user experience.

- **Frontend**: Built with Next.js (App Router), Tailwind CSS, and ShadCN UI for a sleek, responsive interface.
- **Backend**: Powered by FastAPI and MongoDB (Beanie ODM) for scalable, asynchronous performance.

## ✨ Features

### 🖥️ Frontend

- **Artist Profiles**: Dedicated, beautifully designed pages for artists.
- **Artwork Showcase**: Detailed views for artworks with masonry-style discovery grids.
- **Interactive Uploads**: Drag-and-drop imagery with live previews.
- **Theming**: Seamless dark/light mode toggle.
- **Responsive Design**: Optimized for everything from mobile phones to large desktops.

### ⚙️ Backend

- **Secure Authentication**: OAuth2 with JWT (Access + Rotate-able Refresh Tokens).
- **User Management**: Unified logic for Artists and Viewers.
- **Media Handling**: Integrated Cloudinary support for optimized image storage.
- **Dynamic Architecture**: Automated API versioning and modular structure.

## 🛠️ Tech Stack

### Frontend

- **Framework**: [Next.js](https://nextjs.org/) (App Router)
- **Styling**: [Tailwind CSS](https://tailwindcss.com/)
- **UI Library**: [ShadCN UI](https://ui.shadcn.com/)
- **Forms**: React Hook Form + Zod
- **Icons**: Lucide React

### Backend

- **Framework**: FastAPI (Python 3.11+)
- **Database**: MongoDB (Beanie ODM + Motor)
- **Security**: OAuth2 JWT, Passlib (Bcrypt)
- **Storage**: Cloudinary
- **Package Manager**: uv

## 📂 Project Structure

This monorepo contains two main directories:

- `artfolio-creative-showcase-backend/`: The FastAPI server code, including models, schemas, and API endpoints.
- `artfolio-creative-showcase-frontend/`: The Next.js client application, including pages, components, and styles.

## 🚀 Getting Started

Follow these instructions to set up the full stack locally.

### Prerequisites

- **Node.js** (v20+)
- **Python** (3.11+)
- **MongoDB** (Local or Atlas)
- **Cloudinary Account** (for image uploads)
- **uv** (recommended for Python) or `pip`

---

### 1️⃣ Backend Setup

1. **Navigate to the backend directory**:

    ```bash
    cd artfolio-creative-showcase-backend
    ```

2. **Configure Environment Variables**:
    Create a `.env` file in the backend root with the following:

    ```env
    # Security
    SECRET_KEY=your_secret_key
    ACCESS_TOKEN_EXPIRE_MINUTES=30
    REFRESH_TOKEN_EXPIRE_DAYS=7

    # Database
    MONGODB_URL=mongodb://localhost:27017
    DB_NAME=artfolio

    # Cloudinary
    CLOUDINARY_CLOUD_NAME=your_cloud_name
    CLOUDINARY_API_KEY=your_api_key
    CLOUDINARY_API_SECRET=your_api_secret
    ```

3. **Install & Run**:
    *Using `uv` (Recommended)*:

    ```bash
    uv sync
    uv run uvicorn main:app --reload
    ```

    *Using `pip`*:

    ```bash
    pip install -r requirements.txt
    uvicorn main:app --reload
    ```

    The backend will be live at `http://localhost:8000`. API Docs: `http://localhost:8000/docs`.

---

### 2️⃣ Frontend Setup

1. **Navigate to the frontend directory** (from project root):

    ```bash
    cd artfolio-creative-showcase-frontend
    ```

2. **Install Dependencies**:

    ```bash
    npm install
    ```

3. **Run Development Server**:

    ```bash
    npm run dev
    ```

    The frontend will be live at `http://localhost:9002` (or the port specified in your terminal).

---

## 👨‍💻 Author

| Profile | Developer Name | Role | GitHub | LinkedIn | X |
| :--- | :--- | :--- | :--- | :--- | :--- |
| [![Sami](https://github.com/saidulalimallick04.png?size=75)](https://github.com/saidulalimallick04) | Saidul Ali Mallick (Sami) | Backend Developer & AIML Engineer | [@saidulalimallick04](https://github.com/saidulalimallick04) | [@saidulalimallick04](https://linkedin.com/in/saidulalimallick04) | [@saidulmallick04](https://x.com/saidulmallick04) |

> ❤️ I believe in building impact, not just writing code.
> *💚 Backend Sage signing off..*
---
