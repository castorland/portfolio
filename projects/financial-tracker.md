# Financial Tracker

**Client:** Personal Project  
**Period:** 2024–2025  
**Role:** Full-stack Developer

---

## Overview

A comprehensive web-based financial management application for tracking and analyzing both business and personal finances. This system helps Hungarian entrepreneurs and individuals manage their financial records by importing bank statements (CIB and Revolut), automatically categorizing transactions, tracking budgets, and generating detailed financial reports.

**Repository:** [financial-tracker](https://github.com/castorland/financial-tracker)

---

## Main Technologies

### Backend
- **Python 3** with **Flask**
- **SQLAlchemy** ORM (SQLite)
- **pdfplumber** for PDF parsing
- Machine learning for transaction categorization

### Frontend
- **React** with **TypeScript**
- **Vite** for build tooling
- **Chart.js** for data visualization
- Modern component-based architecture

---

## Core Features

### Bank Statement Import
- **CIB Bank PDF parser** with structured field extraction
- **Revolut PDF parser** with multi-currency support
- Automatic detection of:
  - Transaction type (card payment, transfer, fee, etc.)
  - Counterparty information
  - Reference numbers
  - Account details
- Intelligent duplicate detection

### Account Management
- Multiple account support (business and personal)
- Different account types (CIB, Revolut)
- Balance tracking across all accounts
- Account-specific filtering

### Transaction Categorization
- **Manual categorization** with category selection
- **Automatic categorization** using machine learning
- Rule-based categorization system
- Bulk transaction categorization
- Income/expense/transfer tracking

### Budget Planning
- Monthly/quarterly/yearly budgets
- Per-category budget allocation
- Budget vs actual spending comparison
- Color-coded budget progress indicators
- Alert system for budget thresholds

### Advanced Analytics
- **Expense Analysis** page with:
  - Merchant spending breakdown
  - Spending trends over time
  - Category distribution
  - Top expenses by amount
  - Monthly comparisons
- **Dashboard** with:
  - Current month income, expenses, net cash flow
  - Total balance across accounts
  - Interactive charts (income vs expenses, category breakdown)
  - Recent transactions list
- **Reports** page with customizable filters

### Transaction Management
- Search and filter by:
  - Account
  - Date range
  - Category
  - Description
  - Amount
- Inline transaction editing
- Manual transaction entry
- Transaction notes
- Transfer detection and linking

---

## My Contributions

- **Designed and implemented** the entire full-stack system
- **Built advanced PDF parsers** for Hungarian and international bank statements
- **Developed REST API** with Flask blueprint architecture
- **Created React frontend** with TypeScript and modern components
- **Implemented machine learning** for transaction categorization
- **Built responsive UI** with interactive charts and dashboards
- **Added structured data extraction** from bank statements
- **Wrote comprehensive documentation** with setup guides and usage instructions

---

## Technical Highlights

### Backend Architecture
- Clean separation of concerns with Flask blueprints
- SQLAlchemy models with relationships
- RESTful API design
- PDF parsing with structured field extraction
- Transaction categorization service with ML
- Database migration scripts

### Frontend Architecture
- React with TypeScript for type safety
- Component-based architecture
- Centralized API service layer
- Chart.js integration for visualizations
- Responsive design with modern CSS
- Form validation and error handling

### Data Processing
- Advanced PDF text extraction with position-based parsing
- Regular expression patterns for Hungarian formats
- Transaction type identification
- Merchant name extraction and cleaning
- Multi-line transaction parsing

### User Experience
- Interactive dashboard with real-time updates
- Color-coded budget indicators
- Modal dialogs for editing
- Confirmation prompts for destructive actions
- Dynamic page titles
- Responsive layout for all screen sizes

---

## Results & Impact

- **Unified financial tracking** for business and personal accounts
- **Automated data entry** from PDF bank statements
- **Intelligent categorization** reduces manual work
- **Visual insights** into spending patterns
- **Budget management** helps control expenses
- **Comprehensive reporting** for tax preparation
- **Open source reference** for similar projects

---

## User Types

- **Solo Entrepreneurs:** Track business finances with automatic categorization
- **Personal Finance Users:** Manage personal accounts and budgets
- **Developers:** Reference for Flask + React + TypeScript projects

---

## Deployment

- **Development:** SQLite database with Flask dev server
- **Frontend:** Vite dev server with hot reload
- **Build:** Production-ready build system
- **Makefile:** Simple commands for setup and running

Quick start:
```bash
make install  # Install dependencies
make init-db  # Initialize database
make dev      # Run backend and frontend
```

---

## Documentation

Comprehensive documentation included:
- `README.md` - Quick start guide and usage
- `Makefile` - All available commands
- Project specification document
- API endpoint documentation
- Component documentation

---

## Key Features Breakdown

### PDF Import Process
1. Select account and upload PDF
2. System parses and extracts transactions
3. Review parsed data with category suggestions
4. Adjust categories if needed
5. Confirm import to database

### Dashboard Views
- **Summary Cards:** Income, Expenses, Net Cash Flow, Total Balance
- **Monthly Chart:** Income vs Expenses over time
- **Category Pie Chart:** Spending distribution
- **Recent Transactions:** Latest account activity

### Expense Analysis
- Filter by date range and account type
- View top merchants with spending totals
- Analyze category breakdowns
- Track spending trends
- Identify unusual spending patterns

### Budget Management
- Create budgets by category and time period
- Set spending limits
- Track progress with visual indicators
- Get alerts when approaching limits
- Compare actual vs budgeted amounts

---

## Open Source

This project is publicly available on GitHub as a reference for:
- Flask + React TypeScript applications
- PDF data extraction from bank statements
- Financial tracking systems
- Machine learning for categorization
- Modern web application architecture

[View on GitHub](https://github.com/castorland/financial-tracker)

---

## Future Enhancements

- Multi-currency support
- More bank statement formats
- Export functionality (CSV, PDF reports)
- Mobile app version
- Cloud deployment
- Multi-user support
