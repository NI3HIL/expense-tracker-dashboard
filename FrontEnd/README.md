# <div align="center">💰 Expense Tracker Frontend</div>

<div align="center">

A modern, responsive React application built with Vite for managing personal finances. This frontend provides an intuitive user interface for tracking expenses, managing income, and visualizing financial data with beautiful charts and analytics.

</div>

<div align="justify">

## 🚀 Features

### 🔐 Authentication & User Management

- **Secure Login/Registration**: JWT-based authentication with form validation
- **Profile Management**: User profile updates with image upload capability
- **Auto Authentication**: Persistent login with token-based session management
- **Protected Routes**: Route guards for authenticated user access
- **Account Deletion**: Complete account removal functionality

### 💸 Expense Tracking

- **Add Expenses**: Create expense entries with categories, amounts, dates, and emoji icons
- **Expense Categories**: Organize expenses by custom categories (Food, Transport, etc.)
- **Visual Expense List**: Beautiful cards displaying expense details
- **Expense Analytics**: Visual charts showing expense distribution and trends
- **Bulk Operations**: Delete all expenses or individual entries
- **Excel Export**: Download expense data as Excel files

### 💰 Income Management

- **Income Tracking**: Record income from multiple sources
- **Income Categories**: Organize income by different sources (Salary, Business, etc.)
- **Income Analytics**: Visual representation of income data
- **Income Overview**: Comprehensive income summaries and insights
- **Excel Export**: Export income data for external analysis

### 📊 Dashboard & Analytics

- **Financial Overview**: Comprehensive pie charts showing balance, income, and expenses
- **Recent Transactions**: Quick view of latest income and expense entries
- **Monthly Analytics**: Month-over-month financial analysis
- **Interactive Charts**: Beautiful charts using Recharts library
- **Real-time Updates**: Live data updates without page refresh

### 🎨 User Interface & Experience

- **Modern Design**: Clean, minimalist interface with Tailwind CSS
- **Responsive Layout**: Mobile-first design that works on all devices
- **Dark/Light Theme**: Elegant color schemes and visual hierarchy
- **Interactive Components**: Smooth animations and user feedback
- **Emoji Integration**: Fun emoji picker for categorizing transactions
- **Toast Notifications**: Real-time success/error feedback

## 🛠️ Tech Stack

### **Core Technologies**

- **React 19.1.0** - Latest React with modern features and hooks
- **Vite 7.0.4** - Ultra-fast build tool and development server
- **React Router DOM 7.7.1** - Client-side routing and navigation
- **Axios 1.11.0** - HTTP client for API communication

### **UI & Styling**

- **Tailwind CSS 4.1.11** - Utility-first CSS framework
- **React Icons 5.5.0** - Comprehensive icon library
- **React Hot Toast 2.5.2** - Beautiful toast notifications
- **Emoji Picker React 4.13.2** - Interactive emoji selection

### **Data Visualization**

- **Recharts 3.1.0** - Composable charting library for React
- **Custom Chart Components** - Tailored pie charts, bar charts, and line charts

### **Utilities & Helpers**

- **Moment.js 2.30.1** - Date manipulation and formatting
- **Custom Axios Instance** - Configured HTTP client with interceptors
- **Helper Functions** - Validation, formatting, and utility functions

### **Development Tools**

- **ESLint 9.30.1** - Code linting and quality assurance
- **Vite Plugins** - React plugin and optimizations
- **TypeScript Support** - Type definitions for React components

## 📁 Project Structure

