# Stock Portfolio Tracker

A web application to help users manage and track their stock portfolios. Built with Django REST Framework for the backend, MySQL for data storage and React JS framework for frontend.

---

## Features

- **User Authentication**: Secure login and signup.
- **Portfolio Management**: Add, update, and remove stocks in your portfolio.
- **Real-time Market Data**: Fetch the latest stock prices and calculate portfolio performance.
- **Cost Prediction**: Take a look at our stock cost prediction through Machine Learning models to take better decisions.
---

## Tech Stack

- **Frontend**: React JS
- **Backend**: Django REST Framework
- **Database**: MySQL
- **API**: Integration with third-party stock market APIs of Alpha Vantage & Yahoo Finance
- **Hosting**: Vercel for Frontend & Render for Backend

---

## Installation and Setup

1. **Clone the Repository**
   ```bash
   git clone https://github.com/Devansh-Kushwaha/StockPortfolio-PredictorApp.git
   cd stock-portfolio-tracker

2. **Set Up Virtual Environment**
   ```bash
   python -m venv venv
   source venv/bin/activate  # On Windows: venv\Scripts\activate

3. **Install Dependencies**
   ```bash
   pip install -r requirements.txt

4. **Set Up Environment Variables**
   Create a .env file in the project root and add the following:
   ```bash
   API_KEY=your_api_keY
   DATABASE_PASSWORD=your_database_password
   DATABASE_USER=your_database_username
   DATABASE_NAME=your_database_name

6. **Run Migrations**
   ```bash
   python manage.py makemigrations
   python manage.py migrate
   
8. **Run the Development Server**
   ```bash
   npm run dev (for frontend)
   python manage.py runserver (for backend)
    
