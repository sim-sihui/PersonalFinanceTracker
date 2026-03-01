*⚠️ Note: The core development of this project took place in a private repository to protect API keys and sensitive configuration. This public version represents the finalised production build.*

# 💰 Expense Tracker

## 📌 About This Application

This is a comprehensive personal finance management web application built with React. It enables users to track income, expenses, budgets, investments, insurance policies, CPF contributions, and overall net worth — all within a single, unified platform.

The application is designed to provide clear financial visibility, structured tracking, and meaningful insights to support better financial decision-making.

## 🎯 Motivation

This project was created with the goal of improving personal financial awareness and literacy. Many individuals lack a consolidated view of their financial position across cash flow, long-term assets, and statutory contributions.

By building this expense tracker, I aim to provide a practical and intuitive tool that empowers users to better understand their financial situation, make informed decisions, and strengthen their long-term financial well-being.

---

## 🛠️ Technologies Used

| Technology | Purpose |
|---|---|
| **React 19** | UI library for building interactive components |
| **Vite 7** | Lightning-fast build tool and dev server with HMR |
| **React Router DOM** | Client-side routing and navigation |
| **Chart.js & react-chartjs-2** | Interactive charts for financial visualisations |
| **Recharts** | Additional charting library for cash flow and trend analysis |
| **PapaParse** | CSV file parsing for importing transactions |
| **SheetJS (xlsx)** | Excel file parsing for importing transactions |
| **LocalStorage** | Client-side data persistence |
| **CSS** | Custom styling with dark mode/colour theme support |

---

## ✨ Features

### 📊 Dashboard
- Net worth overview at a glance
- Summary of income, expenses, and savings

### 💸 Money Flow (Transactions, Budgets & Loans)
- Add, edit, and delete income/expense transactions
- Categorise transactions (e.g. Food, Transport, Bonus, etc.)
- Tag transactions as Want or Need
- Track payment method and card used
- **Import transactions** from CSV and Excel files
- Create and manage monthly budgets with overflow tracking
- Recurring budgets that auto-renew each month
- Budget overspend warnings with carry-over options
- Savings goals with progress tracking
- Emergency fund tracker with history chart
- Loan management (add, edit, delete loans)

### 💎 Wealth (Investments, Assets & CPF)
- Investment portfolio tracking
- Credit/debit card management
- CPF (Central Provident Fund) calculator — OW/AW breakdown, contribution rates by age
- CPF account balance tracking (OA, SA, MA)

### 🛡️ Protection & Obligations (Insurance & Tax)
- Insurance policy management (add, edit, delete policies)
- Singapore tax estimation based on income and CPF data

### 📅 Calendar View
- Visual calendar showing transactions by date

### 🎨 General
- Dark mode and theme switching
- Responsive design
- Data persisted locally in the browser (no backend required)

---

## 🏗️ The Build Process

1. **Scaffolded with Vite** — initialised the project using `create-vite` with the React template for a fast, modern development setup.
2. **Built the Dashboard first** — created the main overview page to establish the layout, navigation, and core data flow.
3. **Transactions page** — developed a full CRUD interface for adding, editing, and deleting income and expense records, including category tagging and payment method tracking.
4. **Budgets & Savings** — added budget creation with monthly tracking, overflow/carry-over logic, recurring budgets, and savings goal progress bars.
5. **CPF & Tax** — built a CPF contribution calculator with OW/AW inputs and age-based rates, plus a tax estimator tied to transaction data.
6. **Investments, Insurance & Loans** — extended the app with pages for tracking investment portfolios, insurance policies, and loan repayments.
7. **Calendar view** — added a calendar visualisation to see transactions by date.
8. **Import feature** — integrated CSV/Excel file parsing (PapaParse & SheetJS) with a column-mapping modal for bulk importing transactions.
9. **Theming & polish** — implemented dark mode, theme switching, and refined the overall UI/UX with custom CSS.

---

## 📚 What I Learned

- **React state management at scale** — managing 10+ pieces of interconnected state (transactions, budgets, savings goals, CPF, loans, insurance, investments, etc.) taught me the importance of clean data flow and when to lift state up.
- **LocalStorage persistence patterns** — learned how to hydrate state from LocalStorage on mount and sync changes back with `useEffect`, including handling edge cases like missing or malformed data.
- **Data visualisation** — gained experience integrating Chart.js and Recharts to build meaningful financial charts (cash flow trends, budget progress, emergency fund history).
- **File parsing in the browser** — learned to use PapaParse and SheetJS to parse user-uploaded CSV and Excel files entirely on the client side.
- **Component architecture** — practised breaking down a large application into reusable, focused components with well-defined props and clear responsibilities.
- **CSS theming** — implemented a theme system with CSS custom properties to support dark mode and multiple colour palettes.

---

## 🌱 Overall Growth

Building this project significantly strengthened my understanding of React and front-end development as a whole. Starting from a simple expense logger, the app evolved into a full personal finance suite — which pushed me to think about architecture, user experience, and maintainability at every step. I became more confident in designing component hierarchies, managing complex state, and creating polished UIs that feel professional and enjoyable to use.

---

## 🚀 How It Could Be Improved

- **Backend & authentication** — add a server (e.g. Node/Express + database) so data is not limited to a single browser's LocalStorage, and allow users to log in across devices.
- **Cloud sync** — sync data to Firebase or Supabase for real-time backup and multi-device access.
- **Data export** — allow users to export their data as CSV/PDF reports.
- **Recurring transactions** — auto-generate repeating expenses (e.g. rent, subscriptions) each month.
- **Multi-currency support** — handle foreign currency transactions and exchange rate conversions.
- **AI-powered insights** — surface spending patterns, anomalies, and personalised savings tips.
- **PWA support** — make the app installable and usable offline as a Progressive Web App.
- **Unit & integration tests** — add a test suite (e.g. Vitest + React Testing Library) for confidence in refactoring.

---

> Built with ❤️ as a personal finance learning project. Enjoy the application.
