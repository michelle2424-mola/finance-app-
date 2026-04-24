# Finance Dashboard - Personal Finance Management System

A full-stack finance management application that helps users track income, expenses, and visualize their financial health through interactive dashboards.

## 📋 Table of Contents

- [Overview](#overview)
- [Features](#features)
- [Tech Stack](#tech-stack)
- [Project Structure](#project-structure)
- [Installation](#installation)
- [Environment Variables](#environment-variables)
- [Running the Application](#running-the-application)
- [API Endpoints](#api-endpoints)
- [Role-Based Access Control](#role-based-access-control)
- [Live Demo](#live-demo)
- [Screenshots](#screenshots)
- [Contributing](#contributing)
- [License](#license)

---

## Overview

The Finance Dashboard is a complete personal finance management solution that allows users to:

- Track income and expenses
- Categorize transactions
- View financial summaries and trends
- Generate visual reports with charts
- Manage user roles and permissions

Built with **Node.js/Express** backend, **React** frontend, and **PostgreSQL/MySQL** database.

---

## Features

### Core Features

| Feature | Description |
|---------|-------------|
| 🔐 **Authentication** | JWT-based authentication with secure password hashing |
| 👥 **Role Management** | Three roles: Admin, Analyst, Viewer |
| 💰 **Transaction Management** | Create, read, update, delete financial records |
| 🔍 **Filtering** | Filter transactions by date range, category, and type |
| 📊 **Dashboard Analytics** | Visual summary of income, expenses, and net balance |
| 🥧 **Category Breakdown** | Pie chart showing expenses by category |
| 📈 **Monthly Trends** | Bar chart comparing income vs expenses over time |
| 📱 **Responsive Design** | Works on desktop, tablet, and mobile devices |

### Security Features

- Password hashing with bcrypt
- JWT token authentication (7-day expiration)
- Rate limiting (1000 requests per 15 minutes)
- Helmet.js for security headers
- Input validation with express-validator
- Role-based access control middleware

---

## Tech Stack

### Backend
| Technology | Purpose |
|------------|---------|
| Node.js | Runtime environment |
| Express.js | Web framework |
| Prisma | ORM for database operations |
| PostgreSQL / MySQL | Database |
| JWT | Authentication |
| bcryptjs | Password hashing |
| express-validator | Input validation |
| helmet | Security headers |
| cors | Cross-origin resource sharing |

### Frontend
| Technology | Purpose |
|------------|---------|
| React.js | UI framework |
| Vite | Build tool |
| Chart.js | Data visualization |
| react-chartjs-2 | React wrapper for Chart.js |
| CSS3 | Styling |

### Deployment
| Platform | Purpose |
|----------|---------|
| Render | Backend hosting + PostgreSQL |
| Vercel | Frontend hosting |
| GitHub | Version control |

---

## Project Structure
