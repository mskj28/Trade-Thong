# Movy: Cinema Booking System

## Member: 
6710
6710615177 น.ส. ฟาร์ริดา มูลรังษี
6710615219 น.ส. มิ่งขวัญ ใสกระจ่าง
## Project Overview
This project is a cinema booking system that allows users to browse movies, select showtimes, reserve seats, and manage bookings with payment handling through a database-driven backend.

## Stakeholders
1. Customer – Browse movies, book seats, make payments
2. Staff – Manage bookings and verify transactions
3. Admin – Manage movies, showtimes, and users

## Functional Requirements
1. The system must allow users to browse movies and showtimes
2. The system must allow users to reserve seats
3. The system must prevent double booking
4. The system must allow booking cancellation
5. The system must calculate total price automatically
6. The system must manage payment status

## Database Design 
ER Diagram Full View: [View here](https://canva.link/h8gbjaoj3cw3ecw)  
ER Diagram Preview:  
<p align="center">
  <img src="docs/er-diagram.png" width="600">
</p>

## Project Structure
```bash
backend/
├── app.py
├── auth.py
├── routes/
|    ├──booking.py
|    ├──movies.py
|    ├──showtime.py
|    └──user.py
├── db.py
├── config.py
├── requirements.txt
├──.env
└── .env.example
```

## Project Setup
1. Clone the repository
   ``` bash
   git clone https://github.com/WuBingXue49/cn230-cinema-booking-system.git
   cd cn230-cinema-booking-system/backend
   ```
2. Create Virtual Environment
   ``` bash
   python -m venv venv
   ```
3. Activate Virtual Environment  
   **For Windows**
   ```bash
   venv\Scripts\activate
    ```
   **For Mac**  
   ```bash
   source venv/bin/activate
    ```
4. Install Dependencies
   ``` bash
   pip install -r requirements.txt
   ```
   To verify installation:
   ``` bash
   pip list
   ```
   You should see: `Flask, mysql-connector-python, python-dotenv`
5. Environment Configuration
   **For Windows**
   ```bash
   copy .env.example .env
    ```
   **For Mac**  
   ```bash
   cp .env.example .env
    ```
   Then edit the .env file:
   ```
   DB_HOST=localhost  
   DB_USER=root  
   DB_PASSWORD=your_mysql_password  
   DB_NAME=cinema  
   ```
6. Setup Database  
   6.1. Open MySQL  
   6.2. Run the SQL script provided in this project  
   6.3. This will create all required tables, views, and sample data  
7. Run Backend
   ``` bash
   cd cn230-cinema-booking-system/backend
   ```
   ``` bash
   python app.py
   ```

## Features
1. Movie booking system: <br> Allows users to browse available movies, view showtimes, and create bookings for selected shows. <br>
2. Seat reservation: <br> Enables users to select specific seats for a chosen showtime with real-time availability checking to prevent double booking. <br>
3. User management: <br> Supports different user roles (e.g., customer, staff, admin) with basic account data stored in the system. <br>
4. Payment handling: <br> Manages booking payments, including payment status (e.g., pending, confirmed, refunded). <br>

## Tech Stack
1. Backend: Flask <br> A lightweight Python web framework used to build RESTful APIs and handle server-side logic. <br>
2. Database: MySQL <br> Relational database used to store all system data such as users, movies, bookings, and payments. <br>
3. Environment: Python (venv) <br> Virtual environment used to isolate project dependencies and ensure consistent setup across different machines. <br>

