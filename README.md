NAME: MICHELLE ANYANGO MOLA | INSTITUTION: KENYA INSTITUTE OF SOFTWARE ENGINEERING AND PROFESSIONAL STUDIES

# Finance Dashboard - Personal Finance Management System

**By Michelle Mola | Kenya Institute of Software Engineering**

A complete full-stack finance management application that helps individuals and businesses track income, monitor expenses, and make informed financial decisions through beautiful, interactive dashboards.

## Quick Links

| Resource | Link |
|----------|------|
| Live Demo | https://finance-dashboard-ashy-six.vercel.app |
| Backend API | https://finance-backend-api-74z9.onrender.com |
| Health Check | https://finance-backend-api-74z9.onrender.com/health |

### Test Credentials

Email: admin@finance.com
Password: Admin@123

## What This App Does

This is a complete finance tracking system where users can:

- Create an account and manage their personal finances
- Add income and expenses with categories and descriptions
- View beautiful charts showing spending patterns
- Filter transactions by date, category, or type
- See financial summaries including total income, expenses, and net balance
- Track monthly trends to understand spending habits
- Edit or delete transactions as needed

## Who Can Use This App

| Role | What They Can Do |
|------|------------------|
| Admin | Full control - manage all users, view all transactions, delete anything |
| Analyst | View dashboards, add and edit their own transactions |
| Viewer | View-only access to their own financial data |

Each user sees ONLY their own transactions. Your data is private to you. Admins can see everything for management purposes.

## How It Works

### For Regular Users

1. Sign up for a free account
2. Log in to your dashboard
3. Add your income (salary, freelance, gifts)
4. Add your expenses (rent, groceries, entertainment)
5. View charts to see where your money goes
6. Filter transactions to analyze specific time periods

### For Admins

- View all users and their transactions
- Manage user roles and permissions
- Delete any inappropriate content
- Monitor system activity

## Features in Detail

### Dashboard Overview
- 4 Stat Cards: Total Income, Total Expenses, Net Balance, Transaction Count
- Real-time updates when you add or delete transactions

### Interactive Charts
- Monthly Trends Bar Chart: Compare income vs expenses month by month
- Category Breakdown Pie Chart: See exactly which categories you spend most on

### Transaction Management
- Add Transaction Modal: Simple form to add income or expense
- Edit Transaction: Update amount, category, date, or description
- Delete Transaction: Remove incorrect entries (Admin only for others)

### Filtering System
- Filter by transaction type (Income/Expense)
- Filter by category (Salary, Rent, Groceries, etc.)
- Filter by date range (start date to end date)
- Clear filters button to reset all

### User Authentication
- Secure login with JWT tokens
- Password hashing with bcrypt
- Session lasts 7 days before requiring re-login

## Use Cases

### Personal Finance
- Track your monthly spending
- Save for goals by monitoring expenses
- Understand where your money goes

### Small Business
- Track business income and expenses
- Generate financial reports
- Monitor cash flow

### Family Budgeting
- Multiple family members can have their own accounts
- Admin parent can oversee children's spending
- Teach financial literacy

### Freelancers
- Track project income
- Categorize business expenses
- Prepare for tax season

## Technical Overview

### Backend (Node.js + Express)
- RESTful API with 20+ endpoints
- JWT authentication for security
- PostgreSQL database for production
- Prisma ORM for type-safe database queries
- Rate limiting to prevent abuse
- Input validation on all endpoints

### Frontend (React + Vite)
- Responsive design works on all devices
- Chart.js for beautiful data visualization
- Modal forms for adding/editing transactions
- Real-time dashboard updates
- Role-based UI (different buttons for different roles)

### Database (PostgreSQL)
- Three main tables: users, roles, transactions
- Foreign key constraints for data integrity
- Enums for status and transaction types
- Indexes for fast queries

## Security Features

| Feature | Implementation |
|---------|----------------|
| Passwords | Hashed with bcrypt (10 rounds) |
| Authentication | JWT tokens (7-day expiration) |
| Rate Limiting | 1000 requests per 15 minutes |
| Headers | Helmet.js for security headers |
| CORS | Restricted to specific frontend domains |
| Input Validation | All inputs validated before processing |
| SQL Injection | Prisma ORM prevents injection attacks |

## Performance

- Backend response time: less than 100ms for most requests
- Frontend loads in under 2 seconds
- Database queries optimized with indexes
- Charts render smoothly even with thousands of transactions

## Deployment

### Live URLs

| Service | URL |
|---------|-----|
| Frontend | https://finance-dashboard-ashy-six.vercel.app |
| Backend API | https://finance-backend-api-74z9.onrender.com |
| PostgreSQL | Hosted on Render (free tier) |

### Hosting Platforms

- Render: Backend API + PostgreSQL database
- Vercel: Frontend React application
- GitHub: Source code version control

## API Endpoints Summary

| Method | Endpoint | Description |
|--------|----------|-------------|
| POST | /api/auth/register | Create account |
| POST | /api/auth/login | Login |
| GET | /api/transactions | Get transactions |
| POST | /api/transactions | Add transaction |
| PUT | /api/transactions/:id | Update transaction |
| DELETE | /api/transactions/:id | Delete transaction |
| GET | /api/dashboard/summary | Get totals |
| GET | /api/dashboard/complete | Full dashboard |
| GET | /api/dashboard/category-totals | Category breakdown |
| GET | /api/dashboard/monthly-trends | Monthly trends |

## What I Learned

Building this project taught me:

- Full-stack development from database to UI
- JWT authentication and secure session management
- Role-based access control with middleware
- Prisma ORM for database operations
- Chart.js for data visualization
- Deployment on Render and Vercel
- REST API design best practices
- Error handling and input validation
- Git workflow and version control

## Future Improvements

- Export transactions to CSV/PDF
- Recurring transactions (monthly bills)
- Budget alerts when nearing limits
- Dark mode toggle
- Mobile app with React Native
- Bank API integration (automatic transaction imports)
- Receipt image upload
- Shared family budgets

## Contributing

Contributions are welcome! Please feel free to submit a Pull Request.

1. Fork the repository
2. Create your feature branch
3. Commit your changes
4. Push to the branch
5. Open a Pull Request

## License

ISC License - Free for personal and commercial use

## Support This Project

If you find this project useful, please give it a star on GitHub! It helps others discover the project and motivates continued development.

Made with ❤️ by Michelle Mola | Kenya Institute of Software Engineering