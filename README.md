# MERN Productivity Tracker

This is a full-stack productivity tracker application designed to help you monitor your time on different websites, block distracting sites, and visualize your productivity through a data-driven dashboard.

The project consists of three main components:
1.  **Chrome Extension**: Tracks website usage and allows blocking of specified sites.
2.  **Node.js/Express Backend**: A RESTful API for user authentication and data storage.
3.  **React Dashboard**: A web-based dashboard to visualize productivity data.

## Project Structure

```
productivity-tracker/
├── dashboard/      # React frontend for data visualization
├── extension/      # Chrome extension source code
└── server/         # Node.js/Express/MongoDB backend
```

## Getting Started

### Prerequisites

*   Node.js and npm
*   MongoDB (local or a cloud instance like MongoDB Atlas)
*   Google Chrome

### 1. Backend Setup

1.  **Navigate to the server directory:**
    ```bash
    cd server
    ```
2.  **Install dependencies:**
    ```bash
    npm install
    ```
3.  **Create a `.env` file** in the `server` directory and add your MongoDB connection string and a JWT secret:
    ```
    MONGO_URI=your_mongodb_connection_string
    JWT_SECRET=your_jwt_secret
    ```
4.  **Start the server:**
    ```bash
    npm start
    ```
    The backend will be running on `http://localhost:5000`.

### 2. Frontend (Dashboard) Setup

1.  **Navigate to the dashboard directory:**
    ```bash
    cd dashboard
    ```
2.  **Install dependencies:**
    ```bash
    npm install
    ```
3.  **Start the React development server:**
    ```bash
    npm start
    ```
    The dashboard will be accessible at `http://localhost:3000`.

### 3. Chrome Extension Setup

1.  Open Google Chrome and navigate to `chrome://extensions`.
2.  Enable **"Developer mode"** in the top right corner.
3.  Click on **"Load unpacked"**.
4.  Select the `extension` folder from the project directory.
5.  The productivity tracker extension should now be active in your browser.