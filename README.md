# eDiary_backend

eDiarySchool is a web-based application built using Node.js, Express, and MongoDB. This repository contains the backend code for the eDiarySchool project.

## Features
- User Authentication (Login/Registration)
- Role-based Access Control (Student, Teacher, Parent)
- eDiary Management
- Attendance 
- Communication between Teachers and Parents
- Notifications and Reminders

## Installation

1. **Clone the repository:**
    ```bash
    git clone https://github.com/your-username/eDiarySchool-backend.git
    cd eDiarySchool-backend
    ```

2. **Install dependencies:**
    ```bash
    npm install
    ```

3. **Set up environment variables:**
    Create a `.env` file in the root directory with the following contents:
    ```plaintext
    MONGO_URI=your_mongodb_connection_string
    JWT_SECRET=your_jwt_secret
    PORT=5000
    ```

## Usage

1. **Run the application:**
    ```bash
    npm run dev
    ```

2. The backend server will start and listen on the port specified in the `.env` file (default is `http://localhost:5000`).

## API Endpoints

Here are some of the key API endpoints:

### Auth
- **POST** `/api/auth/register` - Register a new user
- **POST** `/api/auth/login` - Login a user

### Users
- **GET** `/api/users` - Get all users (restricted to admins)
- **GET** `/api/users/:id` - Get a specific user by ID
- **PUT** `/api/users/:id` - Update user information
- **DELETE** `/api/users/:id` - Delete a user

### Diaries
- **GET** `/api/diaries` - Get all diaries
- **POST** `/api/diaries` - Create a new diary
- **GET** `/api/diaries/:id` - Get a specific diary by ID
- **PUT** `/api/diaries/:id` - Update a diary
- **DELETE** `/api/diaries/:id` - Delete a diary

### Assignments
- **GET** `/api/assignments` - Get all assignments
- **POST** `/api/assignments` - Create a new assignment
- **GET** `/api/assignments/:id` - Get a specific assignment by ID
- **PUT** `/api/assignments/:id` - Update an assignment
- **DELETE** `/api/assignments/:id` - Delete an assignment

## Technologies Used

- **Node.js:** JavaScript runtime for building the backend server.
- **Express:** Backend framework for building the RESTful API.
- **MongoDB:** NoSQL database for storing application data.
- **Mongoose:** ODM library for MongoDB and Node.js.
- **JWT:** For handling user authentication and authorization.

## Contributing

1. Fork the repository.
2. Create a new branch (`git checkout -b feature-branch`).
3. Make your changes and commit them (`git commit -m 'Add new feature'`).
4. Push to the branch (`git push origin feature-branch`).
5. Open a Pull Request.
