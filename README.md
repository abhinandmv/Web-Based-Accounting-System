# Accounting System Web App

A complete web-based Accounting System built with **Flask**, **SQLAlchemy**, **SQLite**, and **Chart.js**. It allows users to register, manage their accounts, record transactions, view financial reports, and export data in CSV/PDF formats.

---

## 📊 Features

- **User Authentication**: Register, login, logout with session management.
- **Accounts Management**: Add, view, and delete different types of accounts (Asset, Liability, Income, Expense).
- **Transactions Management**: Add and delete transactions linked to accounts, with automatic balance updates.
- **Dashboard**: Overview of assets, incomes, expenses, GST payable, and recent transactions with charts.
- **Reports**: Generate Income Statement, Balance Sheet, Ledger, and Cash Flow Statement.
- **Export**: Export reports to **CSV** and **PDF** formats.
- **GST Calculation**: Auto-calculate GST based on transaction type (18% for Income, 5% for Expense).
- **Import Transactions**: Upload CSV files to bulk import transactions.
- **Session Timeout**: Auto-logout after inactivity.

---

## 📚 Tech Stack

- **Frontend**: HTML, CSS, JavaScript, Chart.js
- **Backend**: Python, Flask
- **Database**: SQLite via SQLAlchemy ORM
- **PDF Generation**: wkhtmltopdf

---

## 🚀 Getting Started

### 1. Clone the repository
```bash
git clone https://github.com/your-username/accounting-system-webapp.git
cd accounting-system-webapp
```

### 2. Create and activate a virtual environment
```bash
python -m venv venv
source venv/bin/activate  # On Windows: venv\Scripts\activate
```

### 3. Install dependencies
```bash
pip install -r requirements.txt
```

### 4. Setup database
```bash
# Automatically created when you run the app (SQLite)
```

### 5. Run the application
```bash
python app.py
```

Visit: `http://127.0.0.1:5000`

---

## 📅 Core Functionalities

| Feature | Route | Description |
| :-- | :-- | :-- |
| Registration | `/register` | Create a new user |
| Login | `/login` | Authenticate user |
| Logout | `/logout` | Clear session |
| Dashboard | `/dashboard` | Financial overview |
| Accounts | `/accounts` | Manage accounts |
| Transactions | `/transactions` | Manage transactions |
| Reports | `/reports` | View and export reports |
| Import CSV | `/import` | Bulk upload transactions |
| Export PDF | `/export_dashboard_pdf` | Dashboard PDF download |

---

## 💡 Key Concepts

- **Session Management**: Flask sessions are configured to auto-expire after inactivity.
- **Secure Passwords**: Passwords are hashed using Werkzeug security.
- **Data Validation**: Server-side validation for transaction imports.

---

## 📁 Project Structure

```
├── app.py
├── models.py
├── templates/
│   ├── base.html
│   ├── auth.html
│   ├── dashboard.html
│   ├── accounts.html
│   ├── transactions.html
│   ├── reports.html
│   ├── ledger.html
│   ├── income_statement.html
│   ├── balance_sheet.html
│   ├── cashflow_statement.html
│   └── profile.html
├── static/
│   ├── styles.css
│   └── ... (icons, fonts)
├── users.db  # Created automatically
├── README.md
├── requirements.txt
```

---

## 🚀 Future Enhancements

- Add email notifications for important actions.
- Multi-user role system (Admin, Accountant).
- More detailed permission management.
- Better charts & analytics.
- Mobile responsive UI.

---

## 📷 Screenshots
![image](https://github.com/user-attachments/assets/05e109c2-1917-4d5b-b8fc-d69eae6caa31)

![image](https://github.com/user-attachments/assets/df1cd905-e005-4e99-bccd-73dfa7255899)

![image](https://github.com/user-attachments/assets/842bab99-fd25-4595-9b69-37a4758483ca)

![image](https://github.com/user-attachments/assets/e51f71c9-1658-427c-9293-d978ef69d244)


## 👥 Contributors
- 👨‍💻 **[Abhinand Meethele Valappil](https://github.com/abhinandmv)**
- 🧑‍💻 **[Garv Randhar](https://github.com/GarvRandhar)**


## ⚠️ License

This project is licensed under the **MIT License** - see the [LICENSE](LICENSE) file for details.

---

> "Accounting simplified for everyone."


