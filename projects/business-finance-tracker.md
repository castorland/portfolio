# Business Finance Tracker

**Client:** Personal Project
**Period:** 2024–2025
**Role:** Full-stack Developer

---

## Overview

A Python-based business finance management system designed for Hungarian solo entrepreneurs. This application helps track and reconcile business finances by extracting and visualizing data from invoices, tax obligations (NAV communications), and bank statements. The tool makes it easy to spot discrepancies and understand where debts accumulated over time.

**Repository:** [business-finance-python](https://github.com/castorland/business-finance-python)

---

## Main Technologies
- **Backend:** Python 3, Flask
- **Database:** SQLAlchemy (SQLite/PostgreSQL)
- **PDF Processing:** PyPDF
- **Frontend:** HTML, CSS, JavaScript

---

## Core Features

### PDF/RTF Data Extraction
- **Automatic invoice parsing** from PDF files
- **NAV tax obligation extraction** from accountant emails (PDF/RTF)
- **Bank statement parsing** for payment tracking
- Smart extraction with Hungarian format awareness

### Database Management
- **Persistent storage** using SQLAlchemy ORM
- **SQLite** for local development
- **PostgreSQL** support for production
- Complete data model for invoices, obligations, and payments

### REST API
- **Full CRUD operations** for all entities (invoices, obligations, payments)
- Manual data correction without re-parsing PDFs
- Extraction history tracking
- Data source tracking (PDF vs manually entered)

### Financial Analysis
- **Monthly income/expense tracking** across multiple years
- **Debt accumulation analysis** with running totals
- **Visual comparison** of obligations vs actual payments
- **Hungarian tax system integration** (ÁFA, TB, SZOCHO, SZJA)
- Month-by-month detailed breakdowns

### User Interface
- **Year switching** (2024/2025)
- **Dashboard with statistics** (total income, obligations, payments, debt)
- **Monthly overview table** with color-coded indicators
- **Running totals view** showing debt accumulation timeline
- **Visual warnings** for months with payment arrears
- **Interactive month details** - click to see breakdown

### Smart Data Management
- **Reload without overwrite** - PDF updates don't erase manual edits
- **Extraction logging** - track when data was imported
- **Backup support** for both SQLite and PostgreSQL

---

## My Contributions

- **Designed and implemented** the entire system from scratch
- **Built PDF/RTF parsers** for Hungarian financial documents
- **Created database schema** with SQLAlchemy ORM
- **Developed REST API** for CRUD operations
- **Implemented Flask web interface** with interactive dashboard
- **Added smart reload logic** to preserve manual edits
- **Wrote comprehensive documentation** including setup, usage, and API guides

---

## Technical Highlights

### Python Best Practices
- Clean separation of concerns (models, database, extractors, app)
- SQLAlchemy ORM for database abstraction
- Environment-based configuration
- RESTful API design

### Data Processing
- Robust PDF/RTF text extraction
- Regular expression parsing for Hungarian formats
- Error handling and validation
- Duplicate detection

### Web Development
- Flask routing and templating
- JSON API responses
- Frontend JavaScript for interactivity
- Responsive CSS layout

---

## Results & Impact

- **Simplified financial tracking** for solo entrepreneurs
- **Eliminated manual spreadsheet work**
- **Clear visualization** of tax obligations vs payments
- **Early detection** of payment discrepancies
- **Historical analysis** showing how debt accumulated
- **Public Python reference** for similar projects

---

## User Types

- **Solo Entrepreneurs:** Track personal business finances
- **Developers:** Reference for Python/Flask/SQLAlchemy projects

---

## Deployment

- **Local development:** SQLite database
- **Production ready:** PostgreSQL support
- Simple startup script: `./start.sh`
- Port 5001 by default

---

## Documentation

Comprehensive documentation included:
- `README.md` - Quick start guide
- `DATABASE_GUIDE.md` - Database schema and API docs
- `CRUD_GUIDE.md` - REST API usage examples
- `SETUP_GUIDE.md` - Installation instructions
- `TROUBLESHOOTING.md` - Common issues and solutions

---

## Open Source

This project is publicly available on GitHub as a Python reference for:
- Flask web applications
- PDF data extraction
- SQLAlchemy ORM usage
- Financial tracking systems
- REST API implementation

[View on GitHub](https://github.com/castorland/business-finance-python)
