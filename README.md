# Cinema Booking System
## Project Setup
1. Clone the repository
   ```bash git clone https://github.com/WuBingXue49/cn230-cinema-booking-system.git
   ```md ```bash cd cn230-cinema-booking-system/backend
2. Create Virtual Environment
   `python -m venv venv`
3. Activate Virtual Environment
   for windows: `venv\Scripts\activate`
   for mac: `source venv/bin/activate`
4. Install Dependencies
   `pip install -r requirements.txt`
   To check if you have all required packages: `pip list` you should see: Flask, mysql-connector-python, python-dotenv
5. Environment Configuration
   for windows: `copy .env.example .env`
   for mac: `cp .env.example .env `
   after that go to .env file and change DB_PASSWORD = your_mysql_password
6. Setup Database
   open MySQL and SQL script in this project
7. Run Backend
   `cd cn230-cinema-booking-system/backend`
   `python app.py`

## Features
1. Movie booking system
2. Seat reservation
3. User management
4. Payment handling

## Tech Stack
1. Backend: Flask
2. Database: MySQL
3. Environment: Python (venv)
