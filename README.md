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
   **Windows**
   ```bash
   venv\Scripts\activate
    ```
   **mac**
   ```bash
   source venv/bin/activate
    ```
   for windows: ``` venv\Scripts\activate ```
   for mac: ``` source venv/bin/activate ```
5. Install Dependencies
   ``` bash
   pip install -r requirements.txt
   ```
   To verify installation:
   ``` bash
   pip list
   ```
   You should see: `Flask, mysql-connector-python, python-dotenv`
6. Environment Configuration
   for windows: `copy .env.example .env`
   for mac: `cp .env.example .env `
   Then edit the .env file:
   ``` bash
   DB_HOST=localhost
   DB_USER=root
   DB_PASSWORD=your_mysql_password
   DB_NAME=cinema
   ```
7. Setup Database
8. ```md
   6.1. Open MySQL  
   6.2. Run the SQL script provided in this project  
   6.3. This will create all required tables, views, and sample data  
9. Run Backend
   ``` bash
   cd cn230-cinema-booking-system/backend
   ```
   ``` bash
   python app.py
   ```

## Features
1. Movie booking system
2. Seat reservation
3. User management
4. Payment handling

## Tech Stack
1. Backend: Flask
2. Database: MySQL
3. Environment: Python (venv)
