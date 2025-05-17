# Groove Up - Your Personalized Music Streaming Experience

## Overview

Groove Up is a modern, Spotify-inspired music streaming web application built with the MERN stack (MongoDB, Express.js, React.js, Node.js). It offers a seamless and intuitive platform to discover, listen to, and organize your favorite music. Key features include secure user authentication, core audio playback functionality, and the ability to create and manage personalized playlists.

## Technologies Used

* **Frontend:**
    * [React.js](https://react.dev/) - A JavaScript library for building user interfaces.
    * [Redux](https://redux.js.org/) (or Context API) - For state management.
    * [Axios](https://axios-http.com/docs/intro) - For making HTTP requests to the backend.
    * [Styled-components](https://styled-components.com/) (or CSS Modules/vanilla CSS) - For styling components.
* **Backend:**
    * [Node.js](https://nodejs.org/en/) - A JavaScript runtime environment.
    * [Express.js](https://expressjs.com/) - A minimalist and flexible Node.js web application framework.
    * [jsonwebtoken](https://www.npmjs.com/package/jsonwebtoken) - For secure user authentication using JWT.
    * [bcrypt](https://www.npmjs.com/package/bcrypt) - For password hashing.
* **Database:**
    * [MongoDB](https://www.mongodb.com/) - A NoSQL database for storing user data, music information, and playlists.
    * [Mongoose](https://mongoosejs.com/) - An elegant MongoDB object modeling for Node.js.

## Features

* **User Authentication:**
    * Secure user registration and login.
    * Password hashing for enhanced security.
* **Core Playback Functionality:**
    * Browse and search for music.
    * Play, pause, skip tracks.
    * Progress bar for controlling playback position.
    * Volume control.
* **Playlist Management:**
    * Create new playlists.
    * Add and remove songs from playlists.
    * View and manage personal playlists.
* **Data Management:**
    * Efficient storage and retrieval of user data, music metadata, and playlist information using MongoDB.
    * Well-structured backend API built with Express.js.
* **Responsive Design:** (Optional, but recommended)
    * The application is designed to work seamlessly across various devices and screen sizes.

## Setup and Installation

To run Groove Up locally, follow these steps:

1.  **Clone the repository:**
    ```bash
    git clone <repository_url>
    cd groove-up
    ```

2.  **Install backend dependencies:**
    ```bash
    cd backend
    npm install
    ```

3.  **Configure MongoDB:**
    * Ensure you have MongoDB installed and running.
    * Create a `.env` file in the `backend` directory and add your MongoDB connection URI:
        ```env
        MONGODB_URI=mongodb://localhost:27017/grooveup
        JWT_SECRET=<your_secret_key>
        ```
        Replace `<your_secret_key>` with a strong, random secret key for JWT.

4.  **Run the backend server:**
    ```bash
    npm start
    ```
    The backend server should now be running on `http://localhost:<port>` (default is usually 5000).

5.  **Install frontend dependencies:**
    ```bash
    cd ../frontend
    npm install
    ```

6.  **Configure frontend environment variables:**
    * Create a `.env.local` file in the `frontend` directory and set the backend API URL:
        ```env
        REACT_APP_API_URL=http://localhost:5000
        ```

7.  **Run the frontend application:**
    ```bash
    npm start
    ```
    The frontend application should now be running on `http://localhost:3000` (or another available port).

## Project Structure