```
FrontEnd/
├── public/
│   └── vite.svg                 # Vite favicon
├── src/
│   ├── assets/
│   │   ├── react.svg           # React logo
│   │   └── images/
│   │       └── card2.png       # Card background image
│   ├── components/
│   │   ├── Cards/
│   │   │   ├── CharAvatar.jsx       # User avatar component
│   │   │   ├── EmptyTransactionInfoCard.jsx # Empty state card
│   │   │   ├── InfoCard.jsx         # Information display card
│   │   │   └── TransactionInfoCard.jsx # Transaction detail card
│   │   ├── Charts/
│   │   │   ├── CustomBarChart.jsx   # Bar chart component
│   │   │   ├── CustomLegend.jsx     # Chart legend component
│   │   │   ├── CustomLineChart.jsx  # Line chart component
│   │   │   ├── CustomPieChart.jsx   # Pie chart component
│   │   │   └── CustomTooltip.jsx    # Chart tooltip component
│   │   ├── Dashboard/
│   │   │   ├── ExpenseTransactions.jsx    # Expense transaction list
│   │   │   ├── FinanceOverview.jsx        # Financial overview widget
│   │   │   ├── Last30DaysExpenses.jsx     # Recent expenses chart
│   │   │   ├── RecentIncome.jsx           # Recent income display
│   │   │   ├── RecentIncomeWithChart.jsx  # Income with chart view
│   │   │   └── RecentTransactions.jsx     # Recent transactions list
│   │   ├── Expense/
│   │   │   ├── AddExpenseForm.jsx         # Expense creation form
│   │   │   ├── ExpenseList.jsx            # Expense listing component
│   │   │   └── ExpenseOverview.jsx        # Expense analytics view
│   │   ├── Income/
│   │   │   ├── AddIncomeForm.jsx          # Income creation form
│   │   │   ├── IncomeList.jsx             # Income listing component
│   │   │   └── IncomeOverview.jsx         # Income analytics view
│   │   ├── Inputs/
│   │   │   ├── Input.jsx                  # Reusable input component
│   │   │   ├── ProfilePhotoSelector.jsx   # Image upload component
│   │   │   └── Textarea.jsx               # Textarea input component
│   │   ├── layouts/
│   │   │   ├── AuthLayout.jsx             # Authentication page layout
│   │   │   ├── DashboardLayout.jsx        # Dashboard page layout
│   │   │   ├── Navbar.jsx                 # Navigation bar
│   │   │   └── SideMenu.jsx               # Sidebar navigation
│   │   ├── Profile/
│   │   │   └── SettingButton.jsx          # Profile settings button
│   │   ├── ConfirmAlert.jsx               # Confirmation dialog
│   │   ├── EmojiPickerPopup.jsx           # Emoji selection popup
│   │   └── Modal.jsx                      # Modal component
│   ├── context/
│   │   └── UserContext.jsx                # User state management
│   ├── hooks/
│   │   └── useUserAuth.jsx                # Authentication hook
│   ├── pages/
│   │   ├── Auth/
│   │   │   ├── Login.jsx                  # Login page
│   │   │   └── SignUp.jsx                 # Registration page
│   │   └── Dashboard/
│   │       ├── Home.jsx                   # Dashboard home page
│   │       ├── Income.jsx                 # Income management page
│   │       ├── Expense.jsx                # Expense management page
│   │       └── Profile.jsx                # User profile page
│   ├── utils/
│   │   ├── apiPaths.js                    # API endpoint definitions
│   │   ├── axiosInstance.js               # Configured Axios client
│   │   ├── data.js                        # Static data and constants
│   │   ├── helper.js                      # Utility functions
│   │   └── uploadImage.js                 # Image upload utilities
│   ├── App.jsx                            # Main application component
│   ├── main.jsx                           # Application entry point
│   └── index.css                          # Global styles and Tailwind imports
├── eslint.config.js                       # ESLint configuration
├── index.html                             # HTML template
├── package.json                           # Dependencies and scripts
├── vite.config.js                         # Vite configuration
└── README.md                              # This file
```

## ⚡ Quick Start

### Prerequisites

- Node.js (v18 or higher)
- npm or yarn package manager
- Backend API running (see Backend README)

### Installation

1. **Clone the repository**

   ```bash
   git clone https://github.com/NhanPhamThanh-IT/Fullstack-MERN-Expense-Tracker.git
   cd Fullstack-MERN-Expense-Tracker/FrontEnd
   ```

2. **Install dependencies**

   ```bash
   npm install
   ```

3. **Environment Configuration**
   Update the API base URL in `src/utils/apiPaths.js`:

   ```javascript
   export const BASE_URL = "http://localhost:5000"; // Your backend URL
   ```

4. **Start the development server**

   ```bash
   npm run dev
   ```

5. **Build for production**

   ```bash
   npm run build
   ```

6. **Preview production build**
   ```bash
   npm run preview
   ```

The application will be available at `http://localhost:5173` (or the next available port).

## 🎨 UI Components & Design System

### **Color Palette**

- **Primary**: `#875CF5` (Purple) - Main brand color
- **Success**: `#10B981` (Green) - Positive actions and income
- **Danger**: `#EF4444` (Red) - Destructive actions and expenses
- **Background**: `#FCFBFC` - Main background color
- **Card Background**: `#FFFFFF` - Card and container backgrounds

### **Typography**

- **Primary Font**: Poppins - Modern, clean sans-serif
- **Font Weights**: 300-900 available
- **Responsive Sizing**: Tailwind's responsive text utilities

### **Component Library**

#### **Cards**

```jsx
// Info Card with statistics
<InfoCard
  title="Total Balance"
  amount="$5,000"
  icon="💰"
  color="purple"
/>

// Transaction Card
<TransactionInfoCard
  transaction={transactionData}
  onDelete={handleDelete}
/>
```

#### **Charts**

