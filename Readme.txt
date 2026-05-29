Expense-Tracker-main/
│
├── 📄 README.md
│
├── 📂 backend/
│   ├── 📄 server.js                        ← Entry point
│   ├── 📄 .env                             ← Environment variables
│   ├── 📄 package.json
│   │
│   ├── 📂 config/
│   │   └── 📄 db.js                        ← MongoDB connection
│   │
│   ├── 📂 models/
│   │   ├── 📄 User.js
│   │   ├── 📄 Income.js
│   │   └── 📄 Expense.js
│   │
│   ├── 📂 controllers/
│   │   ├── 📄 authController.js
│   │   ├── 📄 dashboardController.js
│   │   ├── 📄 incomeController.js
│   │   └── 📄 expenseController.js
│   │
│   ├── 📂 routes/
│   │   ├── 📄 authRoutes.js
│   │   ├── 📄 dashboardRoutes.js
│   │   ├── 📄 incomeRoutes.js
│   │   └── 📄 expenseRoutes.js
│   │
│   ├── 📂 middleware/
│   │   ├── 📄 authMiddleware.js            ← JWT auth guard
│   │   └── 📄 uploadMiddleware.js          ← Multer file upload
│   │
│   └── 📂 uploads/                         ← Profile photos stored here
│
└── 📂 frontend/expense-tracker/
    ├── 📄 index.html
    ├── 📄 vite.config.js
    ├── 📄 package.json
    │
    └── 📂 src/
        ├── 📄 main.jsx                     ← React entry point
        ├── 📄 App.jsx                      ← Routes & app shell
        ├── 📄 index.css
        │
        ├── 📂 pages/
        │   ├── 📂 Auth/
        │   │   ├── 📄 LoginForm.jsx
        │   │   └── 📄 SignUpForm.jsx
        │   └── 📂 Dashboard/
        │       ├── 📄 Home.jsx
        │       ├── 📄 Income.jsx
        │       └── 📄 Expense.jsx
        │
        ├── 📂 components/
        │   ├── 📄 Modal.jsx
        │   ├── 📄 DeleteAlert.jsx
        │   ├── 📄 EmojiPickerPopup.jsx
        │   ├── 📂 Cards/
        │   │   ├── 📄 CharAvatar.jsx
        │   │   ├── 📄 InfoCard.jsx
        │   │   └── 📄 TransactionInfoCard.jsx
        │   ├── 📂 Charts/
        │   │   ├── 📄 CustomBarChart.jsx
        │   │   ├── 📄 CustomLineChart.jsx
        │   │   ├── 📄 CustomPieChart.jsx
        │   │   ├── 📄 CustomLegend.jsx
        │   │   └── 📄 CustomTooltip.jsx
        │   ├── 📂 Dashboard/
        │   │   ├── 📄 FinanceOverview.jsx
        │   │   ├── 📄 RecentTransactions.jsx
        │   │   ├── 📄 RecentIncome.jsx
        │   │   ├── 📄 RecentIncomeWithChart.jsx
        │   │   ├── 📄 ExpenseTransactions.jsx
        │   │   └── 📄 Last30DaysExpenses.jsx
        │   ├── 📂 Income/
        │   │   ├── 📄 IncomeOverview.jsx
        │   │   ├── 📄 AddIncomeForm.jsx
        │   │   └── 📄 IncomeList.jsx
        │   ├── 📂 Expense/
        │   │   ├── 📄 ExpenseOverview.jsx
        │   │   ├── 📄 AddExpenseForm.jsx
        │   │   └── 📄 ExpenseList.jsx
        │   ├── 📂 Inputs/
        │   │   ├── 📄 Input.jsx
        │   │   └── 📄 ProfilePhotoSelector.jsx
        │   └── 📂 Layouts/
        │       ├── 📄 AuthLayout.jsx
        │       ├── 📄 DashboardLayout.jsx
        │       ├── 📄 Navbar.jsx
        │       └── 📄 SideMenu.jsx
        │
        ├── 📂 context/
        │   └── 📄 UserContext.jsx           ← Global user state
        │
        ├── 📂 hooks/
        │   └── 📄 useUserAuth.js            ← Auth custom hook
        │
        └── 📂 utils/
            ├── 📄 apiPaths.js              ← API endpoint constants
            ├── 📄 axiosInstance.js         ← Axios config + interceptors
            ├── 📄 helper.js               ← Utility functions
            ├── 📄 data.js                 ← Static data/constants
            └── 📄 uploadImage.js          ← Image upload helper