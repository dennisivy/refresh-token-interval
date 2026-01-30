# Refreshing Tokens With Fetch | Custom Interceptor

<img width="1881" height="882" alt="Screenshot 2026-01-30 at 9 45 25 AM" src="https://github.com/user-attachments/assets/fae05c12-ee7f-409b-83dc-89d2b72cb9f6" />

## About

This repository demonstrates how to implement JWT token refresh functionality using the Fetch API with a custom interceptor. It's a companion project for the YouTube tutorial on handling access and refresh tokens in web applications.

**Tutorial Video:** [Watch on YouTube](https://www.youtube.com/watch?v=16-1mTdGBoM)

## Tech Stack

- **Backend:** Django REST Framework with Simple JWT
- **Frontend:** React with React Router
- **Authentication:** JWT (JSON Web Tokens)

## Prerequisites

Before you begin, ensure you have the following installed:

- Python 3.x
- Node.js and npm
- Git

## Installation

Clone the repository:

```bash
git clone https://github.com/dennisivy/refresh-token-interval
cd refresh-token-interval
```

## Setup

### Backend Setup

1. Navigate to the backend directory:
   ```bash
   cd backend
   ```

2. Install Python dependencies:
   ```bash
   pip install -r requirements.txt
   ```

3. Run database migrations:
   ```bash
   python manage.py migrate
   ```

4. Create a superuser account:
   ```bash
   python manage.py createsuperuser
   ```

5. Start the Django development server:
   ```bash
   python manage.py runserver
   ```

The backend will be running at `http://localhost:8000`

### Frontend Setup

1. Navigate to the frontend directory (from the project root):
   ```bash
   cd frontend
   ```

2. Install Node.js dependencies:
   ```bash
   npm install
   ```

3. Start the React development server:
   ```bash
   npm start
   ```

The frontend will be running at `http://localhost:3000`

## Usage

1. Make sure both the backend and frontend servers are running
2. Open your browser and navigate to `http://localhost:3000`
3. Log in with the superuser credentials you created
4. The application will automatically handle token refresh using the custom interceptor
