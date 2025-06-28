# SlidesManager

SlidesManager is a full-stack web application designed for educators to create, store, and manage study content modules. Educators can control access to their modules by setting them as public or private, while students can easily browse available content. Real-time chat functionality is integrated to enhance networking and communication between users.

## Key Features

- **User Authentication and Authorization**:
  - Secure login and access management using JSON Web Tokens (JWT).
  
- **Module Creation and Management**:
  - Educators can create, store, and manage study modules, with options to set their content as public or private.

- **Real-time Chat**:
  - Socket.IO-powered chat functionality for real-time communication between educators and students.

## Tech Stack

- **Frontend**: React.js
- **Backend**: Node.js with Express
- **Database**: MongoDB
- **Authentication**: JSON Web Tokens (JWT)
- **Real-time Communication**: Socket.IO
- **Styling**: Tailwind CSS

## Getting Started

### Prerequisites

Make sure you have the following tools installed:

- **Node.js**: v14+ 
- **MongoDB**: v4.4+

### Installation

1. Clone the repository:
    ```bash
    git clone [https://github.com/Phoenix_681/slidesmanager.git]
    cd slidesmanager
    ```

2. Install backend dependencies:
    ```bash
    cd backend
    npm install
    ```

3. Install frontend dependencies:
    ```bash
    cd frontend
    npm install
    ```

4. Setup MongoDB:
   - Make sure MongoDB is running locally or provide a remote connection URL in `.env`.

5. Configure environment variables:
   - Create a `.env` file in the root of your backend directory and add the following:
     ```bash
     PORT=5000
     JWT_SECRET=your_jwt_secret
     MONGO_URI=your_mongodb_connection_string
     ```

### Running the Application

1. Start the backend server:
    ```bash
    cd backend
    npm run start
    ```

2. Start the frontend:
    ```bash
    cd frontend
    npm run start
    ```

3. Open the application in your browser at `http://localhost:3000`.

### Folder Structure

```bash
slidesmanager/
├── backend/         # Express server for API and authentication
│   ├── models/      # MongoDB models
│   ├── routes/      # API routes for user management, modules, etc.
│   └── server.js    # Main server file
├── frontend/        # React application for user interface
│   ├── src/         # React components, hooks, and context
│   └── public/      # Static assets
├── .env             # Environment configuration (ignored in repo)
└── README.md        # Project documentation

