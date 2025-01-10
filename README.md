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

## API Endpoints

| Endpoint                  | Method | Description                     |
|---------------------------|--------|---------------------------------|
| `/api/stocks/`            | GET    | View portfolio                  |
| `/api/stocks/create/`     | POST   | Add a new stock                 |
| `/api/stocks/delete/<int:pk>`| DELETE| Remove a stock from the portfolio |
| `/api/stocks/update/<int:pk>`| PUT | Edit a stock in the portfolio   |
| `/api/stocks/ predict`    | POST   | Get predictions of a stock's costd |

## Future Enhancements

- Advanced Analytics: Risk analysis and portfolio diversification insights.
- Notifications: Real-time price alerts and updates.
- Multi-currency Support: Track portfolios in various currencies.

## Limitations

- **Live Prices**: The live stock prices are fetched only when the page is refreshed.  
- **Fallback for API Failures**: If any of the external APIs fail to return a response, the stock price is defaulted to `$100`. This serves as a debugging aid and helps in identifying API-related issues.

## Deployment

- **Frontend**: [Vercel](https://stock-portfolio-deployed.vercel.app/)


## Contributing
**Contributions are welcome! Please follow these steps:**

1. Fork the repository.
2. Create a new branch.
   ```bash
   git checkout -b feature-name
3. Commit your changes.
   ```bash
   git commit -m "Add feature-name"
4. Push to your forked repository.
   ```bash
   git push origin feature-name
5. Create a pull request.

## Licence
This project is licensed under the [MIT License](https://opensource.org/license/MIT). See the LICENSE file for details.

## Acknowledgements
- [Django REST Framework](https://www.django-rest-framework.org/)
- [MySQL](https://www.mysql.com/)
- [React JS](https://react.dev/)
- [Alpha Vantage](https://www.alphavantage.co/documentation/)
- [Yahoo Finance](https://finance.yahoo.com/)

## Contacts

**Devansh Kushwaha**  
Email: [devansh.67.kushwaha@gmail.com](devansh.67.kushwaha@gmail.com)  
GitHub: [Devansh-Kushwaha](https://github.com/Devansh-Kushwaha)  
LinkedIn: [Devansh Kushwaha](https://www.linkedin.com/in/devansh-kushwaha-333466267/)  

