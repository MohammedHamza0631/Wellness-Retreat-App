# Wellness Retreat Webpage

This project is a Wellness Retreat Webpage that allows users to browse and book various retreats. The application provides a smooth and interactive user experience, leveraging modern technologies such as React, ShadCN, and TailwindCSS for the frontend, and Node.js with Express and PostgreSQL for the backend and database.

## Table of Contents
- [Features](#features)
- [Tech Stack](#tech-stack)
- [Installation](#installation)
- [Usage](#usage)
- [API Endpoints](#api-endpoints)
- [License](#license)

## Live Link
- To access the live project, go [here](https://wellness-client.vercel.app/).

## Features

- **User Authentication**: Users can register and log in using custom forms.
- **Retreat Browsing**: Users can browse available retreats and view detailed information.
- **Pagination**: Retreats are displayed with pagination for easy navigation.
- **Retreat Booking**: Users can book retreats and view their booking status.

## Tech Stack

- **Frontend**: React, ShadCN, TailwindCSS, TypeScript
- **Backend**: Node.js, Express
- **Database**: PostgreSQL
- **Authentication**: Authentication using JWT Tokens

## Installation

1. Clone the repository:
    ```bash
    git clone https://github.com/your-username/wellness-retreat-webpage.git
    cd wellness-retreat-webpage
    ```

2. Install backend dependencies:
    ```bash
    cd server
    npm install
    ```

3. Install frontend dependencies:
    ```bash
    cd ../client
    npm install
    ```
4. Set up a cloud database:
   - Go to Railway and create an account.
   - Create a new Postgrs Deployment
   - Copy your connection URL.

6. Configure environment variables:
    - Create a `.env` file in the `backend` directory and add the following:
    ```bash
    PORT=5000
    DATABASE_URL=your_database_url
    JWT_SECRET=your_jwt_secret
    ```

7. Start the backend server:
    ```bash
    cd backend
    npm start
    ```

8. Start the frontend development server:
    ```bash
    cd ../frontend
    npm start
    ```

## Usage

1. **Register/Login**: Users can register a new account or log in using the custom forms provided.
2. **Browse Retreats**: Users can browse available retreats and view detailed information.
3. **Book Retreats**: Users can book retreats and view their booking status.
4. **Pagination**: Navigate through retreats using pagination.

## API Endpoints

- **Authentication**
  - `POST /api/auth/register`: Register a new user
  - `POST /api/auth/login`: Login with user credentials

- **Retreats**
  - `GET /api/retreats`: Get all retreats with pagination
  - `GET /api/retreats/search`: Get retreats based on searchTerm

- **Bookings**
  - `POST /api/book/:retreatId`: Create a booking
  - `GET /api/book/:userId`: Check booking status



## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.