```jsx
// Pie Chart for financial overview
<CustomPieChart
  data={chartData}
  colors={['#875CF5', '#FA2C37', '#FF6900']}
  showTextAnchor={true}
/>

// Bar Chart for expense trends
<CustomBarChart
  data={monthlyData}
  xKey="month"
  yKey="amount"
/>
```

#### **Forms**

```jsx
// Reusable Input Component
<Input
  label="Email Address"
  type="email"
  placeholder="john@example.com"
  value={email}
  onChange={handleEmailChange}
/>

// Emoji Picker for categories
<EmojiPickerPopup
  onSelect={handleEmojiSelect}
  selectedEmoji="🍕"
/>
```

## 🔌 API Integration

### **Axios Configuration**

The application uses a custom Axios instance with:

- **Base URL Configuration**: Centralized API endpoint management
- **Request Interceptors**: Automatic JWT token attachment
- **Response Interceptors**: Global error handling and authentication
- **Timeout Handling**: 10-second request timeout

### **API Structure**

```javascript
// Authentication APIs
AUTH: {
  LOGIN: "api/v1/auth/login",
  REGISTER: "api/v1/auth/register",
  GET_USER_INFO: "api/v1/auth/getUser",
  DELETE_ACCOUNT: "api/v1/auth/deleteAccount"
}

// Expense Management APIs
EXPENSE: {
  ADD_EXPENSE: "api/v1/expense/add",
  GET_ALL_EXPENSE: "api/v1/expense/get",
  DELETE_EXPENSE: (id) => `api/v1/expense/${id}`,
  DOWNLOAD_EXPENSE: "api/v1/expense/downloadexcel"
}

// Income Management APIs
INCOME: {
  ADD_INCOME: "api/v1/income/add",
  GET_ALL_INCOME: "api/v1/income/get",
  DELETE_INCOME: (id) => `api/v1/income/${id}`,
  DOWNLOAD_INCOME: "api/v1/income/downloadexcel"
}
```

### **Error Handling**

- **Global Error Interceptor**: Handles 401 (unauthorized) and 500 (server error) responses
- **User-Friendly Messages**: Converts API errors to readable messages
- **Toast Notifications**: Real-time error and success feedback
- **Automatic Redirects**: Redirects to login on authentication failures

## 🎯 Key Features Deep Dive

### **Authentication Flow**

1. **Registration**: User creates account with email verification
2. **Login**: JWT token received and stored in localStorage
3. **Auto-Login**: Token validation on app startup
4. **Protected Routes**: Automatic redirection for unauthenticated users
5. **Logout**: Token removal and state cleanup

### **Expense Management**

1. **Add Expense**: Form with category, amount, date, and emoji selection
2. **Expense List**: Paginated list with search and filter capabilities
3. **Categories**: Custom categorization with emoji icons
4. **Analytics**: Visual charts showing expense distribution
5. **Export**: Excel download functionality

### **Income Tracking**

1. **Income Sources**: Multiple income stream tracking
2. **Income Analytics**: Monthly and yearly income analysis
3. **Visual Charts**: Pie and bar charts for income distribution
4. **Income Overview**: Comprehensive income summaries

### **Dashboard Analytics**

1. **Financial Overview**: Total balance, income, and expense visualization
2. **Recent Transactions**: Latest 10 transactions display
3. **Monthly Trends**: Month-over-month financial analysis
4. **Interactive Charts**: Hover effects and detailed tooltips

## 📱 Responsive Design

### **Breakpoints**

- **Mobile**: `< 640px` - Optimized for phones
- **Tablet**: `640px - 1024px` - Tablet-friendly layout
- **Desktop**: `> 1024px` - Full desktop experience
- **Large Desktop**: `> 1920px` - Ultra-wide screen support

### **Mobile Optimizations**

- **Touch-Friendly**: Large tap targets and swipe gestures
- **Responsive Charts**: Charts adapt to screen size
- **Mobile Navigation**: Collapsible sidebar for mobile
- **Optimized Forms**: Mobile-first form design

## 🔧 Development

### **Available Scripts**

```bash
# Start development server with hot reload
npm run dev

# Build for production
npm run build

# Preview production build locally
npm run preview

# Run ESLint for code quality
npm run lint
```

### **Code Quality**

- **ESLint Configuration**: Modern ESLint setup with React hooks rules
- **Code Formatting**: Consistent code style enforcement
- **Import Organization**: Structured import statements
- **Component Structure**: Consistent component organization

### **Development Best Practices**

- **Component Composition**: Reusable component architecture
- **State Management**: Context API for global state
- **Custom Hooks**: Reusable logic extraction
- **Error Boundaries**: Graceful error handling
- **Performance Optimization**: Lazy loading and memoization

