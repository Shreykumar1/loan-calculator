# Loan Calculator

## About This App

This Loan Calculator App is a modern, single-page web application built using React JS and Material UI. It allows users to calculate loan EMIs (Equated Monthly Installments), view a detailed amortization schedule, and see real-time currency conversions of their EMI using live exchange rates.

## Live Demo
https://loan-horizon.netlify.app/


## Features

- Loan EMI calculation using standard financial formulas
- Dynamic amortization schedule table with monthly breakdown
- Real-time currency conversion of EMI using a live exchange rate API
- Paginated exchange rate table for 160+ currencies
- Dark/Light mode toggle for a customizable experience
- Collapsible header navigation on mobile screens
- Fully responsive UI built with Material UI

## Technologies Used

This project is built with:

- React (Hooks, Routing, Context API)
- Vite
- TypeScript
- Material UI for styling and responsive components
- Tailwind CSS (if still used, otherwise remove)
- Axios for API calls
- Exchange Rate API for real-time currency conversion

## Getting Started

Follow these steps to set up the project locally:

```sh
# Step 1: Clone the repository using the project's Git URL.
git clone https://github.com/Shreykumar1/loan-calculator.git

# Step 2: Navigate to the project directory.
cd loan-calculator # Or the actual project directory name

# Step 3: Install the necessary dependencies.
npm i

# Step 4: Set up your API Key
# You must register and obtain a free API key from ExchangeRate-API.
# Then, locate where YOUR_API_KEY is used in the app code (e.g., in a .env file or directly in a service file)
# and replace it with your actual key.

# Step 5: Start the development server.
npm run dev
```

## EMI Formula Used

The EMI (Equated Monthly Installment) is calculated using the standard formula:

\[EMI = \frac{P \times R \times (1+R)^N}{(1+R)^N – 1}\]

Where:

-   `P` = Principal loan amount
-   `R` = Monthly interest rate (annual rate / 12 / 100)
-   `N` = Loan duration in months

## Currency Conversion API

This app integrates with the free tier of the [ExchangeRate-API](https://www.exchangerate-api.com/) to fetch live exchange rates.

**API Endpoint Example:**
`https://v6.exchangerate-api.com/v6/YOUR_API_KEY/latest/USD`