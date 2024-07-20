# Ftrack2898

**Ftrack** is a comprehensive web application designed for personal financial management. It provides functionalities to manage expenses, income, loans, and profile details, with dynamic visualizations and transaction management.

## Table of Contents

- [Project Overview](#project-overview)
- [Technologies Used](#technologies-used)
- [Features](#features)
- [Installation](#installation)
- [Usage](#usage)
- [File Structure](#file-structure)
- [License](#license)

## Project Overview

Ftrack is a full-stack application that allows users to track their financial activities, including:

- **Expenses**: Add, view, edit, and delete expense records.
- **Income**: Manage income sources with similar functionalities.
- **Loans**: Track loans given and received with detailed records.
- **Profile**: Manage user profile information and change passwords.
- **Dashboard**: View an overview of financial data and recent transactions with visualizations.

## Technologies Used

- **Frontend**:
  - **React**: For building the user interface.
  - **Recharts**: For visualizations (line charts and bar graphs).
  - **CSS**: For styling.

- **Backend**:
  - **Node.js**: For server-side logic.
  - **Express.js**: For API development.
  - **MongoDB**: For database management.
  - **Mongoose**: For MongoDB object modeling.

- **Authentication**:
  - **JWT (JSON Web Tokens)**: For user authentication.

## Features

- **Home Page**: Welcome page with navigation to login and signup.
- **Login/Signup**: User authentication with secure login and registration.
- **Dashboard**: Displays financial overview, visualizations, and recent transactions.
- **Update Page**: Manage and update expenses and income records.
- **Loans Page**: Track loans given and received with detailed records.
- **Profile Page**: Update user profile details and change password.

## Installation

### Clone the Repository

```bash
git clone https://github.com/yourusername/ftrack.git
cd ftrack
```

### Backend Setup

1. **Navigate to the server directory**:

    ```bash
    cd server
    ```

2. **Install dependencies**:

    ```bash
    npm install
    ```

3. **Create a `.env` file** in the `server` directory and add your MongoDB connection string:

    ```env
    MONGO_URI=mongodb+srv://<username>:<password>@cluster0.mongodb.net/mydatabase?retryWrites=true&w=majority
    PORT=5000
    ```

4. **Start the server**:

    ```bash
    node index.js
    ```

### Frontend Setup

1. **Navigate to the `src` directory**:

    ```bash
    cd ../src
    ```

2. **Install dependencies**:

    ```bash
    npm install
    ```

3. **Start the React application**:

    ```bash
    npm start
    ```

## Usage

1. **Access the application**: Open your web browser and navigate to `http://localhost:3000`.

2. **Login/Signup**: Use the login or signup page to authenticate or create a new account.

3. **Navigate through pages**: Use the navigation bar to access the Dashboard, Update Page, Loans Page, and Profile Page.

4. **Manage records**: Add, edit, and delete expenses, income, and loans through their respective pages.

## File Structure

```
ftrack/
├── server/
│   ├── models/
│   │   ├── Expense.js
│   │   ├── Income.js
│   │   ├── LoanGiven.js
│   │   ├── LoanTaken.js
│   │   ├── User.js
│   ├── routes/
│   │   ├── expenseRoutes.js
│   │   ├── incomeRoutes.js
│   │   ├── loanGivenRoutes.js
│   │   ├── loanTakenRoutes.js
│   │   ├── userRoutes.js
│   ├── middleware/
│   │   ├── authMiddleware.js
│   ├── .env
│   ├── index.js
├── src/
│   ├── components/
│   │   ├── Dashboard.js
│   │   ├── UpdatePage.js
│   │   ├── LoansPage.js
│   │   ├── ProfilePage.js
│   │   ├── Navbar.js
│   │   ├── LoginPage.js
│   │   ├── SignUpPage.js
│   ├── App.js
│   ├── index.js
│   ├── styles/
│   │   ├── LoginPage.css
│   │   ├── SignUpPage.css
│   │   ├── Dashboard.css
│   │   ├── UpdatePage.css
│   │   ├── LoansPage.css
│   │   ├── ProfilePage.css
│   │   ├── Navbar.css
```

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

