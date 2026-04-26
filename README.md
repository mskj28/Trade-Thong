# Cinema Booking System
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
**1. Movie booking system:** <br> Allows users to browse available movies, view showtimes, and create bookings for selected shows.
**2. Seat reservation:** <br> Enables users to select specific seats for a chosen showtime with real-time availability checking to prevent double booking.
**3. User management:** <br> Supports different user roles (e.g., customer, staff, admin) with basic account data stored in the system.
**4. Payment handling:** <br> Manages booking payments, including payment status (e.g., pending, confirmed, refunded).

## Tech Stack
1. Backend: Flask
2. Database: MySQL
3. Environment: Python (venv)