## 🚀 Deployment

### **Build Configuration**

```javascript
// vite.config.js
export default defineConfig({
  plugins: [react(), tailwindcss()],
  build: {
    outDir: "dist",
    sourcemap: true,
    minify: "terser",
  },
});
```

### **Production Deployment**

1. **Build the application**

   ```bash
   npm run build
   ```

2. **Deploy to hosting platform**
   - **Vercel**: Connect GitHub repository for automatic deployments
   - **Netlify**: Drag and drop `dist` folder or connect repository
   - **AWS S3**: Upload `dist` folder to S3 bucket with static hosting
   - **GitHub Pages**: Use GitHub Actions for automated deployment

### **Environment Configuration**

Update API endpoints for production:

```javascript
// src/utils/apiPaths.js
export const BASE_URL =
  process.env.NODE_ENV === "production"
    ? "https://your-api-domain.com"
    : "http://localhost:5000";
```

## 🧪 Testing

### **Manual Testing Checklist**

- [ ] User registration and login flow
- [ ] Add/edit/delete expenses and income
- [ ] Chart rendering and responsiveness
- [ ] Mobile device compatibility
- [ ] Error handling and validation
- [ ] Data persistence and synchronization

### **Browser Compatibility**

- ✅ Chrome (90+)
- ✅ Firefox (88+)
- ✅ Safari (14+)
- ✅ Edge (90+)
- ✅ Mobile browsers (iOS Safari, Chrome Mobile)

## 🎨 Customization

### **Theme Customization**

Update Tailwind configuration in `src/index.css`:

```css
@theme {
  --color-primary: #your-primary-color;
  --font-display: "Your-Font", "sans-serif";
}
```

### **Component Styling**

All components use Tailwind utility classes for easy customization:

```jsx
// Easy style customization
<button className="btn-primary hover:bg-your-color">Custom Button</button>
```

### **Chart Colors**

Update chart color schemes:

```javascript
const COLORS = ["#875CF5", "#FA2C37", "#FF6900", "#your-color"];
```

## 🤝 Contributing

1. Fork the repository
2. Create a feature branch (`git checkout -b feature/amazing-feature`)
3. Follow the existing code style and structure
4. Test your changes thoroughly
5. Commit your changes (`git commit -m 'Add some amazing feature'`)
6. Push to the branch (`git push origin feature/amazing-feature`)
7. Open a Pull Request

### **Contribution Guidelines**

- Follow React best practices and hooks patterns
- Maintain consistent component structure
- Add appropriate PropTypes or TypeScript types
- Ensure responsive design compatibility
- Test on multiple browsers and devices

## 📋 Browser Support

| Feature       | Chrome | Firefox | Safari | Edge |
| ------------- | ------ | ------- | ------ | ---- |
| ES6+ Support  | ✅     | ✅      | ✅     | ✅   |
| CSS Grid      | ✅     | ✅      | ✅     | ✅   |
| Flexbox       | ✅     | ✅      | ✅     | ✅   |
| Local Storage | ✅     | ✅      | ✅     | ✅   |
| Fetch API     | ✅     | ✅      | ✅     | ✅   |

## 🔍 Performance Optimization

### **Bundle Optimization**

- **Code Splitting**: Automatic route-based code splitting
- **Tree Shaking**: Unused code elimination
- **Asset Optimization**: Image and resource optimization
- **Lazy Loading**: Component lazy loading for better performance

### **Runtime Performance**

- **React Hooks**: Efficient state management with hooks
- **Memoization**: Component and calculation memoization
- **Virtual Scrolling**: Large list performance optimization
- **Debounced Search**: Optimized search functionality

## 🙏 Acknowledgments

- **React Team** for the amazing React framework
- **Vite Team** for the lightning-fast build tool
- **Tailwind CSS** for the utility-first CSS framework
- **Recharts** for beautiful and responsive charts
- **Open Source Community** for the incredible ecosystem

## 📞 Support

If you encounter any issues or have questions:

1. **Check the Issues**: Look through existing GitHub issues
2. **Create New Issue**: Provide detailed information about the problem
3. **Documentation**: Refer to the inline code documentation
4. **Community**: Join our community discussions

### **Common Issues & Solutions**

**Q: Charts not rendering properly?**
A: Ensure the container has proper dimensions and data is in the correct format.

**Q: Authentication not working?**
A: Check if the backend API is running and CORS is properly configured.

**Q: Mobile layout issues?**
A: Verify Tailwind responsive classes are applied correctly.

</div>

---

<div align="center">

**Built with ❤️ using React, Vite, and Tailwind CSS**

**Happy Coding! 🚀**

</div>
