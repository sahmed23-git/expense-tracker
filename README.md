# Expense Tracker

A full-stack web application built with Flask for tracking personal expenses with user authentication and category-based organization.

![Python](https://img.shields.io/badge/Python-3.8+-blue.svg)
![Flask](https://img.shields.io/badge/Flask-3.0.0-green.svg)
![SQLite](https://img.shields.io/badge/Database-SQLite-orange.svg)

## Features

- **User Authentication**: Secure registration and login system with password hashing
- **Expense Management**: Create, read, update, and delete (CRUD) expenses
- **Category Tracking**: Organize expenses by categories (Food, Transportation, Entertainment, etc.)
- **Dashboard Analytics**: 
  - Total expenses summary
  - Category-wise breakdown
  - Expense count statistics
- **Responsive Design**: Modern, gradient UI with smooth user experience
- **Data Security**: User-specific data isolation and authorization checks

## Technologies Used

- **Backend**: Flask (Python)
- **Database**: SQLite with SQLAlchemy ORM
- **Authentication**: Flask-Login with Werkzeug password hashing
- **Frontend**: HTML5, CSS3, Jinja2 templating
- **Architecture**: MVC (Model-View-Controller) pattern

## Prerequisites

- Python 3.8 or higher
- pip (Python package manager)

## Installation

1. **Clone the repository**
```bash
   git clone https://github.com/YOUR_USERNAME/expense-tracker.git
   cd expense-tracker
```

2. **Install dependencies**
```bash
   pip install -r requirements.txt
```

3. **Run the application**
```bash
   python app.py
```

4. **Access the application**
   Open your browser and navigate to `http://127.0.0.1:5000`

## Project Structure
```
expense-tracker/
│
├── app.py                    # Main application file with routes
├── models.py                 # Database models (User, Expense)
├── requirements.txt          # Project dependencies
├── expenses.db              # SQLite database (auto-generated)
│
└── templates/               # HTML templates
    ├── base.html           # Base template with styling
    ├── index.html          # Landing page
    ├── login.html          # Login page
    ├── register.html       # Registration page
    ├── dashboard.html      # Main dashboard
    ├── add_expense.html    # Add expense form
    └── edit_expense.html   # Edit expense form
```

## Usage

1. **Register**: Create a new account with a username and password
2. **Login**: Access your personal expense dashboard
3. **Add Expenses**: Click "Add Expense" to record new expenses with:
   - Description
   - Amount
   - Category
   - Date
4. **View Dashboard**: See all your expenses, totals, and category breakdowns
5. **Edit/Delete**: Manage your existing expenses

## Security Features

- Password hashing using Werkzeug
- User session management with Flask-Login
- User-specific data isolation
- Authorization checks on all expense operations
- SQL injection prevention through SQLAlchemy ORM

## Database Schema

### User Table
- `id`: Primary key
- `username`: Unique username
- `password`: Hashed password

### Expense Table
- `id`: Primary key
- `description`: Expense description
- `amount`: Expense amount (float)
- `category`: Expense category
- `date`: Expense date
- `user_id`: Foreign key to User table

## Author

**Your Name**
- GitHub: [@sahmed23](https://github.com/sahmed23-git)
- LinkedIn: [Saif Ahmed](www.linkedin.com/in/saif-ahmed-961b23335)
