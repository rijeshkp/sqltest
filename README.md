Python MySQL Touchstone Project

This project demonstrates how to use Python to connect to a MySQL database, perform basic CRUD (Create, Read, Update, Delete) operations, and manage database interactions. It’s a beginner-friendly example to get started with MySQL in Python.

Features

Connect to a MySQL database using mysql-connector-python.

Create a users table.

Insert touchstone data into the table.

Retrieve and display data from the database.

Project Structure

python-mysql-touchstone/
│
├── app.py                # Main application script
├── requirements.txt      # Python dependencies
└── config.py             # Database configuration

Requirements

Python 3.8 or later

MySQL Server

mysql-connector-python package

Setup Instructions

1. Clone the Repository

git clone <your_repository_url>
cd python-mysql-touchstone

2. Install Dependencies

Install the required Python libraries using:

pip install -r requirements.txt

3. Configure the Database

Ensure MySQL is running on your machine.

Create a MySQL database named touchstone_db:

CREATE DATABASE touchstone_db;

Update the config.py file with your MySQL credentials:

DATABASE_CONFIG = {
    'host': 'localhost',
    'user': 'your_username',
    'password': 'your_password',
    'database': 'touchstone_db'
}

4. Run the Application

Run the main script to create the table, insert touchstone data, and fetch it:

python app.py

Expected Output

When you run the script, you should see output similar to:

Connected to MySQL database!
Table 'users' created successfully.
3 rows inserted.
Fetched Data:
(1, 'Alice', 25, 'alice@example.com')
(2, 'Bob', 30, 'bob@example.com')
(3, 'Charlie', 35, 'charlie@example.com')
Connection closed.

Usage

You can modify the app.py script to add more complex database operations like updates, deletes, or joins. This project is a starting point for learning Python and MySQL integration.

Contributing

Feel free to fork this repository, make changes, and submit pull requests. Contributions are welcome!

License

This project is licensed under the MIT License. See the LICENSE file for details.
