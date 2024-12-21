Simple Portfolio Tracker
A web application that allows users to manage their stock portfolios, view real-time stock prices, and track key portfolio metrics.

Features
Add, edit, view, and delete stock holdings.
Real-time stock price integration.
Dashboard displaying key metrics like total portfolio value, top-performing stocks, and portfolio distribution.
Steps to Run the Project Locally
Prerequisites
Node.js and npm installed for the frontend.
Java JDK and Maven installed for the backend.
MySQL installed and running.
Frontend Setup
Navigate to the frontend folder:
cd frontend

Install dependencies:
npm install

Start the development server:
npm start

Access the application at http://localhost:3000.


Backend Setup
Navigate to the backend folder:
cd backend

Build the project:
mvn clean install

Run the application:
java -jar target/<your-backend-jar-file>.jar

Backend API will be available at http://localhost:8080.


Database Setup
Open MySQL and create a new database:
CREATE DATABASE portfolio_tracker;

Import the schema provided in the /backend/src/main/resources folder.
Update application.properties in the backend to match your database credentials:
spring.datasource.url=jdbc:mysql://localhost:3306/portfolio_tracker
spring.datasource.username=<your-username>
spring.datasource.password=<your-password>


Assumptions and Limitations
The application assumes the user portfolio contains 5 predefined stocks with a quantity of 1 each.
Real-time stock price updates are dependent on a free API (e.g., Alpha Vantage) and may have usage limitations.
No authentication is implemented; the application is built for a single user.
Portfolio calculations assume all stock prices are fetched correctly and in USD.


Notes
Ensure the API key for the stock price API is correctly configured in both the frontend and backend.
Deployed application links and live API documentation will be added post-deployment.
