# Task Tracker Web Application

This is a simple web application built with Django and MySQL for tracking tasks or to-do items. Follow the instructions below to set up and run the project.

## Prerequisites

- Python 3.x installed on your system.
- MySQL installed and running on your system.
- Git installed on your system.

## Getting Started

### 1. Clone the Repository

Clone the project repository to your local machine using Git:

```bash
git clone https://github.com/your-username/task-tracker.git
```

### 2. Create a Virtual Environment

Navigate to the project directory and create a virtual environment. You can use `virtualenv` or `venv` depending on your preference:

```bash
cd task-tracker
python -m venv venv
```

Activate the virtual environment:

**On Windows:**

```bash
venv\Scripts\activate
```

**On macOS and Linux:**

```bash
source venv/bin/activate
```

### 3. Install Dependencies

Install the project dependencies using `pip`:

```bash
pip install -r requirements.txt
```

### 4. Configure Environment Variables

Copy the environment variables from the `env.example` file to a new `.env` file in the project root:

```bash
cp env.example .env
```

Edit the `.env` file and provide values for the following variables:

- `DEBUG`: Set to `True` for development, and `False` for production.
- `DB_NAME`: Name of your MySQL database.
- `DB_USER`: Your MySQL username.
- `DB_PASSWORD`: Your MySQL password.
- `DB_HOST`: Host where your MySQL server is running (usually 'localhost' for local development).
- `DB_PORT`: Port on which MySQL is running (usually '3306' for MySQL).

### 5. Migrate the Database

Run the database migrations to create the necessary tables:

```bash
python manage.py migrate
```

### 6. Run the Application

Start the Django development server:

```bash
python manage.py runserver
```

The application will be accessible at `http://localhost:8000/` in your web browser.

## Usage

- Visit `http://localhost:8000/` to access the task tracker application.
- Sign up for a new account or log in if you already have one.
- Create, edit, and manage your tasks.

## Contributing

If you'd like to contribute to this project, please open an issue or create a pull request. We welcome contributions!

