
---

# REST_API

A simple RESTful API built using Django REST Framework (DRF) that performs CRUD operations on user data, including name and age.

## Features

- **Create** a new user with a name and age.
- **Read** user details.
- **Update** an existing user's details.
- **Delete** a user.

## Technologies Used

- **Python** (Django & Django REST Framework)
- **SQLite3** (default database)

## Installation

1. **Clone the repository**  
   ```bash
   git clone https://github.com/DhananjayaBandara/REST_API.git
   cd REST_API
   ```

2. **Create a virtual environment (optional but recommended)**  
   ```bash
   python -m venv venv
   source venv/bin/activate  # On Windows use: venv\Scripts\activate
   ```

3. **Install dependencies**  
   ```bash
   pip install -r requirements.txt
   ```

4. **Run database migrations**  
   ```bash
   python manage.py migrate
   ```

5. **Start the development server**  
   ```bash
   python manage.py runserver
   ```

## API Endpoints

| Method | Endpoint       | Description           |
|--------|--------------|-----------------------|
| `POST`   | `/api/users/`      | Create a new user  |
| `GET`    | `/api/users/`      | Get all users      |
| `GET`    | `/api/users/<id>/` | Get a specific user  |
| `PUT`    | `/api/users/<id>/` | Update user details |
| `DELETE` | `/api/users/<id>/` | Delete a user      |

## Testing the API

- Use **Postman** or **cURL** to test API requests.
- Example **POST request** to create a user:
  ```json
  {
      "name": "John Doe",
      "age": 25
  }
  ```
